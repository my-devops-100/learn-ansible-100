# Aliyun

* <https://developer.aliyun.com/mirror/ubuntu?spm=a2c6h.13651102.0.0.3e221b11Ff7Gcs>
* <https://developer.aliyun.com/article/767805>

> clash rules

```
DOMAIN,mirrors.cloud.aliyuncs.com,DIRECT
```


```yaml
 pre_tasks:
    - name: Mirror Aliyun.
      replace:
        path: /etc/apt/sources.list
        regexp: 'http://(archive|security).ubuntu.com'
        replace: http://mirrors.aliyun.com
        
```