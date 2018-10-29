# How to get started using Binder

Monday 29th October, 2018

Louise Bowler

## About Binder

On the 17th July 2018, I attended the [Build-a-Binder](https://build-a-binder.github.io/) workshop in Birmingham. Binder is an easy-to-use service that runs version-controlled computational environments, and it is particularly well-suited for use with Jupyter notebooks.

Clicking on a Binder link will take you straight to a fully interactive version of a project - this might be a notebook that contains the analysis presented in a paper, or a collection of notebooks used for teaching purposes. This approach sidesteps the need to clone the repo and install packages, which is ideal for sharing resources with those unfamiliar with git/GitHub, or who are short on time.

### This sounds great! Can I see some examples?

Sure! Here are some examples of notebooks associated with papers:
- Reproduction of _CheXNet: Radiologist-Level Pneumonia Detection on Chest X-Rays with Deep Learning_: [paper](https://arxiv.org/abs/1711.05225), [GitHub](https://github.com/jrzech/reproduce-chexnet)
- _Second-order variational equations for N-body simulations_: [paper](https://academic.oup.com/mnras/article/459/3/2275/2595117), [GitHub](https://github.com/hannorein/variations)

and here are some other applications of Binder:
- Notebooks containing examples and exercises for lecture courses: [Quantitative Big Imaging at ETH Zürich](https://github.com/kmader/Quantitative-Big-Imaging-2018)
- Interactive snippets in documentation: [spaCy](https://spacy.io/usage/linguistic-features)
- Demos and tutorials: [JupyterLab](https://github.com/jupyterlab/jupyterlab-demo), [Bokeh](https://bokeh.pydata.org/en/latest/docs/installation.html)

### What sort of projects are best suited for Binder?

Ideally, you will have a public git repository (if you need a hand with this, get in touch with me, Martin or Kirstie) that contains one or more Jupyter notebooks.

Data can either be stored in the repo (the best option for files <100Mb), or can otherwise be imported into the Binder after the container has been created (more on that later).

There are some practical limitations involved with [mybinder.org](https://mybinder.org) in terms of compute capabilities and storage, so it's best to avoid having to import, say, 500Mb of data. Instead, see if you can downsample or reduce the amount of data required so that you can run a smaller example on mybinder.org.

So if you have:
- A GitHub repo containing some Jupyter notebooks, and
- A small to medium amount of data...

you're good to go!

### Surely Binder must be really hard to set up?!

No, not at all!

If your repo already contains any data that you need to import, all you need to provide are the details of the packages needed to run the code in your notebooks.

You can do this through either a `requirements.txt` file (if you install packages with pip) or an `environment.yml` file (if you use conda). For instructions on how to generate these files, see these sites for [pip](https://pip.pypa.io/en/stable/user_guide/#requirements-files) or [conda](https://conda.io/docs/user-guide/tasks/manage-environments.html#sharing-an-environment).

Once you've generated and committed that file to your repo, copy the link to your repo and paste it into the appropriate box on [mybinder.org](https://mybinder.org). This should launch your project in Binder!

### What other things can I do in Binder?

You can:
- Link directly to a specific version of a notebook
- Add a Binder button to your GitHub repo
- Use a [postBuild](https://mybinder.readthedocs.io/en/latest/using.html#postbuild) file to:
  - Import data files from other sources
  - Reorganise content in the repo to direct the user to e.g. the demo files

For details on all these, and more, see the [Binder documentation pages](https://mybinder.readthedocs.io/en/latest/).
