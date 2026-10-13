# BLOCO IV — CARDINALIDADE FINITA E CONTAGEM

## TEXTO PRÁTICO — VERSÃO DEFINITIVA

**Plano de Estudo Matemático 4.0 · Tópico 1.2 — Teoria dos Conjuntos**

Todos os conjuntos considerados nas atividades são finitos. Os complementos e as regiões externas devem ser tomados no universo indicado em cada situação.

---

# 1. Cardinalidade e Relações entre Conjuntos

### 1. Quantos objetos distintos?

Considere

\[
A=\{2,2,5,7,5\},\qquad E=\varnothing,\qquad F=\{\varnothing\},
\]

\[
G=\{1,\{1\},\varnothing,\{1\},\{\varnothing\}\}.
\]

a) Determine \(|A|\), \(|E|\), \(|F|\) e \(|G|\).

b) Identifique os elementos distintos que pertencem diretamente a \(G\) e explique por que \(\varnothing\) e \(\{\varnothing\}\) não devem ser contados como o mesmo objeto.

---

### 2. A quantidade não identifica os elementos

Considere

\[
D=\{1,2,3,4,5,6,7,8,9\},
\]

\[
P=\{x\in D\mid x<5\},\qquad Q=\{x\in D\mid x>5\}.
\]

a) Determine \(P\), \(Q\), \(|P|\) e \(|Q|\).

b) Decida se \(P=Q\). Justifique sua resposta por pertinência, mesmo que as cardinalidades coincidam.

c) O número que expressa \(|Q|\) pertence necessariamente a \(Q\)? Responda examinando este caso.

---

### 3. Quais implicações são válidas?

Avalie as afirmações abaixo para conjuntos finitos arbitrários \(A\) e \(B\). Justifique as válidas e refute as inválidas com conjuntos concretos.

\[
\text{I. }A=B\implies |A|=|B|;
\]

\[
\text{II. }|A|=|B|\implies A=B;
\]

\[
\text{III. }|A|<|B|\implies A\subseteq B;
\]

\[
\text{IV. }A\subseteq B\text{ e }|A|=|B|\implies A=B.
\]

Nos contraexemplos, confira a hipótese numérica e indique uma relação de pertinência que contradiga a conclusão.

---

### 4. Contar sob uma hipótese de inclusão

Sabe-se que \(A\subseteq B\) e \(|A|=7\).

a) Se \(|B|=11\), determine \(|B\setminus A|\). Justifique utilizando uma decomposição de \(B\) em partes disjuntas.

b) Se, em outro caso, \(|B|=7\), o que se pode concluir sobre a relação entre \(A\) e \(B\)? Justifique.

c) É possível manter \(A\subseteq B\) e \(|A|=7\) com \(|B|=6\)? Explique.

---

### 5. Uma decomposição sem sobreposições

Um conjunto \(S\) é a união de três partes \(P\), \(Q\) e \(R\), disjuntas duas a duas. Sabe-se que

\[
|S|=19,\qquad |P|=6,\qquad |Q|=8.
\]

a) Determine \(|R|\).

b) Explique por que a soma das cardinalidades das três partes conta cada elemento de \(S\) exatamente uma vez. Identifique o papel da disjunção e o papel da igualdade \(S=P\cup Q\cup R\).

---

### 6. Duas maneiras de uma contagem falhar

Analise separadamente as situações.

**Situação I.** Um estudante sabe apenas que \(S=P\cup Q\) e conclui que \(|S|=|P|+|Q|\).

a) A conclusão é garantida? Construa um exemplo com \(P\cap Q\neq\varnothing\) e confira a contagem que refuta o argumento.

**Situação II.** Sabe-se que \(P,Q\subseteq S\), \(P\cap Q=\varnothing\), \(|P|=3\), \(|Q|=4\) e \(|S|=10\). Outro estudante conclui que \(|S|=7\).

b) Localize a informação que falta para justificar essa conclusão e determine quantos elementos de \(S\) ficam fora de \(P\cup Q\).

c) Compare os dois erros: em qual situação podem ocorrer contagens repetidas e em qual situação a contagem omite elementos?

---

# 2. Uniões, Diferenças e Complementos: Contagem de Dois Conjuntos

### 7. Dos elementos às quantidades

Considere

\[
U=\{1,2,3,4,5,6,7,8,9,10\},
\]

\[
A=\{1,2,3,4,5,6\},\qquad B=\{4,5,6,7,8\}.
\]

a) Determine as cardinalidades de \(A\cap B\), \(A\cup B\), \(A\setminus B\), \(B\setminus A\) e \(U\setminus(A\cup B)\).

b) Compare \(|A|+|B|\) com \(|A\cup B|\). Identifique os elementos responsáveis pela diferença entre os resultados.

c) Confira \(|U|\) somando as quantidades das quatro regiões disjuntas: somente \(A\), ambos, somente \(B\) e nenhum.

---

### 8. Duas línguas e uma pesquisa

*Baseada/adaptada de Iezzi e Murakami, Fundamentos de Matemática Elementar, vol. 1, cap. II, exercício 52, p. 36.*

Uma pesquisa considera todos os \(80\) estudantes de uma turma ampliada. Entre eles, \(46\) estudam inglês, \(35\) estudam francês e \(17\) estudam ambas as línguas. Denote por \(U\) o conjunto dos estudantes pesquisados, por \(I\) os que estudam inglês e por \(F\) os que estudam francês.

a) Determine quantos estudam somente inglês e quantos estudam somente francês.

b) Determine quantos estudam pelo menos uma dessas línguas e quantos não estudam nenhuma delas.

c) Determine quantos estudam exatamente uma das duas línguas. Represente essa seleção por operações entre \(I\) e \(F\), sem introduzir uma nova operação.

d) Apresente uma verificação de que sua distribuição abrange os \(80\) estudantes sem repetição.

---

### 9. Reconstruindo a parte comum

Em um universo \(U\) com \(60\) elementos, dois subconjuntos \(A\) e \(B\) satisfazem

\[
|A|=34,\qquad |B|=29,\qquad |U\setminus(A\cup B)|=12.
\]

a) Determine \(|A\cup B|\) e \(|A\cap B|\).

b) Determine as quantidades dos elementos que pertencem somente a \(A\) e somente a \(B\).

c) Compare as quantidades de elementos que **não pertencem a nenhum dos dois conjuntos** e que **não pertencem aos dois simultaneamente**. Represente as duas seleções em relação a \(U\) e explique a diferença.

---

### 10. O que se retira do primeiro conjunto?

Sabe-se que

\[
|A|=14,\qquad |B|=9,\qquad |A\cap B|=4.
\]

a) Determine \(|A\setminus B|\) e \(|B\setminus A|\).

