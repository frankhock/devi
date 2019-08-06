Automate your remote dev env

## What you get

- zsh
- oh-my-zsh
- spaceship-prompt (zsh theme)
- zsh syntax highlighting
- zsh auto suggestions
- tmux
- SpaceVim
- nvm
- rbenv
- awscli
- htop
- dev user with ssh access
- disabled root login

## Setup

make sure ansible is installed on your machine `brew install ansible`

create `ansible/inventory` file - update config using `ansible/inventory.example` as reference

create `ansible/variables.yml` file - update variables using `ansible/variables.yml.example` as reference

install dependencies - from the `ansible` directory run `ansible-galaxy install -r requirements.yml`

run playbook - from the `ansible` directory run `ansible-playbook -i inventory -u root --private-key=$HOME/.ssh/id_rsa devi.yml`
