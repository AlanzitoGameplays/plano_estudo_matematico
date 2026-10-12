# BLOCO III — OPERAÇÕES ENTRE CONJUNTOS

## TEXTO PRÁTICO — VERSÃO CANDIDATA

**Plano de Estudo Matemático 4.0 · Tópico 1.2 — Teoria dos Conjuntos**

---

# 1. Interseção, União e Condições de Pertinência

### 1. Duas condições, duas seleções

Complete as duas últimas colunas com V ou F, de acordo com as definições das operações.

| \(x\in A\) | \(x\in B\) | \(x\in A\cap B\) | \(x\in A\cup B\) |
|---|---|---|---|
| V | V |  |  |
| V | F |  |  |
| F | V |  |  |
| F | F |  |  |

a) Explique por que a primeira linha satisfaz a condição da união.

b) Um estudante afirma: “Para quaisquer conjuntos \(A\) e \(B\) e qualquer objeto \(x\), se \(x\in A\cup B\), então \(x\in A\cap B\)”. Identifique uma linha da tabela incompatível com essa afirmação. Em seguida, escolha conjuntos \(A\) e \(B\) e um elemento que realizem essa possibilidade e refutem a afirmação.

As linhas descrevem possibilidades de pertinência; não afirmam que todas elas ocorrem em quaisquer conjuntos escolhidos.

---

### 2. Operar sem confundir os objetos

Considere

\[
A=\{1,\{1\},2\},
\qquad
B=\{\{1\},2,3\}.
\]

a) Determine \(A\cap B\) e \(A\cup B\) por enumeração.

b) Determine se \(\{1\}\in A\cap B\) e se \(1\in A\cap B\). Justifique distinguindo os objetos examinados.

---

### 3. Da propriedade à operação

Considere

\[
D=\{1,2,3,4,5,6,7,8\},
\]

\[
P=\{x\in D\mid x>3\},
\qquad
Q=\{x\in D\mid x<6\}.
\]

a) Escreva \(P\cap Q\) e \(P\cup Q\) por propriedade, mantendo o domínio \(D\) explícito.

b) Determine os dois resultados por enumeração.

c) Existe algum elemento de \(D\) fora de \(P\cup Q\)? Justifique examinando as condições que selecionam os elementos do domínio.

---

### 4. Reconstruindo um conjunto e um diagrama

Sabe-se que

\[
U=\{a,b,c,d,e,f\},
\qquad
A=\{a,b,c\},
\qquad B\subseteq U,
\]

\[
A\cap B=\{b,c\},
\qquad
A\cup B=\{a,b,c,d,e\}.
\]

a) Determine \(B\). Explique como cada informação restringe seus elementos.

b) Construa um diagrama de Venn com o universo \(U\) e os conjuntos \(A\) e \(B\). Posicione cada elemento de \(U\) uma única vez, na região correspondente às suas pertinências.

c) Justifique por que \(f\) não pode pertencer a \(B\).

No diagrama, a posição registra pertinência; tamanhos e áreas das regiões não fornecem informação quantitativa.

---

### 5. Casos particulares sob a mesma definição

Complete a tabela para conjuntos arbitrários que satisfaçam a condição de cada linha. Simplifique cada resultado quando a condição permitir; quando ela não determinar uma redução da expressão, registre essa limitação.

| Condição | \(A\cap B\) | \(A\cup B\) |
|---|---|---|
| \(A\subseteq B\) |  |  |
| \(A\cap B=\varnothing\) |  |  |
| \(A=\varnothing\) |  |  |

a) Justifique os dois resultados da primeira linha usando a inclusão dada.

b) Na segunda linha, é possível substituir sempre \(A\cup B\) por \(A\) ou por \(B\)? Justifique.

c) Dois conjuntos disjuntos precisam ser diferentes? Apresente um exemplo que sustente sua resposta.

---

### 6. O agrupamento faz diferença?

Considere

\[
A=\{1,2\},
\qquad B=\{2,3\},
\qquad C=\{3,4\}.
\]

a) Determine

\[
X=(A\cup B)\cap C
\qquad\text{e}\qquad
Y=A\cup(B\cap C).
\]

b) Decida se \(X=Y\). Se forem diferentes, indique um elemento que testemunhe a diferença e registre suas duas relações de pertinência.

c) Para um objeto arbitrário \(x\), escreva as condições de pertinência a \(X\) e a \(Y\) usando apenas pertinências a \(A\), \(B\) e \(C\), conectivos lógicos e parênteses.

---

# 2. Diferença, Complemento e Universo

### 7. De qual conjunto partimos?

Considere

\[
U=\{a,b,c,d,e,f\},
\qquad A=\{a,b,c,d\},
\qquad B=\{c,d,e\}.
\]

a) Determine \(A\setminus B\) e \(B\setminus A\).

b) Um estudante argumenta: “Como \(f\notin B\), temos \(f\in A\setminus B\)”. Localize a condição que ele deixou de verificar e corrija a conclusão.

c) A definição de \(A\setminus B\) exige \(B\subseteq A\)? Responda usando os conjuntos dados e o significado da diferença.

---

### 8. Um conjunto, duas referências

Considere

\[
U=\{1,2,3,4,5,6\},
\qquad V=\{1,2,3,4,5,6,7,8\},
\qquad A=\{2,4\}.
\]

a) Determine \(U\setminus A\) e \(V\setminus A\).

b) Determine

\[
U\setminus(U\setminus A)
\qquad\text{e}\qquad
V\setminus(U\setminus A).
\]

c) Um estudante utiliza a identidade de dupla complementação para afirmar que os dois resultados do item b são iguais a \(A\). Explique por que a identidade não justifica essa conclusão e apresente uma testemunha da igualdade que falha.

---

### 9. Traduzindo condições de exclusão

Fixe um universo \(U\) e suponha \(A,B\subseteq U\). Todos os complementos desta atividade são relativos a \(U\).

a) Para \(x\in U\), escreva as condições de pertinência a cada conjunto abaixo usando somente \(x\in A\), \(x\in B\) e conectivos lógicos:

\[
X=A\setminus B,
\qquad
Y=U\setminus(A\cap B),
\qquad
Z=(U\setminus A)\cap B.
\]