b) Um estudante calcula \(|A\setminus B|=14-9=5\). Explique por que o cálculo não corresponde à diferença dada e corrija o procedimento.

c) Sob que relação de inclusão entre \(A\) e \(B\) a expressão \(|A|-|B|\) seria uma maneira válida de calcular \(|A\setminus B|\)? Justifique.

---

### 11. A referência muda a quantidade externa

Considere universos finitos \(U\subseteq V\), com

\[
|U|=36,\qquad |V|=41,
\]

e o mesmo conjunto \(A\subseteq U\), com \(|A|=14\).

a) Determine \(|U\setminus A|\) e \(|V\setminus A|\).

b) Determine \(|V\setminus U|\) e explique como seus elementos participam da diferença entre as respostas do item a.

c) Uma anotação registra apenas “\(|A^c|=22\)”. Qual referência deve acompanhar a anotação para que ela descreva corretamente um dos resultados desta atividade?

---

### 12. Justificando a correção da dupla contagem

*Baseada/adaptada de Iezzi e Murakami, Fundamentos de Matemática Elementar, vol. 1, cap. II, exercício 48, p. 36.*

Sejam \(A\) e \(B\) conjuntos finitos arbitrários. Considere as três regiões

\[
P=A\setminus B,\qquad Q=A\cap B,\qquad R=B\setminus A.
\]

a) Escreva \(A\), \(B\) e \(A\cup B\) como uniões das regiões indicadas. Justifique por que a aditividade das cardinalidades pode ser aplicada a essas decomposições.

b) Compare \(|A|+|B|\) com \(|A\cup B|\) e obtenha uma igualdade que determine a cardinalidade da união.

c) Explique o que essa igualdade fornece se \(A\cap B=\varnothing\) e se \(A\subseteq B\). A demonstração continua válida nesses casos?

---

# 3. Contagem com Três Conjuntos e Sobreposições

### 13. Quantas vezes cada elemento é contado?

*Baseada/adaptada de Iezzi e Murakami, Fundamentos de Matemática Elementar, vol. 1, cap. II, exercício 50, p. 36.*

Sejam \(A\), \(B\) e \(C\) conjuntos finitos. Para um elemento fixo, complete a tabela indicando sua contribuição a cada contagem. A última coluna corresponde à primeira contagem menos a segunda.

| Situação do elemento | Em \(\lvert A\rvert+\lvert B\rvert+\lvert C\rvert\) | Em \(\lvert A\cap B\rvert+\lvert A\cap C\rvert+\lvert B\cap C\rvert\) | Saldo após as subtrações |
|---|---|---|---|
| Não pertence a nenhum dos três |  |  |  |
| Pertence a exatamente um |  |  |  |
| Pertence a exatamente dois |  |  |  |
| Pertence aos três |  |  |  |

a) Qual parcela deve ser acrescentada para que todos os elementos da união contribuam exatamente uma vez? Justifique pela tabela.

b) Escreva e justifique a fórmula resultante para \(|A\cup B\cup C|\), incluindo a hipótese de finitude.

---

### 14. Lendo quantidades em um diagrama

No diagrama, cada número indica a **quantidade de elementos da região em que está escrito**, e não o nome de um elemento. Os conjuntos \(A\), \(B\) e \(C\) estão incluídos no universo \(U\). As áreas não representam proporções quantitativas.

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 620 460" width="620" height="460" role="img" aria-label="Universo U com três conjuntos A, B e C. Cada número indica a quantidade de elementos de uma região disjunta.">
<rect x="20" y="20" width="580" height="420" rx="2" fill="white" stroke="#263341" stroke-width="2"/>
<g fill="none" stroke="#263341" stroke-width="2.2">
<circle cx="240" cy="180" r="130"/>
<circle cx="390" cy="180" r="130"/>
<circle cx="315" cy="295" r="130"/>
</g>
<g font-family="Arial, sans-serif" font-size="23" fill="#18232d" text-anchor="middle">
<text x="42" y="49">U</text>
<text x="202" y="78">A</text>
<text x="429" y="78">B</text>
<text x="315" y="417">C</text>
<text x="165" y="185">6</text>
<text x="465" y="185">5</text>
<text x="315" y="370">4</text>
<text x="315" y="125">3</text>
<text x="230" y="277">2</text>
<text x="400" y="277">1</text>
<text x="315" y="229">2</text>
<text x="72" y="395">7</text>
</g>
</svg>

a) Determine \(|A|\), \(|B|\), \(|C|\) e as cardinalidades das três interseções duplas. Compare \(|A\cap B|\) com \(|(A\cap B)\setminus C|\).

b) Determine quantos elementos pertencem a exatamente um conjunto, a exatamente dois, aos três, a pelo menos um e a nenhum deles.

c) Determine \(|U|\) e confira a cardinalidade da união pela inclusão-exclusão.

---

### 15. Dos totais às regiões exclusivas

Em um universo \(U\), com \(|U|=70\), os subconjuntos \(A\), \(B\) e \(C\) satisfazem:

\[
|A|=32,\qquad |B|=28,\qquad |C|=24,
\]

\[
|A\cap B|=12,\qquad |A\cap C|=10,\qquad |B\cap C|=8,
\]

\[
|A\cap B\cap C|=4.
\]

As interseções duplas dadas incluem os elementos pertencentes aos três conjuntos.

a) Construa um diagrama de Venn e determine a quantidade em cada uma das sete regiões interiores e na região externa.

b) Determine quantos elementos pertencem a exatamente dois conjuntos e quantos pertencem a pelo menos dois.

c) Apresente uma conferência que recupere as cardinalidades individuais e o total de \(U\) a partir das regiões reconstruídas.

---

### 16. A sobreposição tripla está escondida

Uma pesquisa considera um universo \(U\) de \(80\) pessoas. Para três conjuntos \(A,B,C\subseteq U\), os registros fornecem

\[
|A|=35,\qquad |B|=32,\qquad |C|=28,
\]

\[
|A\cap B|=15,\qquad |A\cap C|=12,\qquad |B\cap C|=9.
\]

Além disso, \(16\) pessoas não pertencem a nenhum dos três conjuntos. As interseções duplas são completas, incluindo quem pertence aos três.

a) Determine \(|A\cap B\cap C|\), explicando como a informação sobre a região externa participa do cálculo.

b) Determine quantas pessoas pertencem somente a \(C\) e quantas pertencem a exatamente dois conjuntos.

c) Confira se as regiões interiores reconstruídas somam a cardinalidade da união obtida no item a.

---

### 17. Contar uma região composta com os dados disponíveis

*Baseada/adaptada de Matemática para o Ensino Médio, vol. I, cap. II, exercício de revisão 24, p. 93.*

Sejam \(A\), \(B\) e \(C\) conjuntos finitos com

