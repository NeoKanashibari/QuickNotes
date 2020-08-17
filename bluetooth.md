# Swith bettween HSP/HFP and A2DP

```sh
vim /etc/pulse/default.pa
# edit line
ad-module module-bluetooth-policy
ad-module module-bluetooth-policy auto_swith=2
```
