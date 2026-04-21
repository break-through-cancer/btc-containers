# btc-containers
Containers to be used in modules that the tool/module authors did not provide a container for.

## how to
A github action accompanies this repo to build and push container images to [btc-registry](https://github.com/orgs/break-through-cancer/packages).
To make a container appear in the btc-registry:
* create a folder in the root of this repo, name it after the desired image name;
* add image/folder path to the [workflow triggers and changed-container filters](https://github.com/break-through-cancer/btc-containers/blob/main/.github/workflows/build-push-container.yml)
* merge to main  
