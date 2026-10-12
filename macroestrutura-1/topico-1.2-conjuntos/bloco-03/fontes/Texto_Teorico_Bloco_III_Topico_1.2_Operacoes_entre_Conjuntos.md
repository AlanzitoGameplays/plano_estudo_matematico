# BLOCO III — OPERAÇÕES ENTRE CONJUNTOS

Comparar dois conjuntos permite investigar relações de inclusão e igualdade, ou reconhecer quando elas não ocorrem. Podemos, porém, fazer algo diferente: utilizar os elementos desses conjuntos para construir uma nova coleção.

Essa construção depende de uma condição. Podemos selecionar os objetos que pertencem aos dois conjuntos, os que pertencem a pelo menos um deles ou os que pertencem ao primeiro e não ao segundo. Cada condição determina uma operação, e o significado dessas condições permite explicar as propriedades dos conjuntos construídos.

---

# PARTE I — INTERSEÇÃO E UNIÃO

## Selecionar o que pertence aos dois conjuntos

Considere

\[
A=\{1,2,3\},
\qquad
B=\{3,4,5\}.
\]

Para construir o conjunto dos elementos comuns a \(A\) e \(B\), precisamos exigir duas condições ao mesmo tempo: o objeto deve pertencer a \(A\) **e** pertencer a \(B\).

O número \(3\) satisfaz ambas. O número \(1\) pertence apenas a \(A\), e o número \(4\) pertence apenas a \(B\); por isso, nenhum deles satisfaz a condição conjunta.

O conjunto dos elementos que pertencem simultaneamente a \(A\) e a \(B\) é chamado de **interseção de \(A\) e \(B\)**. Sua notação é \(A\cap B\), lida como “\(A\) interseção \(B\)”. No exemplo,

\[
A\cap B=\{3\}.
\]

A definição se expressa pela condição de pertinência:

\[
\boxed{x\in A\cap B
\iff
(x\in A\land x\in B).}
\]

Essa equivalência fornece tanto um critério para selecionar elementos quanto uma maneira de utilizar a informação de que um elemento pertence à interseção. Se \(x\in A\cap B\), podemos concluir separadamente \(x\in A\) e \(x\in B\). Reciprocamente, as duas pertinências juntas garantem que \(x\in A\cap B\).

A interseção é um novo conjunto determinado pelos elementos comuns. Não é uma afirmação de que \(A\) e \(B\) sejam iguais, nem exige que um deles esteja incluído no outro.

## Reunir o que pertence a pelo menos um dos conjuntos

Podemos utilizar os mesmos conjuntos para outra construção: reunir os elementos que pertencem a \(A\) **ou** a \(B\).

Agora, pertencer a apenas um deles é suficiente. Os números \(1\) e \(2\) entram por pertencerem a \(A\); \(4\) e \(5\) entram por pertencerem a \(B\). O número \(3\) também entra, pois pertencer aos dois conjuntos satisfaz a exigência de pertencer a pelo menos um.

Esse conjunto é a **união de \(A\) e \(B\)**, também chamada de reunião. Escrevemos \(A\cup B\), com a leitura “\(A\) união \(B\)”. Assim,

\[
A\cup B=\{1,2,3,4,5\}.
\]

Por definição,

\[
\boxed{x\in A\cup B
\iff
(x\in A\lor x\in B).}
\]

O OU é **inclusivo**: a condição admite que o elemento pertença a \(A\), a \(B\) ou aos dois. Excluir \(3\) da união seria substituir essa condição por “pertence a exatamente um dos conjuntos”, que tem outro significado.

O elemento comum não aparece duas vezes no conjunto resultante. Sua presença em ambas as coleções não cria dois objetos distintos: a união contém o próprio número \(3\), assim como contém os demais elementos.

> **[R01 — UNIÃO E INTERSEÇÃO]**  
> Integrar aqui dois diagramas de Venn com a mesma disposição de duas regiões sobrepostas, identificadas como \(A\) e \(B\). No primeiro, destacar somente a região comum, correspondente a \(A\cap B\); no segundo, destacar toda a região de \(A\) ou de \(B\), incluindo a sobreposição, correspondente a \(A\cup B\). Função: contrastar a seleção conjunta com a alternativa inclusiva. A fidelidade é relacional; tamanhos e áreas não representam quantidade de elementos. O recurso não substitui as definições por pertinência.