b) Reescreva \(X\) como uma interseção com um complemento e \(Z\) como uma diferença. Justifique as duas reescritas pelas condições encontradas.

c) Qual das condições do item a admite um elemento de \(U\) que não pertença nem a \(A\) nem a \(B\)? Justifique.

---

### 10. As duas partes de um conjunto

Sabe-se que

\[
A=\{p,q,r,s\},
\qquad
A\cap B=\{q,s\},
\qquad
B\setminus A=\{t\}.
\]

a) Determine \(A\setminus B\) e \(B\). Explique por que as informações determinam esses resultados.

b) Verifique, com os conjuntos encontrados, que

\[
A=(A\cap B)\cup(A\setminus B).
\]

c) As duas parcelas do lado direito possuem algum elemento comum? Justifique pelas condições de pertinência a \(B\).

---

### 11. O que permanece após uma restrição?

*Baseada/adaptada de FATEC, vestibular do 2º semestre de 2025, questão 37, página 14.*

Fixe o universo \(U\) dos alimentos de um cardápio. Sejam \(A\subseteq U\) o conjunto dos alimentos que uma pessoa consumia regularmente e \(C\subseteq U\) o conjunto dos alimentos que contêm carne.

A pessoa passa a excluir de sua alimentação todos os alimentos de \(A\) que contêm carne. Nenhum alimento é acrescentado, e todos os demais alimentos de \(A\) permanecem. Denote o novo conjunto por \(B\).

a) Expresse \(B\) em termos de \(A\) e \(C\) e explique a condição que um alimento deve satisfazer para permanecer.

b) Reescreva a expressão com interseção e complemento relativo a \(U\).

c) Outra pessoa afirma que \(B=C^c\), com complemento em \(U\). Essa igualdade é garantida? Construa um exemplo com conjuntos finitos \(U\), \(A\) e \(C\) que sustente sua resposta e explique o papel de um alimento que não era consumido anteriormente.

---

# 3. Identidades e Relações entre Operações

### 12. O efeito de repetir, acrescentar e complementar

Fixe \(U\), suponha \(A\subseteq U\) e tome todos os complementos relativamente a \(U\).

Determine o resultado de cada expressão. Ao lado de cada resposta, identifique a propriedade correspondente: idempotência, neutralidade, dominância ou complementação. Para \(U^c\) e \(\varnothing^c\), registre diretamente o significado do complemento.

| Expressão | Resultado | Propriedade ou significado |
|---|---|---|
| \(A\cap A\) |  |  |
| \(A\cup A\) |  |  |
| \(A\cup\varnothing\) |  |  |
| \(A\cap U\) |  |  |
| \(A\cap\varnothing\) |  |  |
| \(A\cup U\) |  |  |
| \(A\cap A^c\) |  |  |
| \(A\cup A^c\) |  |  |
| \((A^c)^c\) |  |  |
| \(U^c\) |  |  |
| \(\varnothing^c\) |  |  |

Explique por que \(\varnothing\) preserva \(A\) em uma das operações e determina um resultado vazio na outra.

---

### 13. Reorganizar sem alterar a seleção

Para conjuntos arbitrários \(A\), \(B\) e \(C\), simplifique cada expressão até que cada letra apareça uma única vez.

\[
X=(A\cup B)\cup(C\cup A),
\]

\[
Y=(B\cap A)\cap(A\cap C).
\]

Apresente uma cadeia de igualdades e identifique as propriedades que autorizam o reagrupamento, a troca de ordem e a retirada de uma repetição.

---

### 14. Uma exigência já está contida na outra?

Para conjuntos arbitrários \(A\), \(B\) e \(C\), simplifique

\[
E=\bigl(A\cap(A\cup B)\bigr)\cup(A\cap C).
\]

a) Apresente as igualdades usadas e justifique cada transformação.

b) Explique, por condições de pertinência, por que o resultado não depende da escolha de \(B\) e \(C\).

---

### 15. Duas maneiras de distribuir

Considere conjuntos arbitrários \(A\), \(B\) e \(C\) e as expressões

\[
X=(A\cap B)\cup(A\cap C),
\qquad
Y=(A\cup B)\cap(A\cup C).
\]

a) Reescreva \(X\) e \(Y\) de modo que \(A\) apareça uma única vez em cada expressão. Identifique as identidades utilizadas.

b) É sempre verdade que \(X=Y\)? Demonstre, se a afirmação for verdadeira, ou construa e verifique um contraexemplo, se for falsa.

---

### 16. O complemento de uma construção composta

Fixe \(U\), suponha \(A,B,C\subseteq U\) e tome todos os complementos em \(U\).

Reescreva as expressões abaixo de modo que o complemento apareça somente sobre conjuntos individuais, sem complementar uniões, interseções ou diferenças:

\[
E=\bigl(A\cup(B\cap C)\bigr)^c,
\qquad
F=(A\setminus B)^c.
\]

Justifique as transformações.

---

### 17. Identidades propostas: refutar e reparar

Um estudante propõe as duas igualdades abaixo para quaisquer conjuntos \(A\), \(B\) e \(C\):

\[
\text{I.}\quad A\setminus(B\setminus C)=(A\setminus B)\setminus C;
\]

\[
\text{II.}\quad A\setminus(B\cap C)=(A\setminus B)\cap(A\setminus C).
\]

a) Para cada proposta, construa um contraexemplo. Calcule os dois lados e identifique uma testemunha da desigualdade.

b) Na proposta II, substitua apenas a operação entre as duas diferenças do lado direito para obter uma identidade válida. Justifique a correção por condições de pertinência.

---

# 4. Demonstração, Integração e Transferência

### 18. Completando uma demonstração por pertinência

Sejam \(A\), \(B\) e \(C\) conjuntos arbitrários. Para um objeto \(x\) arbitrário, complete as lacunas da demonstração, mantendo as equivalências válidas:

\[
\begin{aligned}
x\in A\setminus(B\cup C)
&\iff (x\in A)\land\neg\bigl((x\in B)\lor(x\in C)\bigr)\\
&\iff (x\in A)\land\bigl(\underline{\hspace{1.5cm}}\land\underline{\hspace{1.5cm}}\bigr)\\
&\iff \bigl((x\in A)\land\underline{\hspace{1.5cm}}\bigr)
\land\bigl((x\in A)\land\underline{\hspace{1.5cm}}\bigr)\\
&\iff x\in\underline{\hspace{2cm}}\cap\underline{\hspace{2cm}}.
\end{aligned}
\]

