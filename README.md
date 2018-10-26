# snap-zotero
Build instructions to create a snap package for zotero (https://www.zotero.org/)


## Usage

This repo contains the snapcraft.yml file to build a snap package for a prebuilt zotero release which you can download from https://www.zotero.org/ .
Extract the downloaded archive into the root of this repo. Afterwards, simply run

    snapcraft
    
which will generate *zotero_0.1_amd64.snap*. This can afterwards be installed

    sudo snap install zotero_0.1_amd64.snap --devmode --dangerous
    
### Comparison to standard installation (extracting and running binaries directly)

- user data usually are stored in ~/Zotero . The snap will put its data into the directory ~/snap/zotero/current/Zotero/
