# demo
Demo of policy automated through ansible and versioned in Git

Execute on your ansible control node with the following command

watch -n 5 ansible-pull -o -d /tmp/playbooks-by-ansible-pull -U https://github.com/jimoq/demo.git demo_playbook.yml