\[
|A\cap B|=12,\qquad |A\cap C|=9,\qquad |A\cap B\cap C|=4.
\]

a) Determine \(|A\cap(B\cup C)|\). Justifique usando operações e uma contagem adequada, sem supor cardinalidades de \(A\), \(B\) ou \(C\) que não foram fornecidas.

b) Qual região seria contada duas vezes se as duas primeiras quantidades fossem simplesmente somadas?

---

### 18. “Somente os dois” não significa a interseção inteira

Uma pesquisa registra as quantidades abaixo para \(A,B,C\subseteq U\):

| Região | Quantidade |
|---|---:|
| Somente \(A\) | 7 |
| Somente \(B\) | 8 |
| Somente \(C\) | 9 |
| \(A\) e \(B\), mas não \(C\) | 6 |
| \(A\) e \(C\), mas não \(B\) | 4 |
| \(B\) e \(C\), mas não \(A\) | 5 |
| Os três conjuntos | 3 |
| Nenhum dos três | 2 |

Um estudante determina corretamente \(|A|=20\), \(|B|=22\) e \(|C|=21\), mas calcula

\[
|A\cup B\cup C|=20+22+21-6-4-5+3=51.
\]

a) Determine as cardinalidades das interseções completas \(A\cap B\), \(A\cap C\) e \(B\cap C\).

b) Localize o erro no cálculo apresentado e obtenha a cardinalidade correta da união.

c) No cálculo incorreto, quantas vezes cada elemento da interseção tripla acaba contado? Use essa informação para explicar a diferença entre \(51\) e o resultado correto.

---

### 19. Seleções em um catálogo de veículos

*Baseada/adaptada de OpenStax, Contemporary Mathematics, seção 1.5, exercício 30, p. 50.*

Uma concessionária registra os \(31\) veículos de um modelo vendidos em determinado mês. Cada veículo pode incluir os pacotes de entretenimento \(E\), reboque \(R\) e esportivo \(S\). No universo \(U\) desses veículos,

\[
|E|=18,\qquad |R|=11,\qquad |S|=16,
\]

\[
|E\cap R|=8,\qquad |E\cap S|=11,\qquad |R\cap S|=7,
\]

\[
|E\cap R\cap S|=5.
\]

As interseções duplas incluem os veículos com os três pacotes. Há veículos sem nenhum dos pacotes.

Para cada seleção abaixo, represente o conjunto por operações e determine sua cardinalidade. Organize os dados como considerar adequado e apresente uma verificação de sua contagem.

a) Veículos com exatamente dois pacotes.

b) Veículos com entretenimento ou pacote esportivo, mas sem reboque.

c) Veículos sem nenhum dos três pacotes.

d) Veículos com reboque, mas sem pacote esportivo, independentemente de possuírem entretenimento.

---

# 4. Integração, Consistência e Transferência

### 20. A união está determinada?

Sabe-se apenas que \(A,B\subseteq U\), \(|U|=6\), \(|A|=3\) e \(|B|=4\).

a) É possível determinar uma única cardinalidade para \(A\cup B\)? Sustente sua resposta construindo dois pares de conjuntos, no mesmo universo, que respeitem os dados e produzam resultados diferentes.

b) Determine todos os valores possíveis de \(|A\cup B|\). Justifique por que não há outros e apresente uma configuração para cada valor indicado.

c) Indique uma informação numérica adicional que permita determinar a cardinalidade da união e explique como ela seria utilizada.

---

### 21. Um relatório cabe no universo?

*Baseada/adaptada de Matemática para o Ensino Médio, vol. I, cap. II, exercício de revisão 19, p. 92.*

Uma pesquisa considera exatamente \(40\) participantes. O relatório afirma que \(28\) participam da atividade \(A\), \(24\) participam da atividade \(B\) e \(9\) participam de ambas. Denote por \(U\) o conjunto dos participantes pesquisados.

a) Verifique se essas informações são compatíveis. Identifique a relação quantitativa que falha.

b) Suponha que apenas o registro de quem participa de ambas possa estar errado. Mantendo os outros dados, determine todos os valores inteiros que esse registro pode assumir para tornar a pesquisa possível.

c) Escolha o menor desses valores e reconstrua as quatro regiões de \(U\), conferindo o total de participantes.

---

### 22. Uma união plausível pode esconder dados impossíveis

Um relatório propõe \(A,B,C\subseteq U\), com \(|U|=30\), e fornece

\[
|A|=10,\qquad |B|=9,\qquad |C|=8,
\]

\[
|A\cap B|=8,\qquad |A\cap C|=7,\qquad |B\cap C|=3,
\]

\[
|A\cap B\cap C|=2.
\]

As interseções duplas são completas.

a) A aplicação da inclusão-exclusão fornece qual valor para a união?

b) Um estudante considera o relatório possível porque esse valor não é negativo e não excede \(|U|\). A justificativa é suficiente? Verifique os dados e apresente uma incompatibilidade concreta, caso exista.

---

### 23. A quantidade precisa ser inteira

Um grupo finito \(U\) foi organizado em três conjuntos \(A,B,C\subseteq U\). Afirma-se que

\[
|A|=|B|=|C|=3
\]

e que cada pessoa de \(U\) pertence a **exatamente dois** dos três conjuntos.

Essa distribuição pode existir? Justifique examinando quantas vezes cada pessoa é contada na soma \(|A|+|B|+|C|\). Se a distribuição for possível, apresente uma realização; se não for, identifique a contradição.

---

### 24. Conhecer todas as interseções duplas basta?

Em um universo \(U\) com \(|U|=8\), são propostos três subconjuntos \(A\), \(B\) e \(C\), com

\[
|A|=|B|=|C|=4,
\]

\[
|A\cap B|=|A\cap C|=|B\cap C|=2.
\]

Não foi informada a cardinalidade da interseção tripla. As interseções duplas são completas.

a) A cardinalidade da união está determinada? Apresente duas distribuições pelas regiões disjuntas que respeitem todos os dados, mas produzam respostas diferentes.

b) Determine todos os valores possíveis para a interseção tripla, para a união e para a região externa. Justifique a possibilidade de cada distribuição e a exclusão de outros valores.

c) Se uma verificação adicional revelar exatamente um elemento fora dos três conjuntos, determine a distribuição completa pelas oito regiões de \(U\).

---

### 25. Uma inclusão pode reduzir o trabalho

Um centro cultural registra um universo \(U\) de \(50\) participantes e três conjuntos de inscrições \(A\), \(B\) e \(C\). Sabe-se que

\[
|A|=26,\qquad |B|=20,\qquad |C|=8,
\]

\[
|A\cap B|=10,\qquad |A\cap C|=5,
\]

e que toda pessoa inscrita em \(C\) também está inscrita em \(B\): \(C\subseteq B\).

