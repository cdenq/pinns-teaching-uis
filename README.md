<!-- Back to top -->
<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="_">
    <img src="repo_assets/header.png" alt="Logo" width="250" height="100">
  </a>

  <h3 align="center">PINNs Teaching</h3>

  <p align="center">
    A companion GitHub repo to the research paper, pre-print draft <a href="">here</a> (link pending revision).
    <br>
    <br>
    <a href="https://github.com/cdenq/">GitHub Home</a>
    ·
    <a href="https://github.com/cdenq/pinns-teaching-uis/issues">Report Bug </a>
  </p>
</div>

<!-- Table of Contents -->
# Table of Contents
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#exe-sum">Executive Summary</a>
    </li>
    <li>
      <a href="#started">Getting Started</a>
      <ul>
        <li><a href="#started-setup">Setup</a></li>
        <li><a href="#started-directory">Directory</a></li>
      </ul>
    </li>
    <li>
      <a href="#ack">Acknowledgements</a>
    </li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ABOUT THE PROJECT -->
<a name="exe-sum"></a>
# Executive Summary

The following is the companion GitHub repo for our research paper "A Meshfree Deep Learning Approach for Numerical Solution of Differential Equations". This is provided as-is for math faculty, educators, and students alike to use in teaching PINNs, deep learning, and differential equations in their classroom settings. This repo is not intended to be "production-ready" or a "complete, self-guided tour", but rather, is a **supplemental resource in understanding our paper**.

<!-- ABOUT THE PROJECT -->
<a name="started"></a>
# Getting Started

<a name="started-setup"></a>
## Setup

Clone repo
```sh
git clone https://github.com/cdenq/pinns-teaching-uis
```

Setup virtual environments

(If `conda activate myenv` does not work, replace it with `source activate myenv`)

```sh
conda create --name harmonic-pinns
conda activate harmonic-pinns
conda install jupyter numpy matplotlib pytorch torchvision torchaudio -c pytorch

conda create --name burgers-pinns
conda activate burgers-pinns
conda install jupyter numpy matplotlib pandas paddlepaddle==2.6.0 --channel https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/Paddle/
conda install -c conda-forge deepxde
```

Locate the appropriate `.ipynb` file within the repo and then select the matching kernel before running.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<a name="started-directory"></a>
## Directory

```bash
fda-food-violation-score-predictor
├── burgers-example
│   └── burgers.ipynb               # code for the burgers example
├── harmonic-example
│   ├── pinns-plot                  # still images for the PINN.gif
│   │   └── *.png
│   ├── trad-plot                   # still images for the NN.gif
│   │   └── *.png
│   └── harmonic.ipynb              # code for the harmonic oscillation example
├── images                          # visual outputs from code
│   ├── *.png    
│   └── *.gif                        
├── repo_assets
│   └── header.jpg                  # the README's header image
├── .gitignore
├── LICENSE
├── README.md
├── requirements1.txt               # the required pip installations for the harmonic oscillation venv
└── requirements2.txt               # the required pip installations for the burgers venv
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGEMENTS -->
<a name="ack"></a>
# Acknowledgments
Special thanks to Ben Mosely for the original harmonic oscilation example and the team behind DeepXDE (Lu Lu et al) for the Burgers example. Full acknowledgements and citations are provided in the linked paper. 

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
<a name="contact"></a>
# Contact

To directly message me or setup a time to chat virtually, see my [contact page](https://github.com/cdenq#contact).

<p align="right">(<a href="#readme-top">back to top</a>)</p>