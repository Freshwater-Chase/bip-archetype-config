# BIP Service Configuration Repository Archetype
This repository serves as an archetype from which to create new service team configuration repositories.

## Generating a Configuration Repository for a New Project
Update the values in the gen.properties file and run gen.sh to create the configuration for your new project. 
Look at the [Generating a New Project](https://github.com/department-of-veterans-affairs/bip-archetype-service#generating-a-new-project) 
documentation for more details.

## Instructions on setting up branch permissions
After creating the service team's configuration repository, follow these steps to apply branch permissions to the master branch:
1. Open your browser to your GitHub repository URL.
1. Navigate to `Settings` > `Branches`
1. Under the `Branch protection rules` section, click the `Add rule` button.
1. Set the `Branch name pattern` field's value to `master`
1. Select the following rule settings:
    * Require pull request reviews before merging
        * Required approvingg reviews: 1
        * Dismiss stale pull request approvals when new commits are pushed
    * Include administrators
    * Restrict who can push to matching branches
        * Add the `BIP ProdOps` team.
1. Click the `Create` button