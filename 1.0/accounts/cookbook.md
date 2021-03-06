# Cookbook

[[toc]]

## Resetting Two Factor Authentication

If you have configured 2FA on your account and lose access to your secure token, you will need to email [forge@laravel.com](mailto:forge@laravel.com) to reset it.

## Forge Is Unable To Access Git Repository

There are several reasons Forge may not be able to access your GitHub / Bitbucket repository. First, you should try refreshing the source control API token that is linked to Forge via your account profile's "Source Control" tab.

Forge attempts to access your repository using your source control provider's API. The API credentials that will be used are the credentials tied to the account of the person who **owns** the Forge server. Note that if the Forge server is shared with you via a circle, it will use the circle **owner's** API credentials. You should ensure this person has full access to the repository on GitHub.

### GitHub Organization Repositories

Sometimes, if the repository is an organization repository, you will need to grant Forge access to that organization. You may do that using the following link: [https://github.com/settings/connections/applications/fdb28071bd05daebc122](https://github.com/settings/connections/applications/fdb28071bd05daebc122)
