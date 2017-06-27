# Bash on Windows

Configuration made easy with Ansible

## Reset

At any time if you have messed up you can reset everything to factory defaults like so:

    lxrun /uninstall /full /y
    lxrun /install

Important notice: all files will be deleted

## Setup

After very first run you need to install ansible itself

    sudo apt-get install -y software-properties-common
    sudo apt-add-repository -y ppa:ansible/ansible
    sudo apt-get update
    sudo apt-get install -y ansible

## Run

To apply configuration just run

    ansible-playbook playbook.yml -i inventory

## TODO

- python 2 vs 3 with pyenv
- bashrc change PS1
- vim config
- tmux config
- `echo “set bell-style none” >> .inputrc`