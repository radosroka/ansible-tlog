# tlog-ansible-setup
Ansible playbook for tlog.

1. Set proper variables in hosts and tlog-setup-test.yml.
2. Set ssh certificate for tlog machine(for ansible).

3. Run:

```{r, engine='bash', count_lines}
ansible-playbook -i hosts -u root tlog-setup-test.yml
```
Works with RHEL7.4 and Centos7.

It is important to check rsyslog version on Centos. There is new rsyslog v8 in RHEL but it doesn't have to be included in Centos now (10.7.2017).
