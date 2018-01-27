## 0. introduction du rapport
## 1 bis. Introduction du jeu de données
## 1. Traitement des valeurs manquantes
## 2. Statistique descriptive
## 3. Cluterring et Clustering ensembliste
## 4. EMM (Exceptional model mining)
## 5. Recherche des motifs fréquents et de règles d'association
## 6. Réduction de dimensions pour visualiser : PCA, t-NSE et Autoencoder
## 7. Expérience, pipeline work en Python



## Note beni

### Pour utiliser R dans Jupyter
```sh
conda install -c r rpy2
```

Puis dans JN : 
```
%load_ext rpy2.ipython
```

Puis utiliser ```%R``` ou ```%%R``` pour écrire du code.

Pour installer un package R connu : `install conda [-c r] r-<package name>`.  
Pour ajouter la channel r dans anaconda : `conda config --add channels r`  
Pour trouver la channel d'un package r non connu `anaconda search -t conda r-mlbench`. Le "répertoire" affiché est le nom de la cannel.  
Puis `anaconda -c channel r-<package>`.    
    
enables the %%R magic, not necessary if you've already done this  
```
%load_ext rpy2.ipython
```
import df from global env  
make default figure size 5 by 5 inches, you can change the units to px, cm, etc  
```
%%R -i df -w 5 -h 5 --units in -r 200
```
Pour utiliser un jeu de données de Python en R `%%R -i jeu_données`.

