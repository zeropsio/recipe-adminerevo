# Zerops x AdminerEvo
The concept of a utility tool illustrates how to set up and use the technologies supported by [Zerops](https://zerops.io).

<br />

![adminerevo](https://github.com/zeropsio/recipe-shared-assets/blob/main/covers/cover-adminerevo.png)

## Deploy on Zerops
You can add the latest version of Adminer to your project by clicking the ```Import Services``` button in the project details and then copying the provided code.


```yaml
services:
  - hostname: adminerevo
    type: php-apache@8.3
    enableSubdomainAccess: true
    buildFromGit: https://github.com/zeropsio/recipe-adminerevo
```
See the [Zerops documentation](https://docs.zerops.io/references/import) and [zerops.yaml](https://github.com/zeropsio/recipe-adminer/blob/main/zerops.yml) to understand how to use it.



<br/>
<br/>

## ADMINER

[AdminerEvo](https://github.com/adminerevo/adminerevo) is a web-based database management interface, with a focus on security, user experience, performance, functionality and size.
It works out of the box with MySQL, MariaDB, PostgreSQL, SQLite, MS SQL, Oracle, Elasticsearch and MongoDB. In addition, there are plugins for SimpleDB, Firebird and ClickHouse.

AdminerEvo is developed by the AdminerEvo community and is a continuation of the Adminer project by Jakub Vrána.


## Production vs. development

- For production environments, it is not advisable to make Adminer publicly accessible. Consider either disabling ```Public Access through the Zerops.io subdomain```  after deployment in GUI  or directly setting `enableSubdomainAccess` to `false` in import file.
- To access Adminer in production environment you can use a  [VPN](https://docs.zerops.io/references/vpn) through [ZCLI](https://docs.zerops.io/references/cli). Once connected, Adminer will be available at the address `adminer.zerops` (or whatever hostname you set).

<br/>
<br/>

Need help setting your project up? Join [Zerops Discord community](https://discord.com/invite/WDvCZ54).