# Bartholomew Site Template

This repository is a template for creating new [Bartholomew](https://github.com/technosophos/bartholomew) websites.

## Directory Structure:

- `config/site.toml`: The main configuration file for your site. You should edit this.
- `content/`: Your markdown files go in here.
- `modules.toml`: The configuration file for your Wagi server. You may need to adjust a few paths.
- `scripts/` (advanced): If you want to write your owh Rhai scripts, they go here.
- `static/`: Static assets like images, CSS, and downloads go in here.
- `templates/`: Your handlebars templates go here. 

## Installation of Wagi, Bartholomew, and the fileserver

To use Bartholomew, you will need to install [Wagi](https://github.com/deislabs/wagi).
Once you have Wagi installed, you can continue setting up Bartholomew.

If you haven't already, you will need to download a copy of `bartholomew.wasm`.
You can get this from the [Bartholomew GitHub repo](https://github.com/technosophos/bartholomew).
You will also need the [Wagi Fileserver](https://github.com/deislabs/wagi-fileserver).

Once you have copies of `bartholomew.wasm` and `fileserver.gr.wasm`, you can do one of two things:

1. Put both modules in this directory
2. OR Modify `modules.toml` to point to the full path of `bartholomew.wasm` and `fileserver.gr.wasm`

To start Bartholomew, run the following command from this directory:

```console
$ wagi -c modules.toml
No log_dir specified, using temporary directory /var/folders/rk/mkbs8vx12zs0gkm680h_gth00000gn/T/.tmpvkGeXG for logs
Ready: serving on 127.0.0.1:3000
```

Now you can point your web browswer to `http://127.0.0.1:3000/` and see your new Bartholomew site.

## About the License

This repository uses CC0. To the greatest extent possible, you are free to use this content however you want.
You may relicense the code in this repository to your own satisfaction, including proprietary licenses.