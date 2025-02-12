# btc-containers
Containers to be used in modules that the tool/module authors did not provide a container for.

## how to
A github action accompanies this repo to build and push container images to [btc-registry](https://github.com/orgs/break-through-cancer/packages).
To make a container appear in the btc-registry:
* create a folder in the root of this repo, name it after the desired image name
* add image/folder name to the [Actions matrix](https://github.com/break-through-cancer/btc-containers/blob/e6477b1b3594f7bf3df0f1688ba3b206379abb70/.github/workflows/build-push-container.yml#L20)
* merge to main  
