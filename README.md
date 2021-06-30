# GitHubAPI_PostmanCollection
GitHub has exposed a REST API that allows certain actions to be executed through various API calls. 
GitHub API Documentation: https://docs.github.com/en/rest/reference

This GitHub API collection can be loaded into Postman but for this to work, an environment should be created with the following variables:
- token: The personal access token created on GitHub (https://docs.github.com/en/github/authenticating-to-github/authenticating-with-saml-single-sign-on/authorizing-a-personal-access-token-for-use-with-saml-single-sign-on)
- repositoryName: Name of the repository
- owner: Username of the owner 
- organisation: Name of the organisation
- projectId: ID of the project
- projectName: Name of the project
- projectDescription: Description of the project
- user: Username of the user
- permission: Permission level (admin, write, read, none)
- cardId: ID of the card
- columnId: ID of the column
- cardName: Name of the card
- cardArchivedStatus: Boolean value of the card archived status
- moveColumnId: ID of the column that should be moved
- cardPosition: Position of the card in the column (top, bottom, or after:<card_id>)
- columnName: Name of the colummn
- columnPosition: Position of the column on the board (first, last, or after:<column_id>)
- teamName: Name of the team
- teamDescription: Description of the team
- parentTeamId: ID of the team at the level above the current team
- teamId: ID of the team
- teamSlug: String identifier of the team
- teamPrivacy: Privacy level of the team (secret, closed)
- childTeamPrivacy: Privacy level of the child team (closed)
- teamProjectPermission: Permission of the team to the project (read, write, admin)
- teamRepositoryPermission: Permission of the team to the repository (pull,push,admin,maintain,triage)

This collection covers the following actions and accommodates the following calls:
- Repositories
  - Organisation
    - Get Organisation Repositories
    - Create Organisation Repository (without linking to a team)
    - Create Organisation Repository (linking to a team)
    - Delete Organisation Repository
  - User
    - Create User Repository
    - Create Issue
    - Delete Repository
    - Get Deleted Repository
    - Get Repositories
- Projects
  - Organisation
    - Get Organisation Project
    - Get Organisation Projects
    - Create Organisation Project
    - Delete Organisation Project
  - User
    - Get User Projects
    - Create User Project
    - Delete User Project
  - Collaborators
    - Delete Project Collaborator
    - List Project Collaborators
    - Add Project Collaborator
    - Get Collaborator Permission
  - Cards
    - Get a Project Card
    - List Project Cards
    - Create a Project Card
    - Update a Project Card
    - Move a Project Card
    - Delete a Project Card
  - Columns
    - List Project Columns
    - Get a Project Column
    - Update a Project Column
    - Create a Project Column
    - Delete a Project Column
    - Move a Project Column
  - Create a Repository Project
  - List Repository Projects
- Teams
  - List Teams
  - Create a Team (Parent)
  - Delete a Team
  - Create a Team (Child)
  - Get a Team by Name
  - List Team Projects
  - Check Team Project Permissions
  - Check Team Permissions for a Repository
  - Add or Update Team Project Permissions
  - Add or Update Team Repository Permissions
  - Remove a Project from a Team
  - List Team Repositories
  - Remove a Repository from a Team
  - List Child Teams
  - Update a Team
- Get Rate Limit
