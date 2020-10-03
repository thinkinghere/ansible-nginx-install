# ansible-nginx-install

## 目录
```
├── ansible.cfg
├── files
│   ├── nginx
│   ├── nginx-1.18.0.tar.gz
│   ├── nginx.service
│   ├── nginx.service.bak
│   └── test.html
├── hosts
├── production
├── roles
│   ├── common
│   │   ├── tasks
│   │   └── vars
│   │       └── main.yml
│   └── nginx
│       ├── handlers
│       │   └── main.yml
│       ├── tasks
│       │   ├── basic-bak.yml
│       │   ├── basic.yml
│       │   ├── main.yml
│       │   └── nginx.yml
│       └── vars
│           └── main.yml
├── staging
├── templates
│   └── test.conf
└── webserver.yml
```
## 执行脚本

`ansible-playbook -i production webserver.yml`

## to do
- 增加systemctl daemon-reload
- 增加nginx 自定义配置文件