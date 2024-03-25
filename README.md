# statTP
Ce TP fait référence au chapitre 3 du cours qui n’a pas été traité en amphi. N’hésitez pas à vous y
référer.
Considérons une réalisation x1, . . . , xn d’un échantillon X1, . . . , Xn de variables identiques et indépendantes de densité commune f. Le but de ce TP est de comparer les noyaux utilisés pour estimer la
densité commune f. Il faut bien comprendre que dans la pratique f est inconnue, ici, pour comparer
l’efficacité des noyaux et la taille de la fenêtre h nous allons supposer dans une première partie que f
est la densité d’une gaussienne centrée réduite, dans une seconde partie nous supposerons que f est la
densité d’une loi de dimension plus grande.
1. Si K : R → R+ est un noyau statistique et µ ∈ R une constante, la translation de K par la constante
a, τµK, est-elle encore un noyau statistique ?
2. Si K : R → R+ est un noyau statistique et λ ∈ R∗ une constante non nulle, montrer que dλK définie
pour tout x ∈ R par dλK(x) = 1
λK

x
λ

est encore un noyau statistique.
3. Montrer que K =
1
2
1[−1,1] est un noyau statistique, on l’appel le noyau uniforme.
4. Montrer que K(x) = (1 − |x|)1[−1,1](x) est un noyau statistique, on l’appel le noyau triangle.
5. Montrer que K(x) = 3
4
(1−x
2
)1[−1,1](x) est un noyau statistique, on l’appel le noyau d’Epanechnikov.
6. Montrer que K(x) = √
1
2π
e
−x
2/2
est un noyau statistique, on l’appel le noyau gaussien.
Soit h > 0 une constante appelée la fenêtre. Soit K un noyau statistique. On considère la fonction fbh,
définie pour tout x ∈ R, par :
fbh(x) = 1
n
Xn
k=1
dhτXiK(x)
C’est l’estimation de la densité f avec la fenêtre h et le noyau K