a) Um aviso deve ser enviado exatamente a quem está inscrito em \(A\) ou em \(C\), mas não em \(B\). Represente a seleção e determine quantas pessoas recebem o aviso.

b) Determine quantas pessoas estão inscritas nos três conjuntos.

c) Determine quantas não estão inscritas em nenhum dos três.

Escolha uma estratégia e justifique em que passagens utiliza a inclusão dada.

---

### 26. Reconstruindo um registro incompleto

Uma pesquisa considera \(60\) pessoas, das quais \(8\) não pertencem a nenhum dos três conjuntos \(A\), \(B\) e \(C\). O registro contém

\[
|A|=30,\qquad |B|=26,\qquad |C|=22,
\]

e as seguintes quantidades **exclusivamente duplas**:

\[
|(A\cap B)\setminus C|=6,
\]

\[
|(A\cap C)\setminus B|=4,
\]

\[
|(B\cap C)\setminus A|=10.
\]

a) Determine quantas pessoas pertencem aos três conjuntos. Justifique a relação quantitativa utilizada para reconstruir essa informação.

b) Determine as quantidades em todas as regiões disjuntas do universo e confira todos os dados do registro.

c) Determine quantas pessoas pertencem a \((A\cup B)\setminus C\) e quantas pertencem a \(A\cap(B\cup C)\). Justifique selecionando as regiões correspondentes.

---

# GABARITO COMENTADO

# 1. Cardinalidade e Relações entre Conjuntos

### 1. Quantos objetos distintos?

**a)**

\[
\boxed{|A|=3,\qquad |E|=0,\qquad |F|=1,\qquad |G|=4}.
\]

Em \(A\), os elementos distintos são \(2,5,7\); as repetições na escrita não acrescentam elementos. O conjunto \(E\) não possui elementos, enquanto \(F\) possui um elemento: \(\varnothing\).

**b)** Os elementos distintos de \(G\) são

\[
1,\qquad\{1\},\qquad\varnothing,\qquad\{\varnothing\}.
\]

A segunda ocorrência de \(\{1\}\) não altera o conjunto. Já \(\varnothing\) não possui elementos, e \(\{\varnothing\}\) possui um; portanto, são objetos diferentes. A cardinalidade de \(G\) conta esses objetos diretamente, sem reunir os elementos dos conjuntos que aparecem dentro dele.

---

### 2. A quantidade não identifica os elementos

**a)**

\[
P=\{1,2,3,4\},\qquad Q=\{6,7,8,9\},
\]

\[
\boxed{|P|=|Q|=4}.
\]

**b)** \(P\neq Q\). Por exemplo, \(1\in P\) e \(1\notin Q\). A coincidência das quantidades não estabelece a coincidência dos elementos.

**c)** Não. Neste caso, \(|Q|=4\), mas \(4\notin Q\). A cardinalidade informa uma quantidade e não adiciona esse número à coleção.

---

### 3. Quais implicações são válidas?

**I — válida.** Se \(A=B\), os dois conjuntos possuem exatamente os mesmos elementos. Contar os objetos distintos de cada um fornece a mesma quantidade.

**II — inválida.** Tome \(A=\{1,2\}\) e \(B=\{3,4\}\). Temos \(|A|=|B|=2\), mas \(1\in A\) e \(1\notin B\); logo, \(A\neq B\).

**III — inválida.** Tome \(A=\{1\}\) e \(B=\{2,3\}\). A hipótese \(|A|=1<2=|B|\) é satisfeita, mas \(1\in A\) e \(1\notin B\), de modo que \(A\nsubseteq B\).

**IV — válida.** Se \(A\subseteq B\), todos os elementos de \(A\) já estão em \(B\). Se existisse um elemento de \(B\) externo a \(A\), a inclusão seria própria, e a finitude garantiria \(|A|<|B|\), contrariando a hipótese. Portanto, \(A=B\).

Outros contraexemplos são suficientes quando preservam a hipótese e contradizem efetivamente a conclusão.

---

### 4. Contar sob uma hipótese de inclusão

**a)** Como \(A\subseteq B\),

\[
B=A\cup(B\setminus A),\qquad A\cap(B\setminus A)=\varnothing.
\]

Pela aditividade,

\[
11=7+|B\setminus A|,
\qquad
\boxed{|B\setminus A|=4}.
\]

**b)** \(\boxed{A=B}\). A inclusão, junto com a igualdade das cardinalidades finitas, exclui a possibilidade de elementos adicionais em \(B\). Pela mesma decomposição, \(|B\setminus A|=7-7=0\).

**c)** Não. De \(A\subseteq B\) decorre \(|A|\leq|B|\). Os valores propostos exigiriam \(7\leq6\), o que é falso. A hipótese de inclusão não pode ser mantida com essas quantidades.

---

### 5. Uma decomposição sem sobreposições

**a)** Como as três partes são disjuntas e sua união é \(S\),

\[
19=6+8+|R|,
\qquad
\boxed{|R|=5}.
\]

**b)** A disjunção duas a duas garante que um elemento não seja contado em duas parcelas. A igualdade \(S=P\cup Q\cup R\) garante que todo elemento de \(S\) apareça em alguma delas. Assim, não há duplicações nem omissões.

---

### 6. Duas maneiras de uma contagem falhar

**a)** A conclusão não é garantida. Tome

\[
P=\{a,b\},\qquad Q=\{b,c\},\qquad S=\{a,b,c\}.
\]

Temos \(S=P\cup Q\), mas \(|P|+|Q|=2+2=4\) e \(|S|=3\). O elemento \(b\) foi contado duas vezes na soma. Falta a hipótese de disjunção para justificar a adição sem correção.

**b)** A disjunção fornece \(|P\cup Q|=3+4=7\), mas não foi dada a igualdade \(S=P\cup Q\). Como a união é um subconjunto de \(S\),

\[
\boxed{|S\setminus(P\cup Q)|=10-7=3}.
\]

**c)** Na Situação I, a cobertura é conhecida, mas a sobreposição pode provocar duplicações. Na Situação II, não há sobreposição entre as partes, mas existem elementos de \(S\) que não foram incluídos na soma. As condições de cobertura e disjunção realizam funções diferentes.

---

# 2. Uniões, Diferenças e Complementos: Contagem de Dois Conjuntos

### 7. Dos elementos às quantidades

**a)**

| Conjunto | Elementos | Cardinalidade |
|---|---|---:|
| \(A\cap B\) | \(\{4,5,6\}\) | 3 |
| \(A\cup B\) | \(\{1,2,3,4,5,6,7,8\}\) | 8 |
| \(A\setminus B\) | \(\{1,2,3\}\) | 3 |
| \(B\setminus A\) | \(\{7,8\}\) | 2 |
| \(U\setminus(A\cup B)\) | \(\{9,10\}\) | 2 |