a) Identifique a lei lógica utilizada na primeira transformação que você completou.

b) Explique por que repetir a exigência \(x\in A\) não muda a condição.

c) Escreva a igualdade entre conjuntos demonstrada e explique por que a argumentação estabelece uma identidade, em vez de verificar apenas um caso.

---

### 19. Demonstrando por dupla inclusão

Para conjuntos arbitrários \(A\), \(B\) e \(C\), demonstre por dupla inclusão que

\[
A\cup(B\cap C)=(A\cup B)\cap(A\cup C).
\]

Apresente separadamente as duas inclusões. Em cada direção, explicite o que pode ser concluído sobre um elemento arbitrário e justifique a passagem ao conjunto do outro lado.

---

### 20. A conclusão está sustentada?

Fixe \(U\) e suponha \(A,B\subseteq U\). Todos os complementos são relativos a \(U\). Dois estudantes tentam demonstrar a identidade

\[
(A\cap B)^c=A^c\cup B^c.
\]

**Argumento I**

> Tomei \(U=\{1,2,3\}\), \(A=\{1,2\}\) e \(B=\{2,3\}\). Obtive \((A\cap B)^c=\{1,3\}\) e \(A^c\cup B^c=\{1,3\}\). Portanto, a igualdade vale para quaisquer conjuntos no mesmo universo.

**Argumento II**

> Seja \(x\in A^c\cup B^c\) arbitrário. Então \(x\in U\) e, além disso, \(x\notin A\) ou \(x\notin B\). Logo, \(x\notin A\cap B\), de modo que \(x\in(A\cap B)^c\). Portanto, os dois conjuntos são iguais.

a) Determine o que foi efetivamente estabelecido em cada argumento e localize a passagem que não está justificada.

b) Complete o Argumento II com o raciocínio que falta para demonstrar a identidade.

---

### 21. Reconhecendo a inclusão por operações

Para conjuntos arbitrários \(A\) e \(B\), demonstre que as quatro afirmações são equivalentes:

\[
\text{I. }A\subseteq B;
\qquad
\text{II. }A\setminus B=\varnothing;
\]

\[
\text{III. }A\cap B=A;
\qquad
\text{IV. }A\cup B=B.
\]

Organize uma demonstração que estabeleça todas as equivalências. Não basta listar propriedades ou verificar conjuntos particulares. Você pode escolher a ordem das implicações que utilizará.

---

### 22. O que uma inclusão permite concluir?

Sejam \(A\), \(B\) e \(C\) conjuntos arbitrários, com \(A\subseteq B\). Avalie as afirmações:

\[
\text{I. }A\cap C\subseteq B\cap C;
\]

\[
\text{II. }A\setminus C\subseteq B\setminus C;
\]

\[
\text{III. }C\setminus A\subseteq C\setminus B.
\]

a) Demonstre cada afirmação que seja válida sob a hipótese dada, usando um elemento arbitrário.

b) Para cada afirmação inválida, construa e verifique um contraexemplo que preserve \(A\subseteq B\).

c) Para cada afirmação inválida, investigue se inverter a direção da inclusão produz uma relação válida sob a hipótese dada. Justifique sua resposta.

---

### 23. Traduzir uma regra e controlar sua simplificação

Em um sistema de inscrições, o universo \(U\) reúne as pessoas cadastradas. Sejam:

- \(S\): pessoas inscritas em uma atividade;
- \(R\): pessoas com cadastro regular;
- \(D\): pessoas com a documentação completa.

Os três conjuntos estão incluídos em \(U\). O sistema envia um aviso exatamente às pessoas inscritas que **não satisfazem conjuntamente** as condições de cadastro regular e documentação completa. Denote o conjunto das pessoas avisadas por \(E\).

a) Expresse \(E\) usando operações entre \(S\), \(R\) e \(D\). Reescreva-o como uma união de diferenças e justifique a equivalência.

b) Um programador usa \(S\setminus(R\cup D)\) para executar a regra. Determine se essa expressão é adequada. Se não for, apresente uma combinação de pertinências que produza resultados diferentes e explique o erro.

c) Suponha agora que todas as pessoas inscritas tenham cadastro regular, isto é, \(S\subseteq R\). Simplifique \(E\) sob essa hipótese e demonstre sua resposta.

---

### 24. Reconstruir, verificar e decidir se os dados são possíveis

São dados três conjuntos \(B\), \(P\) e \(Q\). Procura-se um conjunto \(A\) que satisfaça simultaneamente

\[
A\cap B=P
\qquad\text{e}\qquad
A\setminus B=Q.
\]

a) Demonstre que, se existir um conjunto \(A\) com essas propriedades, ele deverá ser \(P\cup Q\).

b) Tomar \(A=P\cup Q\) garante as duas propriedades para quaisquer \(B\), \(P\) e \(Q\)? Determine condições necessárias e suficientes sobre \(P\) e \(Q\) em relação a \(B\) para que essa construção funcione. Demonstre tanto a necessidade quanto a suficiência das condições.

c) Aplique seu resultado aos dois registros abaixo. Quando houver solução, determine \(A\); quando não houver, identifique a incompatibilidade.

\[
\begin{aligned}
\text{Registro I: }&B=\{b,d\},\quad P=\{b\},\quad Q=\{a,c\};\\
\text{Registro II: }&B=\{b,d\},\quad P=\{b\},\quad Q=\{a,d\}.
\end{aligned}
\]

---

# GABARITO COMENTADO

# 1. Interseção, União e Condições de Pertinência

### 1. Duas condições, duas seleções

| \(x\in A\) | \(x\in B\) | \(x\in A\cap B\) | \(x\in A\cup B\) |
|---|---|---|---|
| V | V | V | V |
| V | F | F | V |
| F | V | F | V |
| F | F | F | F |

**a)** A união exige pertencer a pelo menos um dos conjuntos. Quem pertence aos dois satisfaz essa exigência. O OU é inclusivo.

