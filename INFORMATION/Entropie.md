<h5 style="text-align: center"> THÉORIE DE L'INFORMATION </h5>

------

## **Entropie**

------

### Principe

> ######Moins une observation est probable, plus son observation est porteuse d’information

---

### Quantité d’information

| **<u>Quantité d’information</u>** |
| :-------------------------------- |
| $h(x)=-\log (P(x))$               |

- Quantité positive et inversement proportionnelle à la probabilité de l’évènement
- Unité : 
  - $\ln​$ : Nat
  - $\log_{10}​$ : Hartley
  - $\log_{2}$ : Shannon (bit/symbole)

---

### Entropie

| **<u>Entropie</u>**                                          |
| :----------------------------------------------------------- |
| $H(X)=E[h(x)]=-\int\limits_{-\infty}^{+\infty}p_X(x)\cdot\log(p_X(x))dx$ |

- Cas limite : $\lim\limits_{p \rightarrow 0} \  p\log(p) = 0$

- L’entropie renseigne sur la redondance exprimée sur la base des $B$ bits de l’alphabet
- Plus une information est redondante, moins elle demande de support binaire (entropie plus faible)

######Entropie et concavité :

- Rappel : $\forall x \in \R^+_*, \ \ln(x)\le x-1$
- Distance euclidienne : $E=\frac{1}{N}\sum\limits_{i=1}^N (x_i-\overline x)^2$
  - $\overline x$ (barycentre) obtenu en minimisant $E$ $\left( \text{i.e. : } \frac{dE}{d\overline x} = 0 \right)$
- Entropie : fonction semi-définie positive et concave

######Entropie à $\pmb n$ symboles :

- **Inégalité de Gibbs** : $\forall P_i, Q_i : \sum\limits_{i=1}^n P_i = \sum\limits_{i=1}^n Q_i \implies \sum\limits_{i=1}^n P_i \cdot \log \left( \frac{P_i}{Q_i} \right) \le 0$
- $0\le H(X) \le \log(n)$
- $n=2^k \implies H(X) \le \log_2\left(2^k\right)$
- L’entropie est maximale pour une loi uniforme

###### Redondance

| **<u>Redondance</u>**            |
| :------------------------------- |
| $R(X)=1-\cfrac{H(X)}{\log_2(n)}$ |

- Plus la redondance est proche de 1, plus la taille binaire de codage peut être réduite

---

### Cas continu

- Modèle uniforme : $p_X(x)=\cfrac{1}{a} \ \delta_{[0,a]}(x)$
  - $H(X)=\log(a)$
- Modèle gaussien : $p_X(x)=\frac{1}{\sigma\sqrt{2\pi}}\exp\left(-\frac{(x-\mu)^2}{2\sigma^2}\right)$
  - $H(X)=\log(\sigma\sqrt{2\pi e})$   (ne dépend pas de la moyenne)
- Distance euclidienne : $E = \int (g_X(x)-p_X(x))^2dx$ : <u>non adaptée</u> car une densité de probabilité n’est pas un objet cartésien

###### Divergence de Kullback-Leibler

| **<u>Divergence de Kullback-Leibler ou entropie relative</u>** |
| :----------------------------------------------------------- |
| $D_{KL}(p_x \Vert \ p_Y)= \int p_X(a)\ln\left( \frac{p_X(a)}{p_Y(a)} \right)da$ |

- Divergence $\ne$ distance : pas de symétrie
- Modèle gaussien : $D_{KL}(p_x \Vert \ p_Y)= \log\left(\frac{\sigma_2}{\sigma_1}\right)+{1 \over 2}\left(\frac{1}{\sigma_2^2}-\frac{1}{\sigma_1^2}\right)(\sigma_1^2 - \sigma_2^2) + \mu_1\left(\frac{\mu_1}{\sigma_1^2}-\frac{\mu_2}{\sigma_2^2}\right)+{1 \over 2}\left(\frac{\mu_2}{\sigma_2^2}-\frac{\mu_1}{\sigma_1^2}\right)$



------

<table width="90%">
<tr>
<td style="width: 30%; text-align: left; background:transparent; border:0;">Théorie de l'information</td>
<td style="width: 30%; text-align: center; background:transparent; border:0;">Alexis Bagarre</td>
<td style="width: 30%; text-align: right; background:transparent; border:0;">T1 - 2018 / 2019</td>
</tr>
</table>