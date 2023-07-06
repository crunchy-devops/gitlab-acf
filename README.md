# Git et Gitlab 

## Pre-requis
Votre git bash est installe  
Dans la zone window de rechercher en bas a gauche de votre ecran entrez git bash 

## Gestion des directories sous Windows Git bash
Faire un ```pwd```  
Faire un ```cd c:```
Creez un projet sous C:  nomme projects    
Faire ```mkdir projects```  
faire ```ls -alrt```  
faire un ```cd projects```  
ouvrir votre navigateur et download le lien esrf  

et placer votre zip in c: projects

## Premiere commande GIT
faire un ```cd esrf```
faire ```git init```    
et un ```ls -alrt```

## Commande git porcelaine 
faire ```git status```  

## Mettre le fichier dans la staging area
faire ```git add .```      
verifier ```git status```   

## Se referencer aupres de git 
```shell
git config --global user.name "Votre nom "
git config --global user.email "votre email adresse"
```

## Mettre le fichier dans le local repository
faire ```git commit -m "first init```     
verifier ```git status```

## les 3 versions du fichier main.py
entrer ```echo "var = 1" > main.py ```    
```cat main.py```  
```git status```  
```git add main.py```  
```git status```  
```git commit -m"main.py version1```    
```git log --oneline```  
ajouter une autre ligne dans le fichier main.py   
entrer ```echo "var = 2" >> main.py ```   
```cat main.py```  
```git status```  
```git add main.py```  
ajouter une troisieme ligne   
entrer ```echo "var = 3" >> main.py ```     
```cat main.py```  
```git status```


## retrouver les differences entre les versions
### difference entre le local repo et la staging area

```git diff --cached```   

### difference entre la zone de travail et la staging area
``` git diff --color```  

### commit des 3 versions
```shell
git commit -m "main.py version2"
git diff --cached
git diff --color
git status
git add main.py
git diff --color
git status
git diff --cached
git commit -m"main.py version3"
git log --oneline
```

### voir le contenu des commits
```shell
git show HEAD
git show HEAD~1


```
### Differences entre 2 commits
```
git diff HEAD..HEAD~2
```

## Deplacement de HEAD 
```shell
git log --oneline --all
cat main.py
git checkout 9afa88f
git log --oneline  --all 