**b)** A segunda linha apresenta uma possibilidade incompatível com a afirmação: um elemento que pertence a \(A\), mas não a \(B\), pertence à união e não à interseção. Para realizá-la, podemos tomar

\[
A=\{1\},\qquad B=\{2\},\qquad x=1.
\]

Nesse caso, \(1\in A\cup B\), mas \(1\notin A\cap B\). Esse contraexemplo refuta a afirmação universal. A terceira linha também pode ser utilizada, com um elemento que pertença apenas a \(B\). Não é necessário que a possibilidade escolhida ocorra em todos os pares de conjuntos: basta uma escolha que contradiga a afirmação.

---

### 2. Operar sem confundir os objetos

**a)** Os objetos comuns são o conjunto \(\{1\}\) e o número \(2\). Portanto,

\[
\boxed{A\cap B=\{\{1\},2\}},
\qquad
\boxed{A\cup B=\{1,\{1\},2,3\}}.
\]

**b)** Temos

\[
\boxed{\{1\}\in A\cap B}
\qquad\text{e}\qquad
\boxed{1\notin A\cap B}.
\]

O conjunto \(\{1\}\) é um elemento de ambos os conjuntos dados. O número \(1\) pertence a \(A\), mas não a \(B\). A presença de \(\{1\}\) em \(B\) não torna \(1\) elemento de \(B\).

---

### 3. Da propriedade à operação

**a)**

\[
\boxed{P\cap Q=\{x\in D\mid x>3\land x<6\}},
\]

\[
\boxed{P\cup Q=\{x\in D\mid x>3\lor x<6\}}.
\]

**b)** Como \(P=\{4,5,6,7,8\}\) e \(Q=\{1,2,3,4,5\}\),

\[
\boxed{P\cap Q=\{4,5\}},
\qquad
\boxed{P\cup Q=\{1,2,3,4,5,6,7,8\}=D}.
\]

**c)** Não existe elemento de \(D\) fora da união. Dentro de \(D\), os elementos \(1,2,3\) satisfazem \(x<6\); \(4,5\) satisfazem as duas condições; e \(6,7,8\) satisfazem \(x>3\). Todo elemento do domínio atende a pelo menos uma condição. Nenhum objeto externo a \(D\) entra, pois ambos os conjuntos foram definidos dentro dele. Portanto, \(P\cup Q=D\).

---

### 4. Reconstruindo um conjunto e um diagrama

**a)** A interseção determina que \(b,c\in B\) e que \(a\notin B\), pois \(a\in A\), mas não aparece na interseção. Os elementos \(d,e\) aparecem na união e não pertencem a \(A\), logo precisam pertencer a \(B\). O elemento \(f\) não aparece na união. Assim,

\[
\boxed{B=\{b,c,d,e\}}.
\]

**b)** O diagrama deve registrar as seguintes posições:

| Região | Elementos |
|---|---|
| Em \(A\), fora de \(B\) | \(a\) |
| Em \(A\) e em \(B\) | \(b,c\) |
| Em \(B\), fora de \(A\) | \(d,e\) |
| Em \(U\), fora de ambos | \(f\) |

Qualquer desenho legível com essas pertinências, os rótulos dos conjuntos e o limite de \(U\) atende ao comando. A tabela permite conferir o desenho; não atribui significado às áreas.

**c)** Se \(f\in B\), então \(f\in A\cup B\), contrariando a união fornecida. Portanto, \(f\notin B\).

---

### 5. Casos particulares sob a mesma definição

| Condição | \(A\cap B\) | \(A\cup B\) |
|---|---|---|
| \(A\subseteq B\) | \(A\) | \(B\) |
| \(A\cap B=\varnothing\) | \(\varnothing\) | \(A\cup B\) |
| \(A=\varnothing\) | \(\varnothing\) | \(B\) |

Na segunda linha, a informação de que os conjuntos são disjuntos não determina uma redução da união a um dos dois conjuntos.

**a)** Se \(A\subseteq B\), todo elemento de \(A\) também pertence a \(B\), de modo que os elementos comuns são exatamente os de \(A\). Reunir os elementos de \(A\) aos de \(B\) não acrescenta nada a \(B\).

**b)** Não. Por exemplo, \(A=\{1\}\) e \(B=\{2\}\) são disjuntos, mas sua união é \(\{1,2\}\), diferente de ambos.

**c)** Não. Tomando \(A=B=\varnothing\), temos \(A\cap B=\varnothing\) e \(A=B\). Se dois conjuntos iguais forem disjuntos, eles terão necessariamente de ser vazios, pois \(A\cap A=A\).

---

### 6. O agrupamento faz diferença?

**a)**

\[
A\cup B=\{1,2,3\},
\qquad
\boxed{X=\{3\}};
\]

\[
B\cap C=\{3\},
\qquad
\boxed{Y=\{1,2,3\}}.
\]

**b)** \(X\neq Y\). Uma testemunha é \(1\), pois \(1\in Y\) e \(1\notin X\). O número \(2\) também serve.

**c)**

\[
x\in X\iff\bigl((x\in A)\lor(x\in B)\bigr)\land(x\in C),
\]

\[
x\in Y\iff(x\in A)\lor\bigl((x\in B)\land(x\in C)\bigr).
\]

As condições são diferentes: em \(X\), pertencer a \(C\) é obrigatório; em \(Y\), pertencer a \(A\) já basta. A associatividade de uma operação isolada não permite deslocar parênteses livremente entre operações diferentes.

---

# 2. Diferença, Complemento e Universo

### 7. De qual conjunto partimos?

**a)**

\[
\boxed{A\setminus B=\{a,b\}},
\qquad
\boxed{B\setminus A=\{e\}}.
\]

**b)** Falta verificar \(f\in A\). Na realidade, \(f\notin A\), portanto

\[
\boxed{f\notin A\setminus B}.
\]

A diferença exige as duas condições: pertencer ao primeiro conjunto e não pertencer ao segundo.

**c)** Não. Neste caso, \(e\in B\) e \(e\notin A\), logo \(B\nsubseteq A\), mas \(A\setminus B\) está perfeitamente definida. Os elementos de \(B\) externos a \(A\) não excluem nenhum elemento adicional da coleção de partida.

---

### 8. Um conjunto, duas referências

**a)**

