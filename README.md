# 使用 Ansible 安装 Kubernetes 集群

* 克隆此项目
* 创建多个 CentOS 7 服务器，可以以一台作为主控节点，而其他作为工作节点
* 编辑 `hosts` 文件中的 IP 地址
* 运行下列命行，分别完成 Kubernetes 主控制节点和工作节点的安装

```
ansible-playbook setup_master_node.yml
ansible-playbook setup_worker_nodes.yml
```

* 工作节点加入集群后，可使用以下命令查看其状态：
```
kubectl get nodes
```

## 参考文献:
* https://medium.com/faun/how-to-create-your-own-kubernetes-cluster-using-ansible-7c6b5c031a5d



