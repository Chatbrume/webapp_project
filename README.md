# webapp_project

Pour cette exercice j'ai utiliser la platforme [eazytraining](https://docker.labs.eazytraining.fr/)
Login: devops
Password: devops

## Création machine virtuelle

## Installation sur master
Se connecter en temps qu'admin:
`sudo su admin`

Quitter le dossier root:
`cd`

Recupere le dépôts git:
`git clone https://github.com/Chatbrume/webapp_project.git`

Allez dans le dossier
`cd webapp_project`

Charger le role:
`ansible-galaxy install chatbrume.webapp_role`

Installer sur le client:
```cwd
ansible-playbook -i host.yml admin.yml
BECOME password: admin
```

## Resultat sur client
open port 8080
