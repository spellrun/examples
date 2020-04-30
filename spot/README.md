# spot

This folder contains some resources on writing *reentrant* model training scripts. Training scripts with this property are perfect for performing long-running modle training jobs using spot instances (aka preemptible instances on GCP) and/or on-demand instances on GCP.

## Automating GPU machine failure recovery in Google Compute Engine

![](https://i.imgur.com/NYowq6j.png)

This blog post, ["Automating GPU machine failure recovery in Google Compute Engine"](https://spell.run/blog/automated-machine-failure-recovery-Xp3TEhEAACUAYwPM), discusses GPU host maintenance (aka the `REPAIRING` machine state) on GCP. The `reentrancy-demo.ipynb` Jupyter notebook contains some helpful code samples. You can launch this notebook by running the following CLI command (requires having the `spell` package installed):

```bash
spell jupyter \
    --lab \
    --github-url https://github.com/spellrun/spell-examples.git \
    spot-demo-workspace
```