**b)** \(|A|+|B|=6+5=11\), enquanto \(|A\cup B|=8\). Os elementos \(4,5,6\) aparecem nas duas contagens individuais. Retirando uma ocorrência de cada um, obtemos \(11-3=8\).

**c)** As quatro regiões têm cardinalidades \(3,3,2,2\). Sua soma é \(3+3+2+2=10=|U|\), sem elementos comuns entre parcelas distintas.

---

### 8. Duas línguas e uma pesquisa

**a)** Somente inglês:

\[
\boxed{|I\setminus F|=46-17=29}.
\]

Somente francês:

\[
\boxed{|F\setminus I|=35-17=18}.
\]

**b)** Pelo menos uma língua:

\[
\boxed{|I\cup F|=46+35-17=64}.
\]

Nenhuma das duas:

\[
\boxed{|U\setminus(I\cup F)|=80-64=16}.
\]

**c)** A seleção é

\[
(I\setminus F)\cup(F\setminus I).
\]

As duas parcelas são disjuntas, pois a primeira exige pertencer a \(I\) e não a \(F\), enquanto a segunda exige o contrário. Portanto, a quantidade é \(\boxed{29+18=47}\).

**d)** A distribuição é \(29\) somente em inglês, \(17\) em ambas, \(18\) somente em francês e \(16\) em nenhuma. A soma \(29+17+18+16=80\) abrange o universo. Também recuperamos \(29+17=46\) e \(18+17=35\), conferindo as cardinalidades individuais.

---

### 9. Reconstruindo a parte comum

**a)** A união e sua região externa decompõem \(U\). Logo,

\[
\boxed{|A\cup B|=60-12=48}.
\]

Reorganizando a inclusão-exclusão,

\[
\boxed{|A\cap B|=34+29-48=15}.
\]

**b)** Somente \(A\): \(\boxed{34-15=19}\). Somente \(B\): \(\boxed{29-15=14}\).

**c)** Não pertencer a nenhum dos conjuntos significa pertencer a

\[
U\setminus(A\cup B),
\]

com \(\boxed{12}\) elementos. Não pertencer aos dois simultaneamente significa pertencer a

\[
U\setminus(A\cap B),
\]

com \(\boxed{60-15=45}\) elementos. Esta última seleção inclui quem está somente em \(A\), somente em \(B\) ou fora de ambos: \(19+14+12=45\). A primeira inclui apenas a região externa à união.

---

### 10. O que se retira do primeiro conjunto?

**a)**

\[
\boxed{|A\setminus B|=14-4=10},
\qquad
\boxed{|B\setminus A|=9-4=5}.
\]

**b)** De \(A\), devem ser retirados apenas seus elementos que também pertencem a \(B\), isto é, os \(4\) elementos de \(A\cap B\). Os demais \(5\) elementos de \(B\) já estão fora de \(A\) e não podem ser retirados de sua contagem. O procedimento correto é \(14-4=10\).

**c)** A relação é \(\boxed{B\subseteq A}\). Sob essa hipótese, \(A\cap B=B\), e portanto

\[
|A\setminus B|=|A|-|A\cap B|=|A|-|B|.
\]

A hipótese não se verifica nos dados iniciais, pois a interseção tem \(4\) elementos e \(B\) tem \(9\).

---

### 11. A referência muda a quantidade externa

**a)**

\[
\boxed{|U\setminus A|=36-14=22},
\qquad
\boxed{|V\setminus A|=41-14=27}.
\]

**b)** Como \(U\subseteq V\),

\[
\boxed{|V\setminus U|=41-36=5}.
\]

Esses elementos estão fora de \(A\), pois \(A\subseteq U\). A decomposição

\[
V\setminus A=(U\setminus A)\cup(V\setminus U)
\]

é disjunta: a primeira parcela está em \(U\), e a segunda está fora dele. Assim, o complemento em \(V\) tem os \(22\) elementos do complemento em \(U\), acrescidos dos \(5\) novos elementos da referência.

**c)** A anotação deve informar que o complemento é relativo a \(\boxed{U}\). A escrita explícita \(|U\setminus A|=22\) também elimina a ambiguidade.

---

### 12. Justificando a correção da dupla contagem

**a)** As decomposições são

\[
A=P\cup Q,\qquad B=Q\cup R,\qquad A\cup B=P\cup Q\cup R.
\]

As regiões \(P,Q,R\) são disjuntas duas a duas. Por exemplo, \(P\) exige não pertencer a \(B\), enquanto \(Q\) exige pertencer a \(B\); \(R\) exige não pertencer a \(A\), enquanto \(P\) e \(Q\) estão em \(A\). A finitude e a ausência de sobreposições legitimam a aditividade.

**b)** Temos

\[
|A|=|P|+|Q|,\qquad |B|=|Q|+|R|,
\]

\[
|A\cup B|=|P|+|Q|+|R|.
\]

Consequentemente,

\[
|A|+|B|=|P|+2|Q|+|R|=|A\cup B|+|Q|.
\]

Como \(Q=A\cap B\),

\[
\boxed{|A\cup B|=|A|+|B|-|A\cap B|}.
\]

A parcela subtraída corrige exatamente a ocorrência adicional dos elementos comuns. A demonstração vale para quaisquer conjuntos finitos, e não apenas para uma enumeração escolhida.

**c)** Se \(A\cap B=\varnothing\), sua cardinalidade é zero, e obtemos \(|A\cup B|=|A|+|B|-0\). Se \(A\subseteq B\), temos \(A\cap B=A\) e \(A\cup B=B\); a fórmula fornece \(|A|+|B|-|A|=|B|\). Regiões vazias não invalidam a decomposição nem a aditividade, portanto a demonstração permanece válida.

---

# 3. Contagem com Três Conjuntos e Sobreposições

### 13. Quantas vezes cada elemento é contado?

| Situação do elemento | Na soma individual | Na soma das interseções duplas | Saldo após as subtrações |
|---|---:|---:|---:|
| Nenhum dos três | 0 | 0 | 0 |
| Exatamente um | 1 | 0 | 1 |
| Exatamente dois | 2 | 1 | 1 |
| Os três | 3 | 3 | 0 |

**a)** Deve-se acrescentar \(\boxed{|A\cap B\cap C|}\). Um elemento dos três conjuntos aparece nas três parcelas individuais e nas três interseções duplas. Depois das subtrações, seu saldo é \(3-3=0\). A adição final recupera uma ocorrência. Os demais elementos não pertencem à interseção tripla e não têm sua contribuição alterada por essa adição.

**b)** Para conjuntos finitos \(A,B,C\),

