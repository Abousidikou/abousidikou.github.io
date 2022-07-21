# READMe

# Install jekyll

```bash
sudo apt-get install ruby-full build-essential zlib1g-dev
```

Évitez d'installer les packages RubyGems (appelés gems) en tant qu'utilisateur root. Au lieu de cela, configurez un répertoire d'installation de gem pour votre compte d'utilisateur. Les commandes suivantes ajouteront des variables d'environnement à votre fichier ~/.bashrc pour configurer le chemin d'installation du gem :

```bash
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```


Install jekyll
```bash
gem install jekyll bundler
```

To verify 
```bash
jekyll -v
```

# Clonage
```bash
git clone https://github.com/Abousidikou/abousidikou.github.io
```
# Entrer dans le repertoire
```bash
cd abousidikou.github.io
```

# Config email
```bash
git condig user.email 'votre email'
```

# Create files
Creer un fichier par article dans `_posts` avec le format  `annee-mois-jour-titre.md`
Ajouter le 'front-matter'
```bash
---
layout: post
title:  "Posts!!"
date:   2022-06-20 21:57:24 +0100
categories: index
permalink: /:categories/:year/:month
---
```

Le fichier peut être éditer en markown.

# Building and serving jekyll
```bash
bundle exec jekyll build
bundle exec jekyll serve
```

La page peut être vu avec l'addresse générée par jekyll serve. (Ex: 127.0.0.1:4000)

# Git pushing
```bash
git add .
git commit -m 'article ajouté'
git push
```

Attendre un moment puis aller sur [abousidikou.github.io](https://abousidikou.github.io)
