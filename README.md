# kibana-proxy
解决社区版kibana无法使用ldap登录的问题
## 实现方式
截获kibana登录请求并强制转换到ldap验证，验证失败后走es内部账户，验证成功后将es内置用户密码更新

## 安装方式
[root@localhost ~]#sh -x install.sh 