\[
\boxed{
\begin{aligned}
|A\cup B\cup C|
={}&|A|+|B|+|C|\\
&-|A\cap B|-|A\cap C|-|B\cap C|\\
&+|A\cap B\cap C|.
\end{aligned}}
\]

A tabela abrange todas as possibilidades de pertinência quanto à quantidade de conjuntos que contêm um elemento. Na expressão final, cada elemento da união contribui exatamente uma vez; um elemento externo contribui zero. Como os conjuntos são finitos, essa conferência das contribuições estabelece a igualdade das contagens. Não se pressupõe que todas as regiões contenham elementos.

---

### 14. Lendo quantidades em um diagrama

**a)** Somando as regiões que constituem cada conjunto,

\[
\boxed{|A|=6+3+2+2=13},
\]

\[
\boxed{|B|=5+3+1+2=11},
\]

\[
\boxed{|C|=4+2+1+2=9}.
\]

As interseções completas incluem a região central:

\[
\boxed{|A\cap B|=3+2=5},\qquad
\boxed{|A\cap C|=2+2=4},\qquad
\boxed{|B\cap C|=1+2=3}.
\]

Já \(\boxed{|(A\cap B)\setminus C|=3}\). A diferença entre \(5\) e \(3\) corresponde aos dois elementos que também pertencem a \(C\).

**b)**

| Seleção | Quantidade |
|---|---:|
| Exatamente um conjunto | \(6+5+4=15\) |
| Exatamente dois conjuntos | \(3+2+1=6\) |
| Os três conjuntos | 2 |
| Pelo menos um conjunto | \(15+6+2=23\) |
| Nenhum dos três | 7 |

As parcelas de cada soma são regiões disjuntas. Em particular, o centro não entra na contagem de exatamente dois.

**c)** \(\boxed{|U|=23+7=30}\). Pela inclusão-exclusão,

\[
|A\cup B\cup C|=13+11+9-5-4-3+2=\boxed{23},
\]

confirmando a soma direta das sete regiões interiores.

---

### 15. Dos totais às regiões exclusivas

**a)** Começando pela região tripla, as regiões exclusivamente duplas são

\[
12-4=8,\qquad 10-4=6,\qquad 8-4=4.
\]

Retirando de cada conjunto as regiões de sobreposição que lhe pertencem, obtemos:

| Região | Quantidade |
|---|---:|
| \(A\setminus(B\cup C)\) | \(32-8-6-4=14\) |
| \(B\setminus(A\cup C)\) | \(28-8-4-4=12\) |
| \(C\setminus(A\cup B)\) | \(24-6-4-4=10\) |
| \((A\cap B)\setminus C\) | 8 |
| \((A\cap C)\setminus B\) | 6 |
| \((B\cap C)\setminus A\) | 4 |
| \(A\cap B\cap C\) | 4 |
| \(U\setminus(A\cup B\cup C)\) | 12 |

A união tem \(14+12+10+8+6+4+4=58\) elementos. A região externa tem \(70-58=12\). O diagrama construído deve posicionar cada quantidade na região indicada, mantendo a referência \(U\). Um diagrama legível com essas informações atende ao comando, sem exigir proporção entre áreas e quantidades.

**b)** Exatamente dois: \(\boxed{8+6+4=18}\). Pelo menos dois: \(\boxed{18+4=22}\). A segunda seleção inclui a interseção tripla, uma única vez.

**c)** As cardinalidades individuais são recuperadas por

\[
14+8+6+4=32,\qquad
12+8+4+4=28,\qquad
10+6+4+4=24.
\]

Também recuperamos as interseções completas: \(8+4=12\), \(6+4=10\) e \(4+4=8\). Todas as regiões têm quantidades inteiras não negativas, e a soma das oito quantidades é \(58+12=70\). A reconstrução é compatível com os dados.

---

### 16. A sobreposição tripla está escondida

**a)** Como \(16\) pessoas estão fora dos três conjuntos,

\[
|A\cup B\cup C|=80-16=64.
\]

Denotando por \(t\) a cardinalidade tripla, a inclusão-exclusão fornece

\[
64=35+32+28-15-12-9+t=59+t.
\]

Portanto, \(\boxed{t=5}\). A informação sobre a região externa permite obter o total da união, necessário para reconstruir a sobreposição desconhecida.

**b)** As regiões exclusivamente duplas têm quantidades \(15-5=10\), \(12-5=7\) e \(9-5=4\). Somente \(C\) contém

\[
\boxed{28-7-4-5=12}
\]

pessoas. Exatamente dois conjuntos contêm \(\boxed{10+7+4=21}\) pessoas.

**c)** Somente \(A\): \(35-10-7-5=13\). Somente \(B\): \(32-10-4-5=13\). As sete regiões interiores somam

\[
13+13+12+10+7+4+5=64.
\]

Acrescentando os \(16\) externos, recuperamos \(80\). A região tripla não foi subtraída duas vezes ao reconstruir as regiões individuais: depois de separar as interseções exclusivamente duplas, ela é retirada uma única vez de cada total.

---

### 17. Contar uma região composta com os dados disponíveis

**a)** Pela distributividade,

\[
A\cap(B\cup C)=(A\cap B)\cup(A\cap C).
\]

Podemos aplicar a inclusão-exclusão a esses dois conjuntos finitos. A interseção entre eles é

\[
(A\cap B)\cap(A\cap C)=A\cap B\cap C.
\]

Assim,

\[
\boxed{|A\cap(B\cup C)|=12+9-4=17}.
\]

Não são necessários os totais de \(A\), \(B\) ou \(C\): os dados fornecidos descrevem precisamente as duas parcelas da união relevante e sua sobreposição.

**b)** A região contada duas vezes seria \(\boxed{A\cap B\cap C}\), com \(4\) elementos. Cada um deles está em \(A\cap B\) e em \(A\cap C\).

---

### 18. “Somente os dois” não significa a interseção inteira

**a)**

\[
\boxed{|A\cap B|=6+3=9},\qquad
\boxed{|A\cap C|=4+3=7},\qquad
\boxed{|B\cap C|=5+3=8}.
\]

**b)** O estudante substituiu as interseções completas pelas regiões exclusivamente duplas. A fórmula exige as primeiras, que também contêm os três elementos da região central. Corrigindo,

\[
|A\cup B\cup C|=20+22+21-9-7-8+3=\boxed{42}.
\]

A soma das sete regiões interiores confirma: \(7+8+9+6+4+5+3=42\). Com os dois elementos externos, \(|U|=44\).

**c)** No cálculo incorreto, cada elemento central aparece três vezes na soma individual, não é retirado pelas parcelas exclusivamente duplas e é acrescentado mais uma vez pela parcela final. Seu saldo é \(3-0+1=4\), quando deveria ser \(1\). São três ocorrências adicionais de cada um dos três elementos centrais, produzindo o excesso \(3\cdot3=9\). Isso explica \(51-42=9\).