No primeiro diagrama, a região selecionada precisa atender às duas condições. No segundo, basta atender a uma delas. A sobreposição participa de ambos os resultados, mas por razões expressas por condições diferentes.

## Condições de pertinência e formas de representação

A ligação com os conectivos pode ser examinada para um objeto \(x\) qualquer. Cada linha da tabela apresenta uma combinação possível das afirmações de pertinência.

| \(x\in A\) | \(x\in B\) | \(x\in A\cap B\) — E | \(x\in A\cup B\) — OU inclusivo |
|---|---|---|---|
| V | V | V | V |
| V | F | F | V |
| F | V | F | V |
| F | F | F | F |

**R02 — Tabela de pertinência.** As linhas representam possibilidades lógicas, não a existência obrigatória de elementos em cada região.

A primeira linha distingue o OU inclusivo de uma interpretação exclusiva: pertencer aos dois conjuntos torna verdadeira tanto a condição da interseção quanto a da união. A última linha mostra que um objeto ausente de ambos não pertence a nenhum dos dois resultados.

Quando os conjuntos são enumerados, essas condições permitem examinar os elementos apresentados. Quando são definidos por propriedades, podemos combinar diretamente as condições que os caracterizam.

Considere

\[
D=\{1,2,3,4,5,6\},
\]

e, dentro desse domínio,

\[
P=\{x\in D\mid x>2\},
\qquad
Q=\{x\in D\mid x<5\}.
\]

Pertencer a \(P\cap Q\) exige estar em \(D\) e satisfazer conjuntamente as duas desigualdades:

\[
P\cap Q=\{x\in D\mid x>2\land x<5\}
=\{3,4\}.
\]

Já a união exige satisfazer pelo menos uma delas:

\[
P\cup Q=\{x\in D\mid x>2\lor x<5\}=D.
\]

Os elementos \(1\) e \(2\) satisfazem \(x<5\); \(5\) e \(6\) satisfazem \(x>2\); \(3\) e \(4\) satisfazem ambas. Por isso, nenhum elemento de \(D\) fica fora da união.

Em geral, se

\[
P=\{x\in D\mid p(x)\},
\qquad
Q=\{x\in D\mid q(x)\},
\]

então

\[
P\cap Q=\{x\in D\mid p(x)\land q(x)\},
\]

e

\[
P\cup Q=\{x\in D\mid p(x)\lor q(x)\}.
\]

O domínio continua delimitando os objetos considerados. Uma propriedade, isolada dessa delimitação, pode selecionar uma coleção diferente.

## Conjuntos disjuntos e relações com inclusão

Dois conjuntos são **disjuntos** quando não possuem elemento comum. Isso equivale a dizer que sua interseção é vazia:

\[
A\cap B=\varnothing.
\]

Por exemplo, \(\{1,3\}\) e \(\{2,4\}\) são disjuntos. Não existe elemento que satisfaça as duas condições de pertinência simultaneamente.

Ser diferente não basta para ser disjunto. Os conjuntos \(\{1,2,3\}\) e \(\{3,4,5\}\) são diferentes, mas possuem o elemento \(3\) em comum. Além disso, o vazio é disjunto de qualquer conjunto, pois não possui elemento que possa pertencer também à outra coleção.

As definições estabelecem relações imediatas com inclusão:

\[
A\cap B\subseteq A,
\qquad
A\cap B\subseteq B.
\]

De fato, qualquer elemento da interseção pertence aos dois conjuntos e, portanto, a cada um deles. Para a união, a direção se inverte:

\[
A\subseteq A\cup B,
\qquad
B\subseteq A\cup B.
\]

Um elemento de \(A\) já satisfaz uma das alternativas exigidas pela união; o mesmo ocorre com um elemento de \(B\). Nenhuma dessas inclusões exige que os conjuntos sejam diferentes.

