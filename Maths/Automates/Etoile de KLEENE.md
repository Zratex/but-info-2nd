$$L^{*} = L^{0}+L^{1} + L^{2} + ...$$
On utilise donc 2 méthodes de calcul :
- [[Addition langage]]
	- Exemple : $L^{1}+L^{2}$
- [[Multiplication langage]]
	- Exemple : $L^{2}=L*L$
	- [[Multiplication langage#Multiplication spéciale|Tout comme en algèbre]], $L^{0} = \varepsilon$
## Exemples
Admettons $\Sigma = {a,b}$
Alors :
- $(a+ab)^{*}=\varepsilon + (a+ab) + (a+ab)*(a+ab)+...$
	- Ici $(a+ab)*(a+ab) = (a+ab)^2$
- $(a+ab)^{*}={\varepsilon,a,ab,a^2,a^2b,aba,(ab)^2,...}$
	- Ici :
		- $a,ab=(a+ab)$
		- $a^2,a^2b,aba,(ab)^2=(a+ab)*(a+ab) = (a+ab)^2$
- $(a+ab)^{*}=$ `{mots construit à l'aide des blocs a et ab}`
### Exemple de simplification
$(a+b)^{*}=$({$a$}+{$b$})$^{*}=${$a,b$}$^{*}=\Sigma^{*}$