\[
\boxed{U\setminus A=\{1,3,5,6\}},
\qquad
\boxed{V\setminus A=\{1,3,5,6,7,8\}}.
\]

**b)**

\[
\boxed{U\setminus(U\setminus A)=\{2,4\}=A},
\]

\[
\boxed{V\setminus(U\setminus A)=\{2,4,7,8\}}.
\]

**c)** A dupla complementação recupera \(A\) quando as duas complementações usam o mesmo universo. A primeira expressão preserva \(U\); a segunda começa com o complemento em \(U\) e depois toma o complemento desse resultado em \(V\). O número \(7\) testemunha a falha da segunda igualdade: pertence a \(V\setminus(U\setminus A)\), mas não a \(A\). O número \(8\) também serve.

---

### 9. Traduzindo condições de exclusão

**a)** Para \(x\in U\),

\[
\begin{aligned}
x\in X&\iff(x\in A)\land\neg(x\in B);\\
x\in Y&\iff\neg\bigl((x\in A)\land(x\in B)\bigr)\\
&\iff\neg(x\in A)\lor\neg(x\in B);\\
x\in Z&\iff\neg(x\in A)\land(x\in B).
\end{aligned}
\]

**b)**

\[
\boxed{X=A\cap B^c},
\qquad
\boxed{Z=B\setminus A}.
\]

Como \(x\in U\), não pertencer a \(B\) equivale a pertencer a \(B^c\). A condição de \(Z\) exige pertencer a \(B\) e não a \(A\), exatamente na direção da diferença indicada.

**c)** Somente \(Y\). Para um elemento fora de ambos, as duas pertinências são falsas e a negação da condição conjunta é verdadeira. Já \(X\) exige pertencer a \(A\), e \(Z\) exige pertencer a \(B\).

---

### 10. As duas partes de um conjunto

**a)** Em \(A\), os elementos \(q,s\) pertencem a \(B\), enquanto \(p,r\) não pertencem a \(B\). Portanto,

\[
\boxed{A\setminus B=\{p,r\}}.
\]

Os elementos de \(B\) que pertencem a \(A\) são \(q,s\), e o único elemento de \(B\) externo a \(A\) é \(t\). Assim,

\[
\boxed{B=\{q,s,t\}}.
\]

**b)**

\[
(A\cap B)\cup(A\setminus B)
=\{q,s\}\cup\{p,r\}
=\{p,q,r,s\}=A.
\]

Essa enumeração verifica a igualdade para os conjuntos da atividade.

**c)** Não. Um elemento da primeira parcela pertence a \(B\); um elemento da segunda não pertence a \(B\). Pertencer às duas exigiria simultaneamente essas condições incompatíveis. Logo, as parcelas são disjuntas.

---

### 11. O que permanece após uma restrição?

**a)**

\[
\boxed{B=A\setminus C}.
\]

Um alimento permanece exatamente quando era consumido antes e não contém carne: \(x\in A\) e \(x\notin C\). A hipótese de que não há acréscimos preserva a coleção de partida \(A\).

**b)** Com complemento em \(U\),

\[
\boxed{B=A\cap C^c}.
\]

**c)** A igualdade \(B=C^c\) não é garantida. Como exemplo, denote por \(a\) e \(b\) dois alimentos sem carne e por \(c\) um alimento com carne. Tome

\[
U=\{a,b,c\},
\qquad A=\{a,c\},
\qquad C=\{c\}.
\]

Então

\[
B=A\setminus C=\{a\},
\qquad C^c=\{a,b\}.
\]

O alimento \(b\) está no cardápio e não contém carne, mas não era consumido anteriormente. Ele pertence a \(C^c\), porém não entra em \(B\). Qualquer exemplo que respeite o universo e apresente um elemento de \(C^c\) externo a \(A\) refuta a igualdade proposta.

---

# 3. Identidades e Relações entre Operações

### 12. O efeito de repetir, acrescentar e complementar

| Expressão | Resultado | Propriedade ou significado |
|---|---|---|
| \(A\cap A\) | \(A\) | Idempotência |
| \(A\cup A\) | \(A\) | Idempotência |
| \(A\cup\varnothing\) | \(A\) | Neutralidade do vazio na união |
| \(A\cap U\) | \(A\) | Neutralidade do universo na interseção |
| \(A\cap\varnothing\) | \(\varnothing\) | Dominância do vazio na interseção |
| \(A\cup U\) | \(U\) | Dominância do universo na união |
| \(A\cap A^c\) | \(\varnothing\) | Complementação: condições incompatíveis |
| \(A\cup A^c\) | \(U\) | Complementação: todas as possibilidades em \(U\) |
| \((A^c)^c\) | \(A\) | Dupla complementação no mesmo universo |
| \(U^c\) | \(\varnothing\) | Nenhum elemento de \(U\) está fora de \(U\) |
| \(\varnothing^c\) | \(U\) | Todo elemento de \(U\) está fora do vazio |

Na união, o vazio não acrescenta elementos a \(A\). Na interseção, a exigência de pertencer também ao vazio não pode ser satisfeita por nenhum objeto. O comportamento depende da operação.

---

### 13. Reorganizar sem alterar a seleção

Uma cadeia possível para \(X\) é

\[
\begin{aligned}
(A\cup B)\cup(C\cup A)
&=((A\cup B)\cup C)\cup A&&\text{(associatividade)}\\
&=A\cup((A\cup B)\cup C)&&\text{(comutatividade)}\\
&=((A\cup A)\cup B)\cup C&&\text{(associatividade)}\\
&=(A\cup B)\cup C&&\text{(idempotência)}.
\end{aligned}
\]

Portanto, \(\boxed{X=A\cup B\cup C}\).

Para \(Y\),

\[
\begin{aligned}
(B\cap A)\cap(A\cap C)
&=(A\cap B)\cap(A\cap C)&&\text{(comutatividade)}\\
&=((A\cap B)\cap A)\cap C&&\text{(associatividade)}\\
&=(A\cap(B\cap A))\cap C&&\text{(associatividade)}\\
&=(A\cap(A\cap B))\cap C&&\text{(comutatividade)}\\
&=((A\cap A)\cap B)\cap C&&\text{(associatividade)}\\
&=(A\cap B)\cap C&&\text{(idempotência)}.
\end{aligned}
\]

