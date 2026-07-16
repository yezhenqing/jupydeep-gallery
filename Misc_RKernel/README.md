# JupyDeep RKernel Demo 🚀

JupyterLab is not restricted to Python alone. Architecturally, the Jupyter framework natively supports a wide variety of programming languages through language-specific kernel specifications and runtimes.

By extending this language-agnostic execution model to the Jupyter MCP capability, JupyDeep enables seamless multi-language workflows. Users can now harness the full power of JupyDeep for data science with unparalleled flexibility, efficiency, and intelligence across diverse runtime environments.

Here we demonstrate how to leverage this capability to run an R kernel in JupyterLab using JupyDeep.

To get started, we need to set up the appropriate environment. We will use [Pixi](https://pixi.prefix.dev/latest/) as our environment manager—please make sure it is installed on your system before proceeding. Afterward, you can clone this example repository - Misc_RKernel.

Next, navigate into the cloned directory and start the environment by running:

```bash
git clone https://github.com/yezhenqing/jupydeep-gallery.git
cd ./jupydeep-gallery/Misc_RKernel
pixi install
pixi run jupyter lab --ip=0.0.0.0
```

Once executed, you will have a ready-to-go JupyterLab environment with both the **R kernel** and **JupyDeep** pre-installed.
If you don't see Agents appear, please try refreshing the web page or restarting the Jupyter server.
Please refer to the [documentation](https://yezhenqing.github.io/jupydeep/en/notebooks/misc/rkernel.html) for details as well.