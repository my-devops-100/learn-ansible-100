# learn-ansible-100

|本期版本| 上期版本
|:---:|:---:
`Sun Jul 21 13:45:46 CST 2024` | -


```yaml
environment:
    https_proxy: http://192.168.56.1:7890
    http_proxy: http://192.168.56.1:7890
    all_proxy: socks5://192.168.56.1:7890
    
pre_tasks:
    - name: Mirror Aliyun.
      replace:
        path: /etc/apt/sources.list
        regexp: 'http://(archive|security).ubuntu.com'
        replace: http://mirrors.aliyun.com

    - name: Update apt cache if needed.
      apt: update_cache=yes cache_valid_time=3600
```


## Ref

* [https://www.ansible.com/](https://www.ansible.com/)
* [https://docs.ansible.com/](https://docs.ansible.com/)
* [https://galaxy.ansible.com/](https://galaxy.ansible.com/)
