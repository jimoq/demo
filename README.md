# demo
Demo of Check Point policy automated through Ansible and versioned in Git

## Run
Add the folllwing admin user to you test check point management server enviroment

username: api_user
password: vpn 123

And execute:

```ansible-pull -d /tmp/ansibel-pull -U https://github.com/jimoq/demo.git demo_playbook.yml -e "target=192.168.233.71" -i 192.168.233.71,```

Or clone the repository and execute:

```ansible-playbook demo_playbook.yml -e "target=192.168.233.71" -i 192.168.233.71,```

## References
* [sk114661 - Automate your management server using "Ansible"](https://supportcenter.checkpoint.com/supportcenter/portal?eventSubmit_doGoviewsolutiondetails=&solutionid=sk114661?tocpath=Posture%20Management%7CThe%20CloudGuard%20Dome9%20GSL%20Language%7C_____0)
* [Check Point Ansible collections](https://galaxy.ansible.com/check_point)
* [Check Point Ansible collection documentation](https://docs.ansible.com/ansible/latest/collections/check_point/mgmt/index.html#plugins-in-check-point-mgmt)
