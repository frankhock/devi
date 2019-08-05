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
- dev user with ssh access

## Setup

make sure ansible is installed on your machine `brew install ansible`

create `ansible/inventory` file - update config using `ansible/inventory.example` as reference

create `ansible/variables.yml` file - update variables using `ansible/variables.yml.example` as reference

run `cd ansible && ansible-playbook -i inventory -u root --private-key=$HOME/.ssh/id_rsa devi.yml`
