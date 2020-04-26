# repo_template

The directory `gendoc` contains scripts neceesary for building website using sphinx and sphinx gallery.
The `.travis.yml` file contains the commands needed for travis-ci to deploy the website to GitHub pages.

The resulting template website can be seen here: https://anwarnunez.github.io/repo_template/

## Setup

Requires minor configuration

### Create GitHub access token

This enables travis to push and create the gh-pages branch.

github.com -> public profile -> developer settings -> personal access tokens -> generate new token

* Under **Note** write something descriptive (e.g. `myrepo-travis-ghpages`).
* Under  **Select scopes** select **repo**. 
* Finally, click on **Generate token** and copy the token.

### Add token to travis repo settings

travis-ci -> dashboard -> select repo -> settings

* Under **Environmental variables**, fill out:
  * *NAME*: `GITHUB_TOKEN`
  * *VALUE*: [paste the token]
* Finally, click **ADD**