Se \(A\subseteq B\), todo elemento de \(A\) já pertence a \(B\). Logo, os elementos comuns são exatamente os de \(A\), enquanto reunir os elementos dos dois conjuntos não acrescenta nada a \(B\):

\[
A\cap B=A,
\qquad
A\cup B=B.
\]

Essas relações mostram que o resultado de uma operação depende das pertinências, inclusive quando um conjunto é vazio ou está incluído no outro. Outra construção surge quando, além de exigir uma pertinência, exigimos que a outra não ocorra.

---

# PARTE II — DIFERENÇA, COMPLEMENTO E CONJUNTO DE REFERÊNCIA

## Selecionar os elementos de um conjunto que não pertencem ao outro

Retome

\[
A=\{1,2,3\},
\qquad
B=\{3,4,5\}.
\]

Para selecionar os elementos de \(A\) que não pertencem a \(B\), começamos pelos elementos de \(A\) e excluímos os que também estão em \(B\). O número \(3\) não permanece; \(1\) e \(2\) permanecem.

O resultado é a **diferença de \(A\) e \(B\)**, indicada por \(A\setminus B\) e lida como “\(A\) menos \(B\)”:

\[
A\setminus B=\{1,2\}.
\]

Por definição,

\[
\boxed{x\in A\setminus B
\iff
(x\in A\land x\notin B).}
\]

As duas condições são indispensáveis. Não pertencer a \(B\) não basta: o objeto precisa pertencer a \(A\). Por exemplo, \(6\notin B\), mas \(6\) não pertence à diferença porque também não pertence a \(A\).

A operação não modifica os conjuntos originais. Ela constrói outro conjunto, selecionando entre os elementos do primeiro aqueles que satisfazem a condição de exclusão.

## A direção da diferença

Se invertermos a ordem dos conjuntos, começamos por outra coleção:

\[
B\setminus A=\{4,5\}.
\]

O resultado mudou porque mudaram tanto a pertinência exigida quanto a ausência exigida:

\[
\begin{aligned}
x\in A\setminus B
&\iff x\in A\land x\notin B,\\
x\in B\setminus A
&\iff x\in B\land x\notin A.
\end{aligned}
\]

O número \(1\) testemunha a diferença entre os resultados: pertence a \(A\setminus B\), mas não a \(B\setminus A\). Portanto, não vale, em geral, a igualdade

\[
A\setminus B=B\setminus A.
\]

> **[R04 — DIFERENÇA EM SENTIDOS OPOSTOS]**  
> Integrar aqui dois diagramas com a mesma configuração de \(A\) e \(B\) sobrepostos. Destacar, no primeiro, a região de \(A\) externa a \(B\), identificada como \(A\setminus B\); no segundo, a região de \(B\) externa a \(A\), identificada como \(B\setminus A\). Função: tornar perceptível a mudança da coleção de partida. Excluir a região comum em ambos; preservar posições e rótulos. A área não tem significado quantitativo.

A diferença é definida para quaisquer dois conjuntos. Não é necessário supor \(B\subseteq A\) para formar \(A\setminus B\). No exemplo, \(4\) e \(5\) pertencem a \(B\), mas estão fora de \(A\); sua presença em \(B\) não altera quais elementos de \(A\) serão selecionados.

Se os conjuntos forem disjuntos, nenhum elemento do primeiro será excluído, e \(A\setminus B=A\). Se todo elemento de \(A\) pertencer a \(B\), nenhum permanecerá, e \(A\setminus B=\varnothing\). Assim, a diferença pode ser igual ao conjunto inicial ou ao vazio sem deixar de obedecer à mesma definição.

## Por que o complemento exige uma referência

Perguntar quais elementos de \(A\) não pertencem a \(B\) delimita a coleção de partida. Já a pergunta “quais objetos não pertencem a \(A\)?” ainda deixa em aberto quais objetos estamos considerando.

Para responder de maneira determinada, fixamos um **conjunto universo**, ou **universo de referência**, indicado por \(U\). Ele reúne os objetos considerados na situação. Ao definir o complemento de \(A\) nesse universo, supomos \(A\subseteq U\).

