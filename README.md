Getting Started
---------------

**1. Install Repo**

Create bin dir to add to PATH:

    $ mkdir -p ~/.bin

Download the Repo script:

    $ curl http://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/.bin/repo

Make it executable:

    $ chmod +x ~/.bin/repo

Add ~/.bin to your PATH

    $ echo 'export PATH=$HOME/.bin:$PATH' >> ~/.bashrc
    $ source ~/.bashrc

**2. Initialize our project**

Create an empty directory:

    $ mkdir yocto
    $ cd yocto

To setup your repo initially:

    $ repo init -u https://github.com/angrydexterous/pi-demo.git


**3. Pull down the latest repos**

Updates all local repos to the branch you have selected:

    $ repo sync

**4. Initialize Yocto**

    $ export TEMPLATECONF=meta-codercamppi/conf
    $ source poky/oe-init-build-env
