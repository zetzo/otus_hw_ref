```
Host bastion
    HostName 51.250.91.111
    User appuser
    IdentityFile ~/.ssh/appuser

Host someinternalhost
    HostName 10.128.0.6
    User appuser
    ProxyJump bastion
```