---

### 19. Seleções em um catálogo de veículos

Uma organização possível é reconstruir as regiões disjuntas:

| Região | Quantidade |
|---|---:|
| Somente \(E\) | \(18-3-6-5=4\) |
| Somente \(R\) | \(11-3-2-5=1\) |
| Somente \(S\) | \(16-6-2-5=3\) |
| \((E\cap R)\setminus S\) | \(8-5=3\) |
| \((E\cap S)\setminus R\) | \(11-5=6\) |
| \((R\cap S)\setminus E\) | \(7-5=2\) |
| \(E\cap R\cap S\) | 5 |
| Nenhum pacote | 7 |

As regiões interiores somam \(4+1+3+3+6+2+5=24\). Logo, há \(31-24=7\) veículos externos à união.

**a)** Exatamente dois pacotes correspondem a

\[
\bigl((E\cap R)\setminus S\bigr)
\cup\bigl((E\cap S)\setminus R\bigr)
\cup\bigl((R\cap S)\setminus E\bigr).
\]

Essas parcelas são disjuntas e fornecem \(\boxed{3+6+2=11}\) veículos.

**b)** A seleção é \(\boxed{(E\cup S)\setminus R}\). Entram somente \(E\), somente \(S\) e \(E\cap S\) sem \(R\), totalizando \(\boxed{4+3+6=13}\).

**c)** A seleção é \(\boxed{U\setminus(E\cup R\cup S)}\), com \(\boxed{7}\) veículos.

**d)** A seleção é \(\boxed{R\setminus S}\), que inclui somente \(R\) e \(E\cap R\) sem \(S\). São \(\boxed{1+3=4}\) veículos. Também podemos obter \(11-7=4\), retirando de \(R\) a interseção completa com \(S\).

**Verificação.** A soma das oito regiões é \(24+7=31\). Recuperamos os totais individuais por \(4+3+6+5=18\), \(1+3+2+5=11\) e \(3+6+2+5=16\), e os totais das interseções por \(3+5=8\), \(6+5=11\) e \(2+5=7\). Cada seleção foi contada como união de regiões disjuntas. Outras organizações corretas são válidas se preservam esses dados e as condições de cada seleção.

---

# 4. Integração, Consistência e Transferência

### 20. A união está determinada?

**a)** Não. Tome o mesmo universo \(U=\{1,2,3,4,5,6\}\) e \(A=\{1,2,3\}\). Se \(B=\{1,2,3,4\}\), a união tem \(4\) elementos. Se \(B=\{3,4,5,6\}\), tem \(6\). Em ambos os casos, \(|A|=3\) e \(|B|=4\); a sobreposição é diferente.

**b)** Como \(B\subseteq A\cup B\subseteq U\),

\[
4\leq|A\cup B|\leq6.
\]

A cardinalidade é inteira, portanto só pode ser \(4\), \(5\) ou \(6\). Todos esses valores são realizáveis:

| \(A\) | \(B\) | União | Cardinalidade da união |
|---|---|---|---:|
| \(\{1,2,3\}\) | \(\{1,2,3,4\}\) | \(\{1,2,3,4\}\) | 4 |
| \(\{1,2,3\}\) | \(\{2,3,4,5\}\) | \(\{1,2,3,4,5\}\) | 5 |
| \(\{1,2,3\}\) | \(\{3,4,5,6\}\) | \(\{1,2,3,4,5,6\}\) | 6 |

**c)** Uma informação suficiente é \(\boxed{|A\cap B|}\). Conhecendo-a, obtemos \(|A\cup B|=3+4-|A\cap B|\). Também serve conhecer a quantidade externa à união, pois ela pode ser subtraída de \(6\). Outras respostas são válidas quando explicam como a informação adicional determina a quantidade pedida.

---

### 21. Um relatório cabe no universo?

**a)** Os dados são incompatíveis. A soma corrigida produziria

\[
28+24-9=43,
\]

excedendo os \(40\) participantes do universo. Como \(A\cup B\subseteq U\), uma união com \(43\) elementos não pode existir nesse universo. A contagem externa seria \(40-43=-3\), também impossível.

**b)** Denote por \(x\) o registro corrigido da interseção. As quatro regiões precisariam ter as quantidades

\[
28-x,\qquad x,\qquad24-x,\qquad40-(28+24-x)=x-12.
\]

Para que todas sejam inteiras não negativas, é necessário que \(x\geq12\) e \(x\leq24\). Assim, os valores possíveis são

\[
\boxed{x=12,13,14,\ldots,24}.
\]

Essas condições também são suficientes: para qualquer inteiro nesse intervalo, as quatro quantidades são não negativas e somam \(40\). Podemos distribuir os participantes em quatro grupos disjuntos com essas quantidades e definir \(A\) e \(B\) pelas regiões correspondentes. Os totais serão \(28\) e \(24\), com interseção \(x\).

**c)** Para o menor valor, \(x=12\), a distribuição é:

| Região | Quantidade |
|---|---:|
| Somente \(A\) | \(28-12=16\) |
| Ambos | 12 |
| Somente \(B\) | \(24-12=12\) |
| Nenhum | 0 |

A soma é \(16+12+12+0=40\). Recuperamos \(16+12=28\) e \(12+12=24\). Uma região externa vazia é um caso legítimo.

---

### 22. Uma união plausível pode esconder dados impossíveis

**a)** A substituição dos números na expressão da inclusão-exclusão fornece

\[
10+9+8-8-7-3+2=\boxed{11}.
\]

Esse valor formal, isoladamente, não demonstra que os conjuntos descritos possam existir.

**b)** A justificativa é insuficiente, e os dados são incompatíveis. Dentro de \(A\), as regiões exclusivamente duplas deveriam conter \(8-2=6\) elementos em \(A\cap B\) sem \(C\) e \(7-2=5\) em \(A\cap C\) sem \(B\). Acrescentando os dois elementos centrais, já seriam necessários

\[
6+5+2=13
\]

elementos de \(A\), embora \(|A|=10\). A região somente em \(A\) exigiria \(10-13=-3\), o que é impossível.

Equivalentemente,

\[
|A\cap(B\cup C)|=8+7-2=13
\]

contradiz a inclusão \(A\cap(B\cup C)\subseteq A\), que exigiria uma cardinalidade no máximo igual a \(10\). Conferir somente o total da união não garante a não negatividade de todas as regiões.

---

### 23. A quantidade precisa ser inteira

A distribuição não pode existir. A soma das cardinalidades é

\[
|A|+|B|+|C|=3+3+3=9.
\]

Sob a condição proposta, cada pessoa de \(U\) contribui exatamente duas vezes a essa soma. Portanto, seria necessário