O **complemento de \(A\) relativamente a \(U\)** é o conjunto dos elementos de \(U\) que não pertencem a \(A\). Com o universo definido, utilizamos a notação

\[
\boxed{A^c=U\setminus A.}
\]

Logo, para qualquer objeto \(x\),

\[
x\in A^c
\iff
(x\in U\land x\notin A).
\]

Somente quando \(x\) já está sendo considerado em \(U\) podemos abreviar a leitura para

\[
x\in A^c\iff x\notin A,
\qquad\text{para }x\in U.
\]

O universo não é um conjunto de todos os objetos possíveis. É a referência delimitada da situação. Um objeto fora de \(U\) não pertence nem a \(A\) nem ao complemento de \(A\) nesse universo.

## O mesmo conjunto em universos diferentes

Considere

\[
A=\{1,3,5\},
\]

e duas referências possíveis:

\[
U=\{1,2,3,4,5\},
\qquad
V=\{1,2,3,4,5,6,7\}.
\]

Em ambos os casos, \(A\) é o mesmo conjunto e está incluído na referência. Entretanto,

\[
U\setminus A=\{2,4\},
\qquad
V\setminus A=\{2,4,6,7\}.
\]

Os números \(6\) e \(7\) não pertencem a \(A\), mas só fazem parte do segundo complemento, porque não pertencem a \(U\). A mudança de universo alterou o resultado.

> **[R05 — COMPLEMENTOS EM UNIVERSOS DISTINTOS]**  
> Integrar aqui dois painéis, um com o universo \(U=\{1,2,3,4,5\}\) e outro com \(V=\{1,2,3,4,5,6,7\}\). Em cada painel, delimitar \(A=\{1,3,5\}\), mantendo sua identidade, e posicionar os demais elementos dentro do respectivo universo e fora de \(A\). Destacar \(\{2,4\}\) no primeiro e \(\{2,4,6,7\}\) no segundo. Função: mostrar que mudar a referência pode mudar o complemento. Usar os rótulos \(U\setminus A\) e \(V\setminus A\); não empregar \(A^c\) sem qualificar o universo nem sugerir proporção entre áreas e quantidades.

Ao comparar universos distintos, escrever explicitamente \(U\setminus A\) e \(V\setminus A\) evita atribuir ao símbolo \(A^c\) dois significados ao mesmo tempo. Em uma expressão que envolva vários complementos, a referência comum deve permanecer fixa.

## Diferença como interseção com um complemento

Suponha agora \(A,B\subseteq U\), com um mesmo universo definido. Um elemento de \(A\setminus B\) pertence a \(A\) e não pertence a \(B\). Como pertence a \(A\), também pertence a \(U\); assim, a ausência de \(B\) o coloca em \(B^c\).

Essas condições dizem que ele pertence simultaneamente a \(A\) e a \(B^c\). Reciprocamente, um elemento desses dois conjuntos pertence a \(A\) e não pertence a \(B\). Portanto,

\[
\boxed{A\setminus B=A\cap B^c,
\qquad A,B\subseteq U.}
\]

A diferença não exige, em sua definição, escolher um universo. Já a escrita com \(B^c\) exige que esse universo tenha sido fixado e contenha os conjuntos considerados. A igualdade conecta as operações sob essas hipóteses; não elimina a dependência do complemento.

Algumas consequências também são imediatas:

\[
A\setminus\varnothing=A,
\qquad
A\setminus A=\varnothing,
\qquad
\varnothing\setminus A=\varnothing.
\]

No primeiro caso, nenhum elemento de \(A\) é excluído. No segundo, a condição exigiria que um objeto pertencesse e não pertencesse a \(A\), o que é impossível. No terceiro, não há elemento na coleção de partida.

Para a referência \(U\), essas mesmas condições fornecem

\[
U^c=\varnothing,
\qquad
\varnothing^c=U.
\]

Tais igualdades não dependem de uma enumeração particular. Elas decorrem das condições de pertinência, que também permitirão justificar relações mais elaboradas entre as operações.

---

# PARTE III — IDENTIDADES E DEMONSTRAÇÃO COM CONJUNTOS