Assim, \(\boxed{Y=A\cap B\cap C}\). Outras cadeias são válidas quando as transformações preservam os conjuntos e suas justificativas são identificáveis.

---

### 14. Uma exigência já está contida na outra?

**a)** Pela absorção,

\[
\begin{aligned}
E&=\bigl(A\cap(A\cup B)\bigr)\cup(A\cap C)\\
&=A\cup(A\cap C)\\
&=\boxed{A}.
\end{aligned}
\]

A primeira transformação utiliza \(A\cap(A\cup B)=A\); a segunda utiliza \(A\cup(A\cap C)=A\).

**b)** Se \(x\in E\), então \(x\in A\cap(A\cup B)\) ou \(x\in A\cap C\). Em ambos os casos, \(x\in A\). Reciprocamente, se \(x\in A\), então \(x\in A\cup B\), logo \(x\in A\cap(A\cup B)\subseteq E\). Portanto, \(x\in E\iff x\in A\) para qualquer \(x\), independentemente de \(B\) e \(C\).

---

### 15. Duas maneiras de distribuir

**a)** Pelas duas identidades distributivas,

\[
\boxed{X=A\cap(B\cup C)},
\qquad
\boxed{Y=A\cup(B\cap C)}.
\]

**b)** Não é sempre verdade que \(X=Y\). Tome

\[
A=\{1\},\qquad B=C=\varnothing.
\]

Então

\[
X=(A\cap\varnothing)\cup(A\cap\varnothing)=\varnothing,
\]

\[
Y=(A\cup\varnothing)\cap(A\cup\varnothing)=\{1\}.
\]

Assim, \(1\in Y\) e \(1\notin X\). O uso do vazio é legítimo: a afirmação proposta não restringe os conjuntos a serem não vazios.

---

### 16. O complemento de uma construção composta

Aplicando sucessivamente as duas leis de De Morgan,

\[
\begin{aligned}
E&=\bigl(A\cup(B\cap C)\bigr)^c\\
&=A^c\cap(B\cap C)^c\\
&=\boxed{A^c\cap(B^c\cup C^c)}.
\end{aligned}
\]

Para \(F\), escrevemos a diferença como interseção com o complemento e usamos De Morgan e dupla complementação:

\[
\begin{aligned}
F&=(A\setminus B)^c\\
&=(A\cap B^c)^c\\
&=A^c\cup(B^c)^c\\
&=\boxed{A^c\cup B}.
\end{aligned}
\]

O universo permanece \(U\) em todas as transformações, e todos os conjuntos envolvidos estão incluídos nele.

---

### 17. Identidades propostas: refutar e reparar

**a) Proposta I.** Tome \(A=B=C=\{1\}\). Então

\[
A\setminus(B\setminus C)=\{1\}\setminus\varnothing=\{1\},
\]

\[
(A\setminus B)\setminus C=\varnothing\setminus\{1\}=\varnothing.
\]

O elemento \(1\) pertence ao lado esquerdo e não ao direito. Logo, a diferença não admite o reagrupamento proposto.

**Proposta II.** Tome \(A=B=\{1\}\) e \(C=\{2\}\). Temos

\[
A\setminus(B\cap C)=\{1\}\setminus\varnothing=\{1\},
\]

\[
(A\setminus B)\cap(A\setminus C)
=\varnothing\cap\{1\}=\varnothing.
\]

Novamente, \(1\) testemunha a desigualdade. Outros contraexemplos são suficientes se os resultados e a testemunha forem corretamente verificados.

**b)** A operação correta é a união:

\[
\boxed{A\setminus(B\cap C)=(A\setminus B)\cup(A\setminus C)}.
\]

Para \(x\) arbitrário,

\[
\begin{aligned}
x\in A\setminus(B\cap C)
&\iff(x\in A)\land\neg\bigl((x\in B)\land(x\in C)\bigr)\\
&\iff(x\in A)\land\bigl((x\notin B)\lor(x\notin C)\bigr)\\
&\iff\bigl((x\in A)\land(x\notin B)\bigr)
\lor\bigl((x\in A)\land(x\notin C)\bigr)\\
&\iff x\in(A\setminus B)\cup(A\setminus C).
\end{aligned}
\]

Foram usadas a lei lógica de De Morgan e a distributividade lógica. A equivalência de pertinência para todo objeto demonstra a identidade, sem necessidade de definir complementos ou escolher um universo.

---

# 4. Demonstração, Integração e Transferência

### 18. Completando uma demonstração por pertinência

A cadeia completa é

\[
\begin{aligned}
x\in A\setminus(B\cup C)
&\iff(x\in A)\land\neg\bigl((x\in B)\lor(x\in C)\bigr)\\
&\iff(x\in A)\land\bigl((x\notin B)\land(x\notin C)\bigr)\\
&\iff\bigl((x\in A)\land(x\notin B)\bigr)
\land\bigl((x\in A)\land(x\notin C)\bigr)\\
&\iff x\in(A\setminus B)\cap(A\setminus C).
\end{aligned}
\]

**a)** Foi usada a lei lógica de De Morgan para a negação de uma disjunção.

**b)** A condição composta exige \(x\in A\), \(x\notin B\) e \(x\notin C\). Repetir a primeira exigência não a fortalece: \(p\land p\iff p\). Associatividade, comutatividade e idempotência da conjunção autorizam o reagrupamento mostrado.

**c)** A identidade demonstrada é

\[
\boxed{A\setminus(B\cup C)=(A\setminus B)\cap(A\setminus C)}.
\]

O objeto \(x\) e os conjuntos são arbitrários. Cada equivalência decorre das definições e de leis lógicas, sem depender de elementos particulares ou de conjuntos não vazios. Assim, os dois lados possuem exatamente os mesmos elementos em todos os casos admitidos.

---

### 19. Demonstrando por dupla inclusão

**Primeira inclusão.** Seja \(x\in A\cup(B\cap C)\) arbitrário. Então \(x\in A\) ou \(x\in B\cap C\).

Se \(x\in A\), ele pertence tanto a \(A\cup B\) quanto a \(A\cup C\). Se \(x\in B\cap C\), ele pertence a \(B\) e a \(C\), o que também garante as duas uniões. Em qualquer alternativa,

