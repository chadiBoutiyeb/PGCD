Définition du PGCD : 
      Le PGCD (Plus Grand Commun Diviseur) de deux entiers 𝑎 et b est le plus grand entier qui divise à la fois 𝑎 et b.


Ènoncé de l´algorithme d’Euclide : 
      L’algorithme d’Euclide permet de calculer le PGCD de deux entiers positifs 𝑎 et 𝑏 en utilisant des divisions successives 
    Ces divisions successives sont :
  Diviser 𝑎 par 𝑏 et noter le reste 𝑟.
  remplacer 𝑎 par 𝑏 et 𝑏 par 𝑟 puis recommencer
  si r=0 alors b est le PGCD 

Example : 252 % 105 = 42
           105 ÷ 42 = 21
           42 ÷ 21 = 0
21 est le PGCD

Example : 119 mod 68 = 51
          68 mod 51 = 17
          51 mod 17 = 0
17 est le PGCD


Algorithme (avec boucle TANT QUE) :
   Algorithme : PGCD
   Variables :
       a, b, r : entiers

   Début
    Lire a, b
     Tant que b ≠ 0 faire
           r ← a mod b
           Afficher "a =", a, ", b =", b, ", reste =", r
           a ← b
           b ← r
      Fin Tant que
    Afficher "Le PGCD est :", a
   Fin
