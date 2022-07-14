# Hello, Welcome to Ansible
![](https://lh6.googleusercontent.com/pvbQyYAnwP2p_Tffl3lgpANmTYuq1KSsKCELRaD7-G6S9rqfVVaDGtIr3Eqwua6vNkgXPG5cndomB9Qz_YuD41KvVlQ8LBJGF0vnm1efUZaGUJljqmAK5-UgpA_ratMtCOC4SAUXSShkB72S05I)

## What is Ansible?
It is a modern automation tool for deployment, software provisioning(setting up IT infrastructure), configuration management, application development tool provides infrastructure as code and automating the tasks. It is an agentless application i.e. we just need to install it on a host machine and then we can use it on any worker machine without installing it on those worker machines.

## Why Ansible?
Because it is more stable and has a lot of configurations using ansible-playbooks in the deployment.
It is one of the top choices to deploy OpenStack. OpenStack-Ansible deploys a production-capable OpenStack environment using Ansible and LXC(linux containers) containers. This approach isolates the various OpenStack services into their own containers and makes it easier to install and update OpenStack.

## What are Ansible Playbooks?
It is a set of tasks that automatically execute against hosts.
Ansible Playbooks offer a repeatable, re-usable, simple configuration management and multi-machine deployment system, one that is well suited to deploying complex applications. If you need to execute a task with Ansible more than once, write a playbook and put it under source control. See how easy it is.

## Playbooks Syntax:
Playbooks are expressed in YAML format with a minimum of syntax.A playbook is composed of one or more ‘plays’ in an ordered list. The terms ‘playbook’ and ‘play’ are sports analogies. Each play executes part of the overall goal of the playbook, running one or more tasks. Each task calls an Ansible module.

## Playbooks Execution:

A playbook runs in order from top to bottom. Within each play, tasks also run in order from top to bottom. Playbooks with multiple ‘plays’ can orchestrate multi-machine deployments, running one play on your web servers, then another play on your database servers, then a third play on your network infrastructure, and so on. At a minimum, each play defines two things:

-   the managed nodes to target, using a pattern
-   at least one task to execute

## Task Execution:
By default, Ansible executes each task in order, one at a time, against all machines matched by the host pattern. Each task executes a module with specific arguments. When a task has been executed on all target machines, Ansible moves on to the next task. You can use strategies to change this default behaviour. Within each play, Ansible applies the same task directives to all hosts. If a task fails on a host, Ansible takes that host out of the rotation for the rest of the playbook.

# Running Playbooks:

Using the cmd : ansible-playbook <playbook_name.yaml>