\[
x\in(A\cup B)\cap(A\cup C).
\]

Portanto,

\[
A\cup(B\cap C)\subseteq(A\cup B)\cap(A\cup C).
\]

**Inclusão inversa.** Seja \(x\in(A\cup B)\cap(A\cup C)\) arbitrário. Então

\[
x\in A\cup B
\qquad\text{e}\qquad
x\in A\cup C.
\]

Se \(x\in A\), já temos \(x\in A\cup(B\cap C)\). Se \(x\notin A\), a primeira união exige \(x\in B\), e a segunda exige \(x\in C\). Logo, \(x\in B\cap C\) e, novamente, \(x\in A\cup(B\cap C)\). Assim,

\[
(A\cup B)\cap(A\cup C)\subseteq A\cup(B\cap C).
\]

Pela dupla inclusão,

\[
\boxed{A\cup(B\cap C)=(A\cup B)\cap(A\cup C)}.
\]

Outras demonstrações por dupla inclusão são válidas se estabelecem as duas direções para elementos arbitrários. Verificar exemplos ou citar apenas o nome da identidade não atende ao comando desta atividade.

---

### 20. A conclusão está sustentada?

**a) Argumento I.** O cálculo está correto: naquele universo e com aqueles conjuntos, os dois lados são \(\{1,3\}\). Foi estabelecida uma igualdade particular. A passagem desse caso para “quaisquer conjuntos” não está justificada. Conjuntos escolhidos favoravelmente não substituem um raciocínio geral.

**Argumento II.** O raciocínio com \(x\) é válido até a conclusão

\[
\boxed{A^c\cup B^c\subseteq(A\cap B)^c}.
\]

O erro está em concluir a igualdade a partir dessa única inclusão. Falta estabelecer a inclusão inversa.

**b)** Seja \(x\in(A\cap B)^c\) arbitrário. Então \(x\in U\) e \(x\notin A\cap B\). Pelas definições e pela lei lógica de De Morgan,

\[
\neg\bigl((x\in A)\land(x\in B)\bigr)
\iff(x\notin A)\lor(x\notin B).
\]

Como \(x\in U\), a condição equivale a \(x\in A^c\) ou \(x\in B^c\). Portanto, \(x\in A^c\cup B^c\), mostrando que

\[
(A\cap B)^c\subseteq A^c\cup B^c.
\]

Junto com a inclusão demonstrada no Argumento II, obtemos a igualdade por dupla inclusão. Não basta repetir a igualdade pretendida: é necessário justificar essa direção ausente.

---

### 21. Reconhecendo a inclusão por operações

Uma possibilidade é estabelecer o ciclo

\[
\text{I}\Rightarrow\text{II}\Rightarrow\text{III}\Rightarrow\text{IV}\Rightarrow\text{I}.
\]

**I \(\Rightarrow\) II.** Se \(A\subseteq B\), não existe elemento que pertença a \(A\) e não pertença a \(B\). Essa é precisamente a condição exigida pela diferença. Logo, \(A\setminus B=\varnothing\).

**II \(\Rightarrow\) III.** Suponha \(A\setminus B=\varnothing\). Para \(x\in A\) arbitrário, não pode ocorrer \(x\notin B\), pois isso colocaria \(x\) na diferença vazia. Assim, \(x\in B\), e portanto \(x\in A\cap B\). Logo, \(A\subseteq A\cap B\). A inclusão \(A\cap B\subseteq A\) decorre diretamente da definição de interseção. Pela dupla inclusão, \(A\cap B=A\).

**III \(\Rightarrow\) IV.** Suponha \(A\cap B=A\). Todo elemento de \(A\) pertence à interseção e, portanto, a \(B\). Agora, se \(x\in A\cup B\), ele pertence a \(A\) ou a \(B\); em ambos os casos, pertence a \(B\). Assim, \(A\cup B\subseteq B\). Como \(B\subseteq A\cup B\) pela definição de união, temos \(A\cup B=B\).

**IV \(\Rightarrow\) I.** Suponha \(A\cup B=B\). Para \(x\in A\) arbitrário, temos \(x\in A\cup B\), logo \(x\in B\). Portanto, \(A\subseteq B\).

O ciclo garante que qualquer uma das afirmações implica todas as outras. Isso demonstra

\[
\boxed{A\subseteq B\iff A\setminus B=\varnothing
\iff A\cap B=A\iff A\cup B=B}.
\]

Também é suficiente demonstrar a equivalência entre I e cada uma das demais, com os dois sentidos justificados. O raciocínio continua válido se algum conjunto for vazio; nenhuma passagem exige a existência de um elemento de \(A\).

---

### 22. O que uma inclusão permite concluir?

**a) Afirmação I — válida.** Seja \(x\in A\cap C\) arbitrário. Então \(x\in A\) e \(x\in C\). Como \(A\subseteq B\), também \(x\in B\). Portanto, \(x\in B\cap C\), demonstrando

\[
\boxed{A\cap C\subseteq B\cap C}.
\]

**Afirmação II — válida.** Seja \(x\in A\setminus C\) arbitrário. Temos \(x\in A\) e \(x\notin C\). A inclusão dada fornece \(x\in B\); preservando \(x\notin C\), concluímos \(x\in B\setminus C\). Logo,

\[
\boxed{A\setminus C\subseteq B\setminus C}.
\]

**b) Afirmação III — inválida em geral.** Tome

\[
A=\{1\},\qquad B=\{1,2\},\qquad C=\{2\}.
\]

A hipótese \(A\subseteq B\) é satisfeita, mas

\[
C\setminus A=\{2\},
\qquad C\setminus B=\varnothing.
\]

O elemento \(2\) pertence ao conjunto da esquerda e não ao da direita, refutando a inclusão proposta.

**c)** A direção correta é

\[
\boxed{C\setminus B\subseteq C\setminus A}.
\]

Seja \(x\in C\setminus B\) arbitrário. Então \(x\in C\) e \(x\notin B\). Não pode ocorrer \(x\in A\), pois \(A\subseteq B\) implicaria \(x\in B\). Logo, \(x\notin A\), e portanto \(x\in C\setminus A\). Ao excluir o conjunto maior \(B\) da mesma coleção \(C\), nenhum elemento adicional pode permanecer.

