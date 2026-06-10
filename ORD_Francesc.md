# Documentació del procés

1. Creació del repositori

El repositori se ha creat desde el github

2. Clonació del repositori
```
git clone https://github.com/cescoliz/ORD_Francesc
```

3. Crear el README
```
cd ORD_Francesc
nano README.md
```

4. Creació de les branques
```
git branch info
git branch proces
```

5. Creació del projecte mkdocs
```
mkdocs new .
```

6. Modificació en el fitxer index.md
```
# Exàmen UD01 - Convocatòria Ordinària

[Infraestructura](infraestructura.md)
[Gh-pages](https://cescoliz.github.io/ORD_Francesc/)
```

7. Creació del document infraestructura.md
```
nano docs/infraestructura.md
```

8. Documentació de mkdocs pujada a main
```
git add mkdocs.yml docs/
git commit -m "Documentació de mkdocs pujada"
git push
```

9. Publicació de la branca info amb les imatges
```
git add img/
git commit -m "Imatges afegides a la branca info"
git push --set-upstream origin info
```

10. Canvi de branca i fusió de branques
```
git checkout main
git merge info
```

11. Publicació en gh-pages
```
mkdocs gh-deploy
```