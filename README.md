# Ansible: Visualization

> This repo explains how to visualize your Ansible playbook.  
>
> Graphviz will draw an SVG picture for you by reading a .dot file ansible-playbook-grapher will create by examining your playbook.  
>
> If you want to build your own map manually, it's worth using the [VSCode MarkMap](https://markmap.js.org/) plugin.

## Usage  
Run this command to visualize your playbook:
```shell
ansible-playbook-grapher -i your-inventory-file --include-role-tasks your-playbook.yml
```
## Installation  
### Prerequisites
Follow [Ansible Playbook Grapher](https://github.com/haidaraM/ansible-playbook-grapher) for details. 
### Graphviz  
```shell
sudo apt-get install graphviz # or yum install or brew install (MacOS)
```
### ansible-playbook-grapher
```shell
pip install ansible-playbook-grapher
```
## Acknowledgments

This repo was inspired by [Ansible Playbook Grapher](https://github.com/haidaraM/ansible-playbook-grapher), and [VSCode MarkMap](https://markmap.js.org/).

## See Also
- [GitHub: Ansible playbook graph](https://github.com/haidaraM/ansible-playbook-grapher)
- [Blog: Visualizing Ansible Plays and Tasks](https://blog.networktocode.com/post/visualizing-ansible-plays-and-tasks/)
- [GitHub: Ansible inventory graph](https://github.com/willthames/ansible-inventory-grapher)
- [Blog: generate a diagram of your Ansible inventory](https://univers-libre.net/posts/ansible-infrastructure-diagram.html)
- [VSCode MarkMap](https://markmap.js.org/)
- [VSCode Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)

## License
Follow all involved parties licenses terms and conditions.