---

### 23. Traduzir uma regra e controlar sua simplificação

**a)** A pessoa deve pertencer a \(S\) e não satisfazer a condição conjunta de pertinência a \(R\) e \(D\). Assim,

\[
\boxed{E=S\setminus(R\cap D)}.
\]

Por condições de pertinência, para \(x\) arbitrário,

\[
\begin{aligned}
x\in E
&\iff(x\in S)\land\neg\bigl((x\in R)\land(x\in D)\bigr)\\
&\iff(x\in S)\land\bigl((x\notin R)\lor(x\notin D)\bigr)\\
&\iff\bigl((x\in S)\land(x\notin R)\bigr)
\lor\bigl((x\in S)\land(x\notin D)\bigr)\\
&\iff x\in(S\setminus R)\cup(S\setminus D).
\end{aligned}
\]

Portanto,

\[
\boxed{E=(S\setminus R)\cup(S\setminus D)}.
\]

Basta faltar uma das condições para a pessoa inscrita receber o aviso; podem faltar ambas.

**b)** A expressão do programador não é adequada em geral. Considere uma pessoa com

\[
x\in S,\qquad x\in R,\qquad x\notin D.
\]

Ela deve receber o aviso porque não atende à condição conjunta. Entretanto, \(x\in R\cup D\), logo \(x\notin S\setminus(R\cup D)\). A expressão incorreta seleciona apenas as pessoas inscritas que estão fora de \(R\) **e** fora de \(D\), excluindo quem tem apenas uma pendência.

Também refuta a expressão a combinação \(x\in S\), \(x\notin R\) e \(x\in D\). Um registro concreto possível para a primeira combinação é \(U=S=R=\{x\}\) e \(D=\varnothing\).

**c)** Sob \(S\subseteq R\), todo elemento de \(S\) já satisfaz a regularidade do cadastro. A única condição que pode faltar é a documentação. Para \(x\) arbitrário,

\[
\begin{aligned}
x\in E
&\iff(x\in S)\land\neg\bigl((x\in R)\land(x\in D)\bigr)\\
&\iff(x\in S)\land(x\notin D)\\
&\iff x\in S\setminus D.
\end{aligned}
\]

Na segunda equivalência, quando \(x\in S\), a pertinência a \(R\) está garantida pela hipótese; quando \(x\notin S\), ambas as condições compostas são falsas. Portanto,

\[
\boxed{E=S\setminus D}.
\]

Também é válida a simplificação \((S\setminus R)\cup(S\setminus D)=\varnothing\cup(S\setminus D)\), pois \(S\subseteq R\).

---

### 24. Reconstruir, verificar e decidir se os dados são possíveis

**a)** Se existe \(A\) com as propriedades dadas, sua decomposição fornece

\[
A=(A\cap B)\cup(A\setminus B)=\boxed{P\cup Q}.
\]

Para justificar a decomposição, tome \(x\in A\) arbitrário. Ele pertence a \(B\) ou não pertence a \(B\); logo, pertence a \(A\cap B=P\) ou a \(A\setminus B=Q\). Isso mostra \(A\subseteq P\cup Q\). Reciprocamente, \(P=A\cap B\subseteq A\) e \(Q=A\setminus B\subseteq A\), portanto \(P\cup Q\subseteq A\). A dupla inclusão estabelece a igualdade. Consequentemente, não pode haver duas soluções diferentes para os mesmos dados.

**b)** A construção não funciona para dados arbitrários. As condições necessárias e suficientes são

\[
\boxed{P\subseteq B\qquad\text{e}\qquad Q\cap B=\varnothing}.
\]

**Necessidade.** Se existe uma solução, temos \(P=A\cap B\), de modo que todo elemento de \(P\) pertence a \(B\). Assim, \(P\subseteq B\). Além disso, \(Q=A\setminus B\); todo elemento de \(Q\) está fora de \(B\). Logo, \(Q\cap B=\varnothing\).

**Suficiência.** Suponha agora essas duas condições e defina \(A=P\cup Q\). Vamos conferir separadamente os dois requisitos.

Se \(x\in A\cap B\), então \(x\in P\cup Q\) e \(x\in B\). Ele não pode pertencer a \(Q\), pois \(Q\cap B=\varnothing\). Portanto, \(x\in P\). Reciprocamente, se \(x\in P\), então \(x\in A\) e, por \(P\subseteq B\), também \(x\in B\). Logo, \(x\in A\cap B\). Assim,

\[
A\cap B=P.
\]

Se \(x\in A\setminus B\), então \(x\in P\cup Q\) e \(x\notin B\). Ele não pode pertencer a \(P\), pois \(P\subseteq B\). Portanto, \(x\in Q\). Reciprocamente, se \(x\in Q\), então \(x\in A\) e, por \(Q\cap B=\varnothing\), \(x\notin B\). Logo, \(x\in A\setminus B\). Portanto,

\[
A\setminus B=Q.
\]

As condições são suficientes e, pelo item a, a solução é única. Não é preciso acrescentar a condição \(P\cap Q=\varnothing\): ela já decorre de \(P\subseteq B\) e \(Q\cap B=\varnothing\).

**c) Registro I.** Temos \(\{b\}\subseteq\{b,d\}\) e \(\{a,c\}\cap\{b,d\}=\varnothing\). As condições são satisfeitas, e

\[
\boxed{A=\{a,b,c\}}.
\]

De fato, \(A\cap B=\{b\}=P\) e \(A\setminus B=\{a,c\}=Q\).

**Registro II.** O elemento \(d\) pertence a \(Q\) e a \(B\), logo \(Q\cap B\neq\varnothing\). Não existe solução: se \(Q=A\setminus B\), nenhum elemento de \(Q\) poderia pertencer a \(B\). Tomar apenas \(A=P\cup Q=\{a,b,d\}\) não corrige os dados, pois nesse caso \(A\cap B=\{b,d\}\neq P\) e \(A\setminus B=\{a\}\neq Q\).

Uma resposta alternativa é suficiente se prova a reconstrução, justifica a necessidade e a suficiência das condições e resolve os dois registros. A enumeração dos registros particulares, sozinha, não demonstra o resultado geral do item b.


