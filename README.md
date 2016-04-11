# ALF

Devoir 2

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
