# ALF

# Tema 2

Cerinta

Ecrivez une grammaire en PEG.js pour valider si un numero de carte de credit est vadid ou non

Solutia

Testam cu regex stringul dat astfel: 
"(4 cifre de la 0 la 9)-(4 cifre de la 0 la 9)-(4 cifre de la 0 la 9)-(4 cifre de la 0 la 9)"

Exemple de functionare corecta

1234-1234-1234-1234
4321-4321-4321-4321
2134-6434-5232-2315

Testarea functionarii corecte:

Intram pe siteul http://pegjs.org/online
Se introduce continutul fisierului "TD2.txt" in inputul numit "Write your PEG.js grammar" marcat cu cifra "1".
Se introduce in inputul numit "Test the generated parser with some input" marcat cu cifra "2" stringul pe care dorim sa-l validam (ex. "1234-1234-1234-1234")
In sectiunea "Output" va fi afisata validarea stringului astfel:
true - daca stringul dat reprezinta un numar de card de credit valid
false - daca stringul dat nu reprezinta un numar de card de credit valid

# Tema 3

Cerinta

Concevez la grammaire d'un langage de programmation a l'aide de PEG.js. Le langage peut-etre imperative ou fonctionnel selon votre choix. Il faut traiter les regles pour instruction imbriquee de type if-then-else

Solutia

Se parseaza inputul iar fiecare instructiune if trebuie sa fie de forma: ("text" = "text") sau "text" != "text"

Exemple de functionare corecta

"Valoarea 1" != "Valoarea 2"
("Valoarea 1" = "Valoarea 1" sau "Valoarea 2" != "Valoarea 2")
("Valoarea 1" = "Valoarea 1" sau ("Valoarea 2" = "Valoarea 2" si "Valoarea 3" = "Valoarea 3")) sau ("Valoarea 4" = "Valoarea 4" sau "Valoarea 5" = "Valoarea 5")
Testarea functionarii corecte:

Intram pe siteul http://pegjs.org/online
Se introduce continutul fisierului "TD3.txt" in inputul numit "Write your PEG.js grammar" marcat cu cifra "1".
Se introduce in inputul numit "Test the generated parser with some input" marcat cu cifra "2" stringul pe care dorim sa-l validam (exemple incluse mai sus)
In sectiunea "Output" va fi afisata parsarea instructiunilor iar fiecare instructiune if va fi afisata sub forma de array


