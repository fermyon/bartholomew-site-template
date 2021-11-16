# Bartholomew Site Template

This repository is a template for creating new [Bartholomew](https://github.com/technosophos/bartholomew) websites.

## Directory Structure:

- `config/site.toml`: The main configuration file for your site. You should edit this.
- `content/`: Your markdown files go in here.
- `modules.toml`: The configuration file for your Wagi server. You may need to adjust a few paths.
- `scripts/` (advanced): If you want to write your owh Rhai scripts, they go here.
- `static/`: Static assets like images, CSS, and downloads go in here.
- `templates/`: Your handlebars templates go here. 

## Installing Bartholomew

If you haven't already, you will need to download a copy of `bartholomew.wasm`.
You can get this from the [Bartholomew GitHub repo](https://github.com/technosophos/bartholomew).

Once you have downloaded it, you can either:

1. Put it in this directory
2. OR Modify `modules.toml` to point to the full path of `bartholomew.wasm`

## Serving Static Files

To serve static files, your `modules.toml` will need to point to an instance of the [Wagi Fileserver](https://github.com/deislabs/wagi-fileserver). You can download a copy of the fileserver from the [releases page](https://github.com/deislabs/wagi-fileserver/releases).

Once you have downloaded it, you can either:

1. Put it in this directory
2. OR Modify `modules.toml` to point to the full path of `fileserver.gr.wasm`

## About the License

This repository uses CC0. To the greatest extent possible, you are free to use this content however you want.
You may relicense the code in this repository to your own satisfaction, including proprietary licenses.