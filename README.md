# Comment j'ai fait

Commandes exécutés:

```sh
ssh-keygen -t rsa -b 4096 -f ./ssh-terra

terraform init

terraform fmt

terraform validate

terraform plan

terraform apply

ansible all -i hosts -m ping --private-key ssh-terra

ansible-playbook -i hosts install.yml --syntax-check

ansible-playbook -i hosts install.yml --check

ansible-playbook -i hosts install.yml --private-key ssh-terra
```

Ne pas oublier d'ajouter les accès IAM dans l'environnement
