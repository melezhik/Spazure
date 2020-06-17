# Spazure

Automation toolset for Azure DevOps written on Sparrow


# Getting started

    zef install --/test Sparrow6
    
    export SP6_REPO=http://repo.westus.cloudapp.azure.com
    
    s6 --search ado

    s6 --install ado-git-branch-create

    s6 --plg-run ado-git-branch-create@project=Backends,repo=Catalog,branch=feature
    

# See also

Ado related Sparrow plugins - http://repo.westus.cloudapp.azure.com/hub/search?q=ado

Sparrow plugins source code - https://github.com/melezhik/sparrow-plugins

Sparrow project - https://github.com/melezhik/Sparrow6
