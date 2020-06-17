# Spazure

Automation toolset for Azure DevOps written on Sparrow


# Getting started

    zef install --/test Sparrow6
    
    export SP6_REPO=http://repo.westus.cloudapp.azure.com
    
    s6 --search ado

    s6 --install ado-git-branch-create

    s6 --plg-run ado-git-branch-create@project=Backends,repo=Catalog,branch=feature
    
Or if you prefer Raku API:

```raku

task-run "create branch", "ado-git-branch-create", %(
    project => "Backends",
    repo => "Catalog",
    branch => "feature"
);

```

# Authentication

Create file named `~/.sparrow-azure-devops.sh`

```
token=$PAT
api=https://dev.azure.com/$organization
user=$api_user
```

Where:

* `user`

User to sign requests

* `token`

User personal access token (PAT)

* `api`

Azure DevOps API URL

# See also

Ado related Sparrow plugins - http://repo.westus.cloudapp.azure.com/hub/search?q=ado

Sparrow plugins source code - https://github.com/melezhik/sparrow-plugins

Sparrow project - https://github.com/melezhik/Sparrow6
