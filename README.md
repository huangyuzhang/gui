# Gui.sh
A Shell-based Ghost Static Generator

## Install
1. Have your local Ghost website ready first.

2. Install `wget`. For MacOS, simply run `brew install wget`.

3. Save `gui.sh` file in the root directory of your local Ghost website. Modify the `# Define urls and https` section as follows:

    ```bash
    # Define urls and https
    from_url=http://localhost:2368 # change this if your local ghost url is different
    to_url=yourdomain.com # change it to your real domain name
    to_https=true # set true to enable HTTPS (e.g. GitHub Pages)
    ```

4. Give execution permission to it:
    ```bash
    chmod +x gui.sh
    ```

5. Run it:
    ```bash
    ./gui.sh
    ```
6. Then go to `static` folder:
    ```bash
    cd static
    ```
7. Initiate a new git repo, commit everything here and push to your new GitHub repo:
    ```bash
    git init
    git add .
    git commit "Initial Commit"
    git remote add origin git@github.com:<your_user_name>/<repo_name>.git
    git push -u origin master
    ```
8. Enable GitHub Pages in settings.