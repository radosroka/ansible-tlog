# tlog-ansible-setup
Ansible playbook for tlog.

1. Set proper variables in hosts and tlog-setup-test.yml.
2. Set ssh certificate for tlog machine(for ansible).

3. Run:

```{r, engine='bash', count_lines}
ansible-playbook -i hosts -u root tlog-setup-test.yml
```
