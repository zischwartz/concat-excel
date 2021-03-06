Concatenates `xlsm` files into one big `xlsm`

### Getting Started

First install [Docker](https://www.docker.com/docker-mac) if it's not installed.

Then download this repo and dump your `xlsm` files into this directory.

Next, navigate to this directory in the terminal and run:

```bash
# if you have npm installed
npm run notebook
```

or

```bash
# if you don't have npm installed
docker run -it --rm -p 8888:8888 -v $PWD:/home/jovyan/work jupyter/datascience-notebook
```

_Warning: this will take a while to download the docker image the first time you run it_

There will be some output, hopefully including `Copy/paste this URL into your browser when you connect for the first time, to login with a token:`

Do that, and then navigate to the [notebook](http://localhost:8888/notebooks/work/concat_excel.ipynb).

[Working with jupyter notebooks](https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Notebook%20Basics.html).