\[
2|U|=9,
\qquad |U|=\frac{9}{2}.
\]

Esse resultado não é inteiro. A cardinalidade de um conjunto finito conta pessoas distintas e precisa ser inteira não negativa. A contradição decorre das próprias condições do registro, não de uma preferência por números maiores ou menores.

---

### 24. Conhecer todas as interseções duplas basta?

Denote por \(t=|A\cap B\cap C|\) a quantidade desconhecida. Cada região exclusivamente dupla tem \(2-t\) elementos. Cada região somente em um dos conjuntos tem

\[
4-(2-t)-(2-t)-t=t
\]

elementos. Pela inclusão-exclusão,

\[
|A\cup B\cup C|=4+4+4-2-2-2+t=6+t.
\]

A região externa tem \(8-(6+t)=2-t\) elementos.

**a)** A união não está determinada. Duas distribuições possíveis são dadas pelas colunas \(t=0\) e \(t=2\) da tabela abaixo. Elas produzem uniões com \(6\) e \(8\) elementos, respectivamente, mantendo todos os totais individuais e todas as interseções duplas.

| Região ou total | \(t=0\) | \(t=1\) | \(t=2\) |
|---|---:|---:|---:|
| Somente \(A\) | 0 | 1 | 2 |
| Somente \(B\) | 0 | 1 | 2 |
| Somente \(C\) | 0 | 1 | 2 |
| \(A\cap B\), sem \(C\) | 2 | 1 | 0 |
| \(A\cap C\), sem \(B\) | 2 | 1 | 0 |
| \(B\cap C\), sem \(A\) | 2 | 1 | 0 |
| Os três | 0 | 1 | 2 |
| Nenhum | 2 | 1 | 0 |
| União dos três | 6 | 7 | 8 |

**b)** Como a interseção tripla está incluída em cada interseção dupla, \(0\leq t\leq2\). A cardinalidade é inteira, logo os únicos candidatos são \(\boxed{0,1,2}\). Para cada candidato, a tabela fornece quantidades inteiras não negativas nas oito regiões, somando \(8\). Cada total individual é \(t+(2-t)+(2-t)+t=4\), e cada interseção dupla tem \((2-t)+t=2\). Assim, todas as distribuições são realizáveis, bastando repartir os oito elementos do universo pelas regiões indicadas.

Os valores possíveis da união são \(\boxed{6,7,8}\), com quantidades externas correspondentes \(\boxed{2,1,0}\). Não é válido combinar esses totais independentemente: cada coluna descreve uma distribuição completa.

**c)** Se a região externa contém exatamente um elemento, \(2-t=1\), portanto \(t=1\). A coluna central fornece a distribuição completa: \(\boxed{1}\) elemento em cada uma das oito regiões. A união tem \(7\) elementos.

---

### 25. Uma inclusão pode reduzir o trabalho

**a)** O conjunto selecionado é

\[
E=(A\cup C)\setminus B.
\]

Um elemento selecionado pertence a \(A\) ou a \(C\) e não pertence a \(B\). Como \(C\subseteq B\), ele não pode vir de \(C\) estando fora de \(B\); precisa pertencer a \(A\setminus B\). Reciprocamente, todo elemento de \(A\setminus B\) satisfaz a seleção. Assim,

\[
\boxed{E=A\setminus B},
\qquad
\boxed{|E|=26-10=16}.
\]

**b)** A inclusão \(C\subseteq B\) garante que um elemento comum a \(A\) e \(C\) já pertence também a \(B\). Logo,

\[
A\cap B\cap C=A\cap C,
\qquad
\boxed{|A\cap B\cap C|=5}.
\]

**c)** Como \(C\subseteq B\), reunir \(C\) a \(A\cup B\) não acrescenta elementos:

\[
A\cup B\cup C=A\cup B.
\]

Portanto,

\[
|A\cup B\cup C|=26+20-10=36,
\]

\[
\boxed{|U\setminus(A\cup B\cup C)|=50-36=14}.
\]

É possível reconstruir as regiões, mas a hipótese de inclusão permite resolver as três seleções sem determinar toda a distribuição. Uma solução alternativa é válida se respeita essa hipótese e justifica as contagens pedidas.

---

### 26. Reconstruindo um registro incompleto

**a)** A união contém \(60-8=52\) pessoas. Seja \(t\) a quantidade que pertence aos três conjuntos. As interseções completas têm cardinalidades \(6+t\), \(4+t\) e \(10+t\). Pela inclusão-exclusão,

\[
\begin{aligned}
52&=30+26+22-(6+t)-(4+t)-(10+t)+t\\
&=58-2t.
\end{aligned}
\]

Logo, \(2t=6\) e \(\boxed{t=3}\).

Também podemos comparar diretamente a soma das contagens individuais com a união. A soma \(30+26+22=78\) excede \(52\) em \(26\) ocorrências. As pessoas de regiões exclusivamente duplas geram \(6+4+10=20\) ocorrências adicionais, uma por pessoa. As \(6\) ocorrências adicionais restantes vêm da região tripla, que gera duas por pessoa. Portanto, ela contém \(6\div2=3\) pessoas.

**b)**

| Região | Quantidade |
|---|---:|
| Somente \(A\) | \(30-6-4-3=17\) |
| Somente \(B\) | \(26-6-10-3=7\) |
| Somente \(C\) | \(22-4-10-3=5\) |
| \(A\) e \(B\), sem \(C\) | 6 |
| \(A\) e \(C\), sem \(B\) | 4 |
| \(B\) e \(C\), sem \(A\) | 10 |
| Os três | 3 |
| Nenhum | 8 |

As oito quantidades são inteiras não negativas e somam

\[
17+7+5+6+4+10+3+8=60.
\]

Recuperamos \(|A|=17+6+4+3=30\), \(|B|=7+6+10+3=26\) e \(|C|=5+4+10+3=22\). As regiões exclusivamente duplas coincidem com as quantidades dadas, e a região externa possui \(8\) pessoas. Assim, todos os registros foram conferidos.

**c)** Para pertencer a \((A\cup B)\setminus C\), a pessoa deve estar somente em \(A\), somente em \(B\) ou em \(A\cap B\) sem \(C\). Portanto,

\[
\boxed{|(A\cup B)\setminus C|=17+7+6=30}.
\]

Para pertencer a \(A\cap(B\cup C)\), deve estar em \(A\cap B\) sem \(C\), em \(A\cap C\) sem \(B\) ou nos três conjuntos. Logo,

\[
\boxed{|A\cap(B\cup C)|=6+4+3=13}.
\]

As parcelas de cada contagem são disjuntas. A interseção tripla foi excluída na primeira seleção e incluída uma única vez na segunda, conforme as condições solicitadas.



