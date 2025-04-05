# GitHub-README-Keyword-Search

**Recruiters, HR managers, and talent acquisition specialists** often need to quickly assess a developer's skills by searching their GitHub READMEs for relevant keywords, a process hindered by manual searching or complex GitHub search syntax. This micro-app simplifies the search by allowing them to enter a GitHub username and keyword to instantly find relevant repositories.

## Usage
**Download** the `index.html` file. You have two main options:
1.  * **Downloading as a ZIP file (easier for most users):**
        * Look for a **green button** labeled "**Code**" on this page - it is in the top section. Click on it.
        * In the dropdown menu, select "**Download ZIP**".
        * Once the ZIP file is downloaded, extract its contents. You will find the `index.html` file inside.
    
    * **Using Git (if you have it installed):** Open your command prompt or terminal and type:
        ```bash
        git clone https://github.com/lzrdGreen/GitHub-README-Keyword-Search.git
        ```
        This will create a folder named `GitHub-README-Keyword-Search` containing the `index.html` file.

2.  **Obtain a personal GitHub access token:** This is needed for the app to securely access GitHub's API. Here's how:
    * Click on your **profile picture** in the top right corner of the GitHub website.
    * Click on "**Settings**" (usually near the bottom of the dropdown menu, next to a cogwheel icon).
    * In the left sidebar, scroll down and find "**Developer settings**". Click on it.
    * Click on "**Personal access tokens**".
    * Click on "**Fine-grained tokens**".
    * Next to "**Fine-grained personal access tokens**", click the button "**Generate new token**". Follow the steps.
    * **Copy the generated token** immediately and store it somewhere safe. You won't be able to see it again.

3.  **Open** the `index.html` file in a simple text editor (like Notepad on Windows, TextEdit on Mac, VS Code, Sublime Text, etc.).

4.  **Locate the line of code where the GitHub token needs to be inserted.** This is typically around line **50 or 51** and looks like this:
    ```javascript
    const GITHUB_TOKEN = "secret_token";
    ```

5.  **Carefully replace the `"secret_token"` part with the personal access token you copied in step 2.** Make sure to keep the quotation marks (`"`) before and after your token. For example:
    ```javascript
    const GITHUB_TOKEN = "YOUR_GENERATED_GITHUB_TOKEN";
    ```
    You can use **Ctrl+V** (on Windows) or **Cmd+V** (on Mac) to paste the token.

6.  **Save** the modified `index.html` file.

7.  **Open** the saved `index.html` file in your web browser (double-click the file). Enter a GitHub username and a keyword to start your search!

**Important!**
**Security:** Treat your GitHub token like a password and do not share it publicly.