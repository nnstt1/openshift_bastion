# openshift_bastion

このリポジトリは、ベアメタル環境にOpenShiftを構築する際の「踏み台サーバ(bastion)」を設定するための Ansible Playbook です。

## Prerequisites

* bastionサーバのOSは CentOS7

* Ansibleコントロールノードからbastionサーバにssh可能

## How to use

* `inventory` の `ansible_host` をbastionサーバのIPアドレスに変更

* `host_vars/bastion.yml` の各変数を変更

* `ansible-playbook -i inventory setup_bastion.yml`