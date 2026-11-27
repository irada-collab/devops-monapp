
# DevOps MonApp

## 1. Présentation du projet

DevOps MonApp est un projet réalisé dans le cadre du module DevOps.
Il a pour objectif de mettre en pratique les outils et les méthodes
de gestion de versions, de collaboration et d'intégration continue.


## 2. Membres de l'équipe et rôles

| Nom et prénom | Rôle |
|---|---|
| Irada Ben Amor | M1 - Git/GitHub et chef de projet |
| Tesnime Azzem | M2 - Application, Dockerfile et performance de build |
| Yasmine Ben Alaya | M3 - Jenkins et les 3 pipelines |
| Chaima Bellalh | M4 - Smoke tests, artefacts, démo et rapport |

## 3. Organisation des branches

- main : branche principale et stable.
- dev : branche de développement.
- feature/* : branches dédiées aux nouvelles fonctionnalités.

Workflow :

main ← dev ← feature/*

Les fonctionnalités sont développées dans des branches feature,
puis intégrées dans dev par Pull Request.
La branche dev est ensuite fusionnée dans main après validation.

## 4. Installation et lancement

### Cloner le dépôt

```bash
git clone https://github.com/irada-collab/devops-monapp.git
cd devops-monapp
```

### Construire l'image Docker

```bash
docker build -t devops-monapp .
```

### Lancer le conteneur Docker

```bash
docker run -d --name devops-monapp -p 8080:80 devops-monapp
```

## 5. Technologies utilisées

- Git et GitHub
- Docker
- Jenkins