## De uma verificação particular a uma identidade

Uma **identidade entre conjuntos** é uma igualdade válida para todas as escolhas dos conjuntos que satisfazem as hipóteses indicadas. Ela expressa que duas construções, mesmo descritas de maneiras diferentes, determinam exatamente os mesmos elementos.

Verificar que uma igualdade funciona com certos conjuntos confirma aquele caso. Demonstrá-la exige explicar por que funciona em todos os casos admitidos. Por exemplo, a coincidência entre \(\{1,2\}\cup\{2,3\}\) e \(\{2,3\}\cup\{1,2\}\) sugere uma propriedade, mas sua validade geral depende do significado do OU na união.

O critério de igualdade orienta as demonstrações:

\[
X=Y
\iff
\forall x\,(x\in X\leftrightarrow x\in Y).
\]

Podemos traduzir as pertinências em condições lógicas e mostrar que elas são equivalentes. Também podemos separar o trabalho nas implicações que provam \(X\subseteq Y\) e \(Y\subseteq X\). Nos dois métodos, o elemento é arbitrário: nenhum passo pode depender de uma escolha particular que favoreça a conclusão.

Quando uma identidade envolver \(U\) ou complementos, os conjuntos considerados serão subconjuntos de um mesmo universo \(U\). Para comparar pertinências nesses casos, podemos trabalhar com \(x\in U\); objetos externos ao universo não pertencem a nenhum dos conjuntos dos dois lados.

## Repetir uma condição e combiná-la com vazio ou universo

Exigir duas vezes a mesma pertinência não seleciona uma coleção diferente. Também não acrescenta elementos permitir duas vezes a mesma alternativa:

\[
A\cap A=A,
\qquad
A\cup A=A.
\]

Essas são as propriedades de **idempotência**. A condição \(x\in A\land x\in A\) equivale a \(x\in A\), assim como \(x\in A\lor x\in A\). A repetição não altera o critério.

Na união, o vazio é um **elemento neutro**:

\[
A\cup\varnothing=A.
\]

Ele não acrescenta nenhum elemento. Na interseção, o universo é neutro, para \(A\subseteq U\):

\[
A\cap U=A.
\]

Todo elemento de \(A\) já está em \(U\), de modo que essa exigência adicional não exclui nada.

As combinações inversas têm outro efeito:

\[
A\cap\varnothing=\varnothing,
\qquad
A\cup U=U,
\quad A\subseteq U.
\]

A primeira condição é impossível, pois nenhum objeto pertence ao conjunto vazio. A segunda seleciona todo elemento de \(U\), pois pertencer a \(U\) já satisfaz uma das alternativas. Dizemos, nesse sentido, que o vazio é **dominante** para a interseção e o universo é dominante para a união.

Neutro e dominante descrevem comportamentos relativos à operação. O mesmo vazio que preserva \(A\) em uma união produz o vazio em uma interseção.

## Ordem dos conjuntos e agrupamento das operações

A ordem dos conjuntos não altera uma condição conjunta nem uma alternativa inclusiva. Por isso, união e interseção são **comutativas**:

\[
A\cap B=B\cap A,
\qquad
A\cup B=B\cup A.
\]

No primeiro caso, as condições \(x\in A\land x\in B\) e \(x\in B\land x\in A\) são equivalentes. No segundo, o mesmo vale para as condições ligadas por OU. Essa justificação vale para qualquer elemento e quaisquer conjuntos.

O agrupamento também não altera o resultado quando se repete uma mesma operação. As propriedades **associativas** são

\[
(A\cap B)\cap C=A\cap(B\cap C),
\]

e

\[
(A\cup B)\cup C=A\cup(B\cup C).
\]

Na interseção, qualquer um dos agrupamentos exige pertencer aos três conjuntos. Na união, qualquer um deles exige pertencer a pelo menos um dos três. As igualdades resultam da associatividade dos conectivos correspondentes.

Por isso, podemos escrever \(A\cap B\cap C\) ou \(A\cup B\cup C\) sem indicar o agrupamento. Quando as operações são diferentes, entretanto, precisamos explicitar o que será combinado primeiro.

