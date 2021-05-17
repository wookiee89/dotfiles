<br />
<p align="center">

  <h3 align="center">Wookiee Dotfiles</h3>

  <p align="center">
    My dotfile repository for all my development environments.
    <br />
  </p>
</p>



<!-- ABOUT THE PROJECT -->
## About The Project

Currently, my main development environment is WSL2 w/ Ubuntu 18 (with other keys tools and services) on a Windows 10 desktop or laptop. The purpose of this repo is to help manage my dotfile configurations between by desktop and laptop. 

The secondary purpose of this repo is to show others how they can use [yadm](https://yadm.io/) (Yet Another Dotfile Manger) to help manage their dotfiles for accross various environments.
 
***Warning: I am by no means an expert in this subject. Both Google and Stackoverflow were my best friends when setting this up.***



<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

* **yadm** installed
* a git repo to store your dotfiles

If you do not have **yadm** already installed, then feel free to use their instructions found [here](https://yadm.io/docs/install#osx), or follow mine below.

I prefer to use [**asdf**](https://asdf-vm.com/#/core-manage-asdf) for managing these types of tools, and they luckily have a yadm plugin, so all you have to do is:

```sh

asdf plugin add yadm

asdf install yadm latest

```

Then I will add my repo for yadm to manage my dotfiles

```sh
# Clone repo

yadm clone git@github.com:wookiee89/dotfiles.git

```

## Usage

If you are doing this for the first time or if you are using an existing repository that holds your dotfiles and want to add new ones, then follow these steps:

```sh

# Add file
# yadm add ~/.bashrc

yadm add [dot file for yadm to manage]

yadm commit -a

yadm push

```