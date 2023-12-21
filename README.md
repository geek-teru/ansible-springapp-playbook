### 利用手順
```

# Syntax check
ansible-playbook -i inventories/docker-local/hosts main.yml --syntax-check

# 疎通確認
ansible -i inventories/docker-local/hosts -u infra all -m ping -vvvv

# 差分確認
ansible-playbook -i inventories/docker-local/hosts main.yml --check --diff

# 適用
ansible-playbook -i inventories/docker-local/hosts main.yml --diff
```