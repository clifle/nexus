# Web applications

## Nexus Web

Nexus Web is the web interface for Blue Brain Nexus, allowing users to interact with data and perform administration tasks. It is being actively developed and new features are regularly added.

It currently contains the following features:

### Login

You can login with your user to access non-public resources (depending on your permissions).

![Login box](./assets/img/login-web.png)

#### Copy Auth Token for reuse with other Nexus-related tools

Once logged-in, you can copy your authentication token, in order to easily reuse it in, for example, an IPython Notebook or the Nexus CLI client.

![Copy token button](./assets/img/copy-token.gif)

### Browsing data

To group and control access to your data, Nexus provides you Organizations and Projects. Much like in Github (if you're familiar with it), there are Organizations which contain Projects (Repositories in Github), which in turn contain your data (files in GitHub, Resources in Nexus).

In Nexus Web, the landing page will show you the list of Organizations you have access to.

![List organizations](./assets/img/list-orgs.png)

After selecting an organization, you will see the list of Projects you have access to inside this organization.

![List projects](./assets/img/list-projects.png)

Select a Project, you'll get to the list of its Resources.

![List resources](./assets/img/list-resources.png)

You can search resources using the ElasticSearch query syntax.

![Search resources](./assets/img/search-resources.png)

Click on a resource and you'll see its full payload in a side panel, in the JSON-LD format.

![View resource](./assets/img/view-resource.png)

##### Advanced use-cases

If you want to have several filtered lists of resources side by side, you can create additional filterable lists by using the "New Query" button in the side panel. It can be handy to make comparisons, or to build a set of ElasticSearch queries we want to reuse in an IPython Notebook or in a script.

![New query button](./assets/img/new-query-button.png)
![New query](./assets/img/new-query.png)

You can also clone one of the active Queries to use it as a starting point.

![Clone query](./assets/img/clone-query.png)

If you need to make complex ElasticSearch queries or if you want to see the raw payload returned by ElasticSearch, you can click on "ElasticSearch query editor". Results will be displayed in JSON-LD format.

![ElasticSearch query button](./assets/img/es-query-button.png)
![ElasticSearch query](./assets/img/es-query.png)

For graph and RDF-related queries, we also offer a SPARQL query editor that runs against our triple-store. Results are displayed in a table.

![SPARQL query button](./assets/img/sparql-query-button.png)
![SPARQL query](./assets/img/sparql-query.png)

### Managing your Nexus instance

#### Creating an Organization

Click on the "Create organization" icon next to the title of the homepage to create a new organization.

![Create organization button](./assets/img/create-organization-button.png)
![Create organization](./assets/img/create-organization.png)

#### Editing or deprecating an Organization

On the list of organizations, click on the "edit" button that appear when hovering on an organization. You'll be able to edit the description of the organization and hit "Save" to modify it. To deprecate the organization, hit the "Deprecate" button.

![Edit organization button](./assets/img/edit-organization-button.png)
![Edit organization](./assets/img/edit-organization.png)

#### Creating a Project

Navigate to the organization where you want to create your project. Click on the "Create Project" icon next to the title of the page.

![Create project button](./assets/img/create-project-button.png)
![Create project](./assets/img/create-project.png)

#### Editing or deprecating a Project

Navigate to the organization where your project is. Click on the "Edit" button that appear when you hover a project in the list. You'll be able to edit its description and hit save to modify it. Hit "Deprecate" to deprecate the project.

![Edit project button](./assets/img/edit-project-button.png)
![Edit project](./assets/img/edit-project.png)

#### Making a project publicly accessible

Navigate to the edition page for the project. Hit the "Make project public" to make the project and all the data it contains publicly accessible.

![Make project public](./assets/img/make-project-public.png)

#### Creating Resources

Navigate to the project where you want to create a resource. Click on the "Create Resource" button in the right sidebar. Build the JSON payload with the help of the interactive editor, then hit "Save".

![Create resource button](./assets/img/create-resource-button.png)
![Create resource](./assets/img/create-resource.png)
