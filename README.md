# My Project zabbix_ansible

# issue
ansibleでzabbix構築を自動化し、grafana連携で可視化性を上げる

# enviloment
#php
PHP_VERSION_REMI: "http://rpms.famillecollet.com/enterprise/remi-release-7.rpm"
PHP_VERSION_EPEL: "epel-release"

#mysql
MYSQL_VERSION: "https://repo.mysql.com//mysql80-community-release-el7-10.noarch.rpm"

#wordpress
Wordpress_VERSION: "https://ja.wordpress.org/wordpress-6.4.3-ja.tar.gz"

#zabbix
Zabbix_VERSION: "https://repo.zabbix.com/zabbix/5.0/rhel/7/x86_64/zabbix-release-5.0-1.el7.noarch.rpm"

#grafana
Grafana_VERSION: "https://s3-us-west-2.amazonaws.com/grafana-releases/release/grafana-4.6.3-1.x86_64.rpm"

# 構文チェック
ansible-playbook servers.yml --syntax-check

# playbook実行
ansible-playbook servers.yml

### 実行ログ
```
PLAY RECAP **********************************************************************************************************************************************************************************************************************************
dev.menta.me               : ok=40   changed=8    unreachable=0    failed=0    skipped=3    rescued=0    ignored=0   
zabbix.menta.me            : ok=52   changed=7    unreachable=0    failed=0    skipped=5    rescued=0    ignored=0  
```


