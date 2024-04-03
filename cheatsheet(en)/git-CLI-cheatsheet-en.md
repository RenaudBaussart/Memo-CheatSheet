### <a id=auth></a>**Authentication**

- `gh auth login`: Log in to a GitHub account
- `gh auth logout`: Log out of a GitHub account

### <a id=depo></a>**Repository Management**

- ```gh repo create [<name>] [flags]```: Create a repository

    Options | Description 
    --- | --- 
    `-p`, ` --template <repository>` | Base the repository on a template
    `-t`, ` --team <name>` | Allow access to a group or organization
    `-c`, ` --clone` | Clone the repository into the current directory
<br>

- `gh repo fork [<repository>] [flags]`: Fork a repository
- `gh repo clone <repository> [<directory>]`: Clone a repository
- `gh repo view [<repository>] [flags]`: View a repository

    Options | Description 
    --- | --- 
    `-b`, ` --branch <string>` | View a branch of the repository
    `-w`, ` --web` | Open a repository in the web browser
<br>

### <a id=issues></a>**Issue Management**

- `gh issue create [flags]`: Create an issue

    Options | Description 
    --- | --- 
    `-t`, ` --title <string>` | Provide a title
    `-l`, ` --label <name>` | Add a label by name
    `-a`, ` --assignee <login>` | Assign someone by their login. Use "@me" to assign it to yourself
<br>

- `gh issue list [flags]`: List issues

    Options | Description 
    --- | --- 
    `-a`, ` --assignee <string>` | Filter by assigned person
    `-A`, ` --author <string>` | Filter by author
    `-s`, ` --state <string> (default "open")` | Filter by status: {open\|closed\|all}
    `-l`, ` --label <strings>` | Filter by label
<br>

- `gh issue status`: Show the status of issues that concern you
- `gh issue view {<number> | <url>} [flags]`: View a specific issue

    Options | Description 
    --- | --- 
    `-c`, ` --comments` | View comments of an issue
<br>

- `gh issue close {<number> | <url>} [flags]`: Close an issue

    Options | Description 
    --- | --- 
    `-c`, ` --comment <string>` | Leave a closing comment
    `-r`, ` --reason <string>` | Reason for closure
<br>

- `gh issue reopen {<number> | <url>} [flags]`: Reopen an issue

    Options | Description 
    --- | --- 
    `-c`, ` --comment <string>` | Leave a reopening comment
<br>

### <a id=pr></a>**Pull Request Management**

- `gh pr create [flags]`: Create a pull request

    Options | Description 
    --- | --- 
    `-B`, ` --base <branch>` | The branch you want to merge your code into
    `-f`, ` --fill` | Use commit info for title and body
    `-l`, ` --label <name>` | Add a label by name
<br>

- ```gh pr list [flags]```: List pull requests

    Options | Description 
    --- | --- 
    `-a`, ` --assignee <string>` | Filter by assigned person
    `-A`, ` --author <string>` | Filter by author
    `-s`, ` --state <string> (default "open")` | Filter by status: {open\|closed\|merged\|all}
    `-l`, ` --label <strings>` | Filter by label
<br>

- `gh pr status`: Show the status of pull requests that concern you
- `gh pr view {<number> | <url> | <branch>} [flags]`: View a specific pull request

    Options | Description 
    --- | --- 
    `-c`, ` --comments` | View comments of a pull request
<br>

- ```gh pr checkout {<number> | <url> | <branch>}```: View details of a pull request
- ```gh pr merge {<number> | <url> | <branch>}```: Merge a pull request
- ```gh pr diff {<number> | <url> | <branch>} [flags]```: View changes in a pull request
- ```gh pr close {<number> | <url> | <branch>} [flags]```: Close a pull request

    Options | Description 
    --- | --- 
    `-c`, ` --comment <string>` | Leave a closing comment
    `-d`, ` --delete-branch` | Delete the local and remote branch after closing
<br>

- `gh pr reopen {<number> | <url> | <branch>} [flags]`: Reopen a pull request

    Options | Description 
    --- | --- 
    `-c`, ` --comment <string>` | Leave a reopening comment
<br>

### <a id=workflows></a>**Workflow Management**

- `gh workflow list [flags]`: List workflow files, hiding disabled by default

    Options | Description 
    --- | --- 
    `-a`, ` --all` | Include disabled workflows

- `gh workflow view [<workflow-id> | <workflow-name> | <filename>] [flags]`: View a summary of a workflow
- `gh workflow run [<workflow-id> | <workflow-name>]`: Execute a workflow
- `gh workflow enable [<workflow-id> | <workflow-name>]`: Enable a workflow, allowing it to be executed
- `gh workflow disable [<workflow-id> | <workflow-name>]`: Disable a workflow, preventing it from being executed
<br>