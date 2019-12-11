
# suricata规则测试

## 1. 测试环境

ubuntu16.04+[suricata](https://github.com/OISF/suricata)+[rules](https://rules.emergingthreats.net/open/suricata-4.0/rules/)

suricata安装教程 ➡️  - https://redmine.openinfosecfoundation.org/projects/suricata/wiki/Ubuntu_Installation

---

## 2. 测试步骤

### 2.1 测试指定流量+规则
```shell 
[root@localhost ~]# suricata -s wannamine.rules -r wannamine.pcap
```
![](https://ws2.sinaimg.cn/large/006tNc79gy1fzt6mbko3qj30to0a6myn.jpg)

---

### 2.2 查看fast.log日志
```shell 
[root@localhost ~]# tail -f fast.log
```
![](https://ws2.sinaimg.cn/large/006tNc79gy1fzt6moyzaaj32100o47mz.jpg)

---

## TODO
- [ ] 整理场景（classtype,tag）
- [ ] 环境准备pcap包对应msg


