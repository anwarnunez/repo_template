# repo_template

## Create access token

This enables travis to push and create the gh-pages branch.

github.com -> public profile -> developer settings -> personal access tokens -> generate new token

* Under **Note** write something descriptive (e.g. `myrepo-travis-ghpages`).
* Under  **Select scopes** select **repo**. 
* Finally, click on **Generate token** and copy the token.

## Add token under travis repo settings

travis-ci -> dashboard -> select repo -> settings

* Under **Environmental variables**, fill out:
  * *NAME*: `GITHUB_TOKEN`
  * *VALUE*: [paste the token]
* Finally, click **ADD**

