l idee : rendre le back end operationel , pre processor sass 


1. cree dossier dans vscode 

2. ouvrir terminal avec gitbash: si soucis , redemarrer vscode

git --version --> te donne la version installer 

3. cree un dossier sass , ensuite 2 sous dossier scss / css

4. crée un dossier style.scss


5. dans le terminal 
node -v
npm -v

6. crée le package.json 

npm init 

7. installation de sass 

 npm install sass -g  

 npm install sass --save   --> crée la dependance dans le package.json 


8. ATTENTION : mettre cette adresse dans le package.json ds le script en dessous de test . 

  "sass": "sass --watch ./sass/scss/:./sass/css/"
                        dossier sous dossier seulement sinon y aura que le fichier pris en compte ex:
    /sass/scss/style.css:./sass/css/style.css

9. lancer le sass 

npm run sass 

10. arreter le pre processor sass 

ctrl + c -> relancer npm run sass 

11. ajouter les partials dans le dossier scss 
_le underscore fait savoir au compilateur qu il ne doit pas tenir compte de se fichier et ne pas le convertir en css

12. exemple : $header-color-h1: blue; --> a mettre dans la variable.scss car reutilisable . 

13. @import "variables" ainsi que les autres fichiers dans le fichier scss ; pour lié les fichiers au style.scss qui lui meme sera relié au style.css avec le preprocessor sass . 


14. cree fichier .gitignore 
et mettre node_modules pour qu il soit ignorer lorsqu ont met son projet sur github etc car volumineux et telechargeable via son terminal pc . 



15. cree docs , un genre de memo pour se rappeler la marche a suivre , les soucis , les tips etc , car svt
on fait le projet puis bcp de temps se passe et on oublie un peu . 

16. cree dossier images , views pour le contenu hmtl 
dossier js egalement 