Considere

\[
A=\{1\},\qquad B=\{2\},\qquad C=\{2\}.
\]

Então

\[
(A\cup B)\cap C=\{2\},
\qquad
A\cup(B\cap C)=\{1,2\}.
\]

Esse contraexemplo mostra que alterar o agrupamento de operações diferentes pode alterar o conjunto. A associatividade de cada operação não autoriza esse deslocamento.

## Absorção: reconhecer uma condição redundante

Considere a construção \(A\cap(A\cup B)\). Para pertencer a ela, um objeto precisa estar em \(A\) e também em \(A\cup B\). Mas a primeira exigência já garante a segunda. A união acrescenta uma condição que, nesse contexto, é redundante.

Essa observação conduz à identidade de **absorção**:

\[
\boxed{A\cap(A\cup B)=A.}
\]

Para demonstrá-la por pertinência, seja \(x\) um objeto arbitrário. Pelas definições,

\[
\begin{aligned}
x\in A\cap(A\cup B)
&\iff
(x\in A)\land(x\in A\cup B)\\
&\iff
(x\in A)\land\bigl((x\in A)\lor(x\in B)\bigr)\\
&\iff x\in A.
\end{aligned}
\]

A última equivalência pode ser reconstruída nos dois sentidos. Se a condição composta é verdadeira, sua primeira parte fornece \(x\in A\). Se \(x\in A\), a alternativa \(x\in A\lor x\in B\) também é verdadeira, e a condição composta fica satisfeita.

Assim, a pertinência no conjunto da esquerda equivale à pertinência em \(A\) para qualquer \(x\). Isso demonstra a igualdade.

A outra identidade de absorção é

\[
A\cup(A\cap B)=A.
\]

Todo elemento de \(A\cap B\) já pertence a \(A\). Reuni-lo aos elementos de \(A\) não acrescenta elemento algum. Em condições lógicas, a equivalência é

\[
(x\in A)\lor\bigl((x\in A)\land(x\in B)\bigr)
\iff x\in A.
\]

Nas duas identidades, reconhecer a redundância simplifica a construção sem perder informação sobre seus elementos.

## Distributividade: combinar uma exigência com alternativas

Pertencer a \(A\cap(B\cup C)\) significa atender a uma exigência fixa — pertencer a \(A\) — e a uma alternativa: pertencer a \(B\) ou a \(C\).

Podemos distribuir a exigência fixa pelas alternativas. O objeto deverá pertencer a \(A\) e a \(B\), ou pertencer a \(A\) e a \(C\). Isso sugere:

\[
\boxed{A\cap(B\cup C)=(A\cap B)\cup(A\cap C).}
\]

Vamos demonstrar essa propriedade por **dupla inclusão**, mantendo visíveis as duas direções do raciocínio.

**Primeira inclusão.** Seja \(x\) arbitrário e suponha

\[
x\in A\cap(B\cup C).
\]

Pela definição de interseção, \(x\in A\) e \(x\in B\cup C\). A segunda pertinência significa que \(x\in B\) ou \(x\in C\).

Se \(x\in B\), sua pertinência a \(A\) fornece \(x\in A\cap B\). Se \(x\in C\), fornece \(x\in A\cap C\). Em qualquer dessas alternativas,

\[
x\in(A\cap B)\cup(A\cap C).
\]

As alternativas podem ocorrer simultaneamente; isso não prejudica a conclusão, pois a união utiliza OU inclusivo. Logo,

\[
A\cap(B\cup C)\subseteq(A\cap B)\cup(A\cap C).
\]

**Inclusão inversa.** Seja \(x\) arbitrário e suponha

\[
x\in(A\cap B)\cup(A\cap C).
\]

Então \(x\in A\cap B\) ou \(x\in A\cap C\). Na primeira alternativa, \(x\in A\) e \(x\in B\); na segunda, \(x\in A\) e \(x\in C\).

Em ambas, \(x\in A\). Além disso, \(x\) pertence a pelo menos um dos conjuntos \(B\) e \(C\), de modo que \(x\in B\cup C\). Portanto,

\[
x\in A\cap(B\cup C),
\]

e

\[
(A\cap B)\cup(A\cap C)\subseteq A\cap(B\cup C).
\]

As duas inclusões demonstram a igualdade. A prova não depende da existência de elementos em uma região particular nem de os conjuntos serem diferentes ou não vazios.

> **[R06 — DISTRIBUTIVIDADE EM TRÊS CONJUNTOS]**  
> Integrar aqui dois diagramas com a mesma disposição de \(A\), \(B\) e \(C\), contemplando todas as combinações de pertinência. No primeiro, destacar a parte de \(A\) que está em \(B\) ou em \(C\). No segundo, identificar \(A\cap B\) e \(A\cap C\) e destacar sua união. Função: mostrar que duas decomposições selecionam as mesmas regiões. A região comum aos três pertence a ambos os resultados; regiões de \(B\) ou \(C\) externas a \(A\) não pertencem. O esquema representa condições possíveis, sem afirmar que todas as regiões possuem elementos, e não substitui a demonstração.

A união também se distribui em relação à interseção:

\[
A\cup(B\cap C)=(A\cup B)\cap(A\cup C).
\]

No lado esquerdo, basta pertencer a \(A\); fora de \(A\), é necessário pertencer tanto a \(B\) quanto a \(C\). O lado direito expressa a mesma seleção: pertencer a \(A\) satisfaz as duas uniões; sem essa pertinência, a primeira exige \(B\), e a segunda exige \(C\).

A equivalência lógica que formaliza essa interpretação é

\[
\begin{aligned}
&(x\in A)\lor\bigl((x\in B)\land(x\in C)\bigr)\\
&\qquad\iff
\bigl((x\in A)\lor(x\in B)\bigr)
\land
\bigl((x\in A)\lor(x\in C)\bigr).
\end{aligned}
\]

Traduzindo cada condição pelas definições das operações, obtemos a identidade para qualquer \(x\).

## Complementação dentro de um universo fixo

Fixe \(U\) e suponha \(A\subseteq U\). Nenhum objeto pode pertencer a \(A\) e ao seu complemento ao mesmo tempo:

\[
A\cap A^c=\varnothing.
\]

A condição exigiria \(x\in A\) e \(x\notin A\). Já todo elemento de \(U\) pertence a \(A\) ou não pertence a \(A\). Na segunda situação, pertence a \(A^c\). Portanto,

\[
A\cup A^c=U.
\]

A união não contém objetos externos ao universo, pois tanto \(A\) quanto \(A^c\) estão incluídos em \(U\). Isso explica por que o resultado é precisamente a referência escolhida.

Complementar novamente, sem mudar o universo, recupera o conjunto inicial:

\[
\boxed{(A^c)^c=A.}
\]

Para \(x\in U\), a condição pode ser acompanhada por

\[
\begin{aligned}
x\in(A^c)^c
&\iff x\notin A^c\\
&\iff \neg(x\notin A)\\
&\iff x\in A.
\end{aligned}
\]

Todos os conjuntos dessa comparação estão em \(U\). A equivalência vale para cada elemento da referência e estabelece a igualdade. Mudar o universo entre as duas complementações alteraria a operação e não estaria coberto por essa propriedade.

## Leis de De Morgan: negar condições de pertinência

Suponha \(A,B\subseteq U\), com os complementos tomados no mesmo universo. Para pertencer ao complemento de \(A\cup B\), um objeto de \(U\) não pode pertencer à união.

Como a união admite a pertinência a qualquer um dos dois conjuntos, ficar fora dela exige ficar fora **de ambos**. Obtemos a primeira lei de De Morgan:

\[
\boxed{(A\cup B)^c=A^c\cap B^c.}
\]

Para demonstrá-la, tome \(x\in U\) arbitrário. A definição de complemento, a definição de união e a lei lógica de De Morgan fornecem:

\[
\begin{aligned}
x\in(A\cup B)^c
&\iff x\notin A\cup B\\
&\iff \neg\bigl((x\in A)\lor(x\in B)\bigr)\\
&\iff \neg(x\in A)\land\neg(x\in B)\\
&\iff (x\notin A)\land(x\notin B)\\
&\iff (x\in A^c)\land(x\in B^c)\\
&\iff x\in A^c\cap B^c.
\end{aligned}
\]

O passo central é lógico: negar uma alternativa inclusiva exige negar as duas possibilidades. A passagem da não pertinência para a pertinência aos complementos é legítima porque \(x\in U\).

Como a equivalência vale para qualquer \(x\in U\), e ambos os conjuntos estão incluídos em \(U\), a igualdade está demonstrada.

Para o complemento de uma interseção, a exigência é diferente. Um elemento de \(U\) fica fora de \(A\cap B\) quando falha pelo menos uma das duas pertinências necessárias. Ele pode pertencer a apenas um dos conjuntos ou a nenhum deles. A segunda lei é:

\[
\boxed{(A\cap B)^c=A^c\cup B^c.}
\]

O argumento se condensa na equivalência

\[
\neg\bigl((x\in A)\land(x\in B)\bigr)
\iff
(x\notin A)\lor(x\notin B),
\]

que, para \(x\in U\), equivale a \(x\in A^c\cup B^c\). Essa tradução demonstra a segunda identidade sem exigir uma repetição integral do procedimento anterior.

Não seria correto substituir a união por interseção nessa segunda lei. Se um objeto pertence a \(A\) e não pertence a \(B\), ele já está fora de \(A\cap B\), embora não esteja fora dos dois conjuntos. Uma única condição que falhe basta para negar a condição conjunta.

## Diferença, interseção e inclusão

A diferença permite reconhecer a inclusão pela ausência de exceções:

\[
\boxed{A\setminus B=\varnothing
\iff
A\subseteq B.}
\]

Se \(A\subseteq B\), todo elemento de \(A\) pertence a \(B\). Não há objeto que pertença a \(A\) e falte em \(B\); portanto, a diferença é vazia.

Reciprocamente, suponha \(A\setminus B=\varnothing\). Para um elemento arbitrário \(x\in A\), não é possível \(x\notin B\), pois isso o colocaria em \(A\setminus B\), contrariando o fato de esse conjunto ser vazio. Assim, \(x\in B\). Como isso vale para qualquer elemento de \(A\), temos \(A\subseteq B\).

Essa equivalência não exige universo nem complementos. Ela retoma exatamente a condição que caracteriza uma inclusão e mostra como uma operação pode expressar a inexistência de testemunhas de sua falha.

Também podemos reconhecer a inclusão pela interseção ou pela união:

\[
A\subseteq B
\iff
A\cap B=A
\iff
A\cup B=B.
\]

A inclusão implica as duas igualdades, como já foi justificado pelas definições. No sentido inverso, se \(A\cap B=A\), todo elemento de \(A\) pertence à interseção e, portanto, a \(B\). Se \(A\cup B=B\), todo elemento de \(A\) pertence à união, que é o próprio \(B\). Cada igualdade implica, assim, \(A\subseteq B\).

A interseção e a diferença ainda permitem recompor \(A\):

\[
A=(A\cap B)\cup(A\setminus B).
\]

De fato, um elemento de \(A\) pertence a \(B\) ou não pertence a \(B\). Na primeira alternativa, pertence a \(A\cap B\); na segunda, a \(A\setminus B\). Reciprocamente, qualquer elemento dessas duas construções pertence a \(A\). A dupla inclusão estabelece a igualdade.

As duas parcelas não possuem elemento comum:

\[
(A\cap B)\cap(A\setminus B)=\varnothing,
\]

pois pertencer a ambas exigiria simultaneamente \(x\in B\) e \(x\notin B\). A decomposição separa, portanto, os elementos de \(A\) segundo duas condições incompatíveis e que, juntas, abrangem todos eles.

As operações constroem conjuntos por condições de pertinência. Quando essas condições são traduzidas em afirmações lógicas, podemos reconhecer exigências redundantes, reorganizar alternativas e justificar igualdades. Uma demonstração mostra por que duas construções selecionam os mesmos objetos; seu alcance vem do raciocínio com elementos arbitrários e das hipóteses preservadas em cada passo.
