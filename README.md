# learn-ansible-100

|本期版本| 上期版本
|:---:|:---:
`Mon Jul 29 15:46:31 CST 2024` | -


### [Interpreter Discovery](https://docs.ansible.com/ansible-core/2.17/reference_appendices/interpreter_discovery.html)


> `ansible.cfg`

```
interpreter_python = /usr/bin/python3.10
```

> `host.ini`

```
192.168.30.5 ansible_user=root ansible_python_interpreter=/usr/bin/python3.10
```

> ~~`playbook.yml`~~

```
vars:
    ansible_python_interpreter: /usr/bin/python3.10
```    


## Ref

* [https://www.ansible.com/](https://www.ansible.com/)
* [https://docs.ansible.com/](https://docs.ansible.com/)
* [https://galaxy.ansible.com/](https://galaxy.ansible.com/)
