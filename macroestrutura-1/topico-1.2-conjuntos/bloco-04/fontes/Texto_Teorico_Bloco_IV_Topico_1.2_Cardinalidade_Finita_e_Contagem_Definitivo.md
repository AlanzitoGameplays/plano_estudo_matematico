# BLOCO IV — CARDINALIDADE FINITA E CONTAGEM

Nos Blocos anteriores, estudamos como identificar elementos, comparar conjuntos e construir novos conjuntos por meio de operações. Essas relações permitem determinar quais objetos pertencem a uma coleção, quais são comuns a duas coleções e quais ficam de fora de uma determinada seleção.

Podemos, entretanto, investigar outra característica dos conjuntos: **a quantidade de elementos que possuem**.

Considere \(A=\{2,4,6,8\}\). Sabemos identificar seus elementos e verificar relações de pertinência, mas também podemos afirmar que \(A\) possui quatro elementos. Essa informação não descreve individualmente os objetos da coleção: ela expressa uma quantidade associada ao conjunto.

A passagem da identificação dos elementos à determinação de sua quantidade introduz a noção de **cardinalidade**. Com ela, poderemos compreender como a quantidade de elementos se relaciona com a igualdade, a inclusão e as operações entre conjuntos.

---

# PARTE I — CONJUNTOS FINITOS E CARDINALIDADE

## Conjuntos finitos e quantidade de elementos

Considere o conjunto

\[
A=\{3,5,7,9\}.
\]

Seus elementos são \(3\), \(5\), \(7\) e \(9\). Podemos contá-los individualmente e concluir que existem quatro elementos em \(A\).

Essa contagem termina porque o conjunto possui uma quantidade limitada de elementos. Dizemos, nesse caso, que \(A\) é um **conjunto finito**.

Um conjunto é finito quando seus elementos podem ser completamente contados, obtendo-se uma quantidade determinada e finita. Isso não significa que todos precisem estar escritos entre chaves. Um conjunto descrito por uma propriedade também pode ser finito, desde que a condição selecione apenas uma quantidade finita de objetos.

Por exemplo, considere

\[
B=\{x\in\{1,2,3,4,5,6\}\mid x>3\}.
\]

A condição seleciona os números \(4\), \(5\) e \(6\). Portanto,

\[
B=\{4,5,6\}.
\]

Embora \(A\) esteja apresentado diretamente por enumeração e \(B\) por uma propriedade, ambos são finitos. A diferença entre suas representações não altera o significado da contagem.

Existem também conjuntos que não possuem uma quantidade finita de elementos. A coleção formada por todos os números da sequência \(1,2,3,\ldots\), sem último termo, é um exemplo. Não é possível terminar sua contagem após uma quantidade finita de passos.

Neste Bloco, trabalharemos exclusivamente com **conjuntos finitos**. Isso nos permitirá associar a cada conjunto estudado uma quantidade inteira não negativa de elementos.

## Cardinalidade: contar elementos distintos

A quantidade de elementos de um conjunto finito é chamada de **cardinalidade**.

Para representar essa quantidade, utilizamos duas barras verticais envolvendo o nome do conjunto. Assim,

\[
|A|
\]

é a notação da cardinalidade de \(A\), lida como “cardinalidade de \(A\)” ou “número de elementos de \(A\)”.

No exemplo anterior,

\[
A=\{3,5,7,9\},
\]

temos

\[
\boxed{|A|=4.}
\]

O número \(4\) não é um elemento adicional de \(A\). Ele expressa quantos elementos distintos pertencem à coleção.

Essa distinção importa porque a cardinalidade é uma característica do conjunto considerado, não um objeto que passa a pertencer a ele. Em nosso exemplo, \(4\notin A\), embora \(|A|=4\).

A contagem também não depende da ordem em que os elementos aparecem. Se escrevermos

\[
C=\{9,3,7,5\},
\]

teremos exatamente os mesmos elementos de \(A\), apenas apresentados em outra ordem. Logo,

\[
C=A
\qquad\text{e}\qquad
|C|=|A|=4.
\]

Da mesma maneira, repetir um elemento na representação não cria novos elementos. A escrita

\[
D=\{3,5,5,7,9,9\}
\]

determina o mesmo conjunto que \(A\). Embora apareçam seis entradas entre as chaves, existem apenas quatro elementos distintos:

\[
D=\{3,5,7,9\},
\qquad
|D|=4.
\]

Portanto, **determinar a cardinalidade não significa contar quantas vezes algo foi escrito, mas quantos objetos distintos pertencem ao conjunto**.

Essa propriedade será essencial quando estudarmos a quantidade de elementos de uma união: um objeto que pertence a dois conjuntos não se transforma em dois elementos diferentes quando eles são reunidos.

## Cardinalidade do vazio e dos conjuntos unitários

O conjunto vazio é um caso fundamental. Como não possui elemento algum, sua cardinalidade é zero:

\[
\boxed{|\varnothing|=0.}
\]

O número zero expressa precisamente a ausência de elementos. Ele não indica que a contagem falhou ou que desconhecemos a quantidade; indica que essa quantidade é nula.

Já um conjunto unitário possui exatamente um elemento. Por exemplo,

\[
E=\{5\}
\]

possui cardinalidade

\[
|E|=1.
\]

A distinção entre o conjunto vazio e um conjunto que contém o próprio vazio, estabelecida no Bloco I, também se manifesta na cardinalidade.

Compare:

\[
\varnothing
\qquad\text{e}\qquad
\{\varnothing\}.
\]

O primeiro conjunto não possui elementos. O segundo possui um elemento, que é justamente o conjunto vazio.

Consequentemente,

\[
\boxed{
|\varnothing|=0,
\qquad
|\{\varnothing\}|=1.
}
\]

Não devemos interpretar o segundo conjunto como vazio apenas porque seu único elemento é \(\varnothing\). A cardinalidade considera **a quantidade de objetos que pertencem diretamente ao conjunto**, independentemente da natureza desses objetos.

O mesmo princípio vale quando os elementos são outros conjuntos. Por exemplo,

\[
F=\bigl\{\{1,2\},\{3\},\varnothing\bigr\}
\]

possui três elementos: o conjunto \(\{1,2\}\), o conjunto \(\{3\}\) e o conjunto vazio. Portanto,

\[
|F|=3.
\]

Os números \(1\), \(2\) e \(3\) não são elementos diretos de \(F\); eles pertencem a conjuntos que, por sua vez, são elementos de \(F\). A contagem precisa respeitar essa organização.

## Igualdade de conjuntos e igualdade de cardinalidades

No Bloco II, estabelecemos que dois conjuntos são iguais quando possuem exatamente os mesmos elementos.

Essa condição fornece uma consequência imediata: **conjuntos iguais possuem a mesma cardinalidade**, desde que sejam finitos.

Se \(A=B\), não existe elemento pertencente a apenas um deles. Como a quantidade de elementos é determinada pelos próprios elementos do conjunto, não pode haver diferença entre suas cardinalidades.

Assim,

\[
\boxed{
A=B\implies |A|=|B|.
}
\]

Entretanto, a implicação inversa não é verdadeira em geral.

Considere

\[
A=\{1,2,3\}
\qquad\text{e}\qquad
B=\{4,5,6\}.
\]

Temos

\[
|A|=3
\qquad\text{e}\qquad
|B|=3.
\]

Os dois conjuntos possuem a mesma cardinalidade, mas não são iguais. O número \(1\), por exemplo, pertence a \(A\) e não pertence a \(B\).

Portanto,

\[
|A|=|B|
\qquad\text{mas}\qquad
A\neq B.
\]

A igualdade entre conjuntos exige a coincidência de todos os elementos. A igualdade entre cardinalidades exige apenas a coincidência das quantidades.

A cardinalidade, por isso, não fornece uma descrição completa de um conjunto. Ela informa quantos elementos existem, mas não determina quais são esses elementos.

Essa diferença permite comparar conjuntos de naturezas distintas. O conjunto \(\{2,4,6\}\), por exemplo, possui a mesma cardinalidade que \(\{\text{a},\text{b},\text{c}\}\), embora seus elementos sejam diferentes.

## Inclusão e comparação de cardinalidades

A inclusão também estabelece relações entre quantidades.

Considere

\[
A=\{2,4\}
\qquad\text{e}\qquad
B=\{1,2,3,4,5\}.
\]

Como todos os elementos de \(A\) pertencem a \(B\),

\[
A\subseteq B.
\]

Além disso,

\[
|A|=2,
\qquad
|B|=5.
\]

A quantidade de elementos de \(A\) é menor que a quantidade de elementos de \(B\). Isso não ocorre por uma coincidência numérica: resulta da própria relação de inclusão.

Quando \(A\subseteq B\), todos os elementos de \(A\) já estão entre os elementos de \(B\). Assim, ao contar os elementos de \(B\), necessariamente encontramos todos os elementos de \(A\), podendo encontrar outros.

Para conjuntos finitos, concluímos que

\[
\boxed{
A\subseteq B\implies |A|\leq |B|.
}
\]

A desigualdade permite a igualdade. Se \(A=B\), os dois conjuntos possuem a mesma quantidade de elementos e a inclusão continua válida.

A situação muda quando a inclusão é própria.

Se \(A\subsetneq B\), sabemos que todos os elementos de \(A\) pertencem a \(B\), mas existe pelo menos um elemento de \(B\) que não pertence a \(A\).

Esse elemento adicional aumenta a quantidade de elementos de \(B\). Como os conjuntos são finitos, temos

\[
\boxed{
A\subsetneq B\implies |A|<|B|.
}
\]

A justificativa utiliza as duas condições da inclusão própria. A inclusão garante que nenhum elemento de \(A\) está ausente de \(B\); a diferença entre os conjuntos garante que \(B\) possui pelo menos um elemento adicional.

Há também uma consequência importante. Se \(A\subseteq B\) e os conjuntos finitos possuem a mesma cardinalidade, então necessariamente \(A=B\).

De fato, se a inclusão fosse própria, \(B\) teria mais elementos que \(A\), contrariando a igualdade das cardinalidades. Logo,

\[
\boxed{
A\subseteq B
\quad\text{e}\quad
|A|=|B|
\implies A=B.
}
\]

Não devemos inverter indiscriminadamente essas relações. Saber apenas que \(|A|<|B|\) não garante que \(A\) esteja incluído em \(B\). Por exemplo,

\[
A=\{8\},
\qquad
B=\{1,2\}
\]

satisfazem \(|A|<|B|\), mas \(A\nsubseteq B\), pois \(8\notin B\).

A inclusão compara os elementos; a cardinalidade compara suas quantidades. Uma relação pode fornecer informações sobre a outra, mas não devemos tratá-las como equivalentes.

## Decomposição de conjuntos finitos

Até aqui, determinamos a cardinalidade de conjuntos apresentados diretamente e relacionamos essa quantidade com igualdade e inclusão.

Podemos avançar utilizando as operações do Bloco III.

Considere

\[
S=\{1,2,3,4,5,6\}.
\]

Esse conjunto possui seis elementos:

\[
|S|=6.
\]

Agora, separe seus elementos em dois conjuntos:

\[
P=\{1,3,5\}
\qquad\text{e}\qquad
Q=\{2,4,6\}.
\]

Todos os elementos de \(S\) aparecem em \(P\) ou em \(Q\). Portanto,

\[
S=P\cup Q.
\]

Além disso, nenhum elemento pertence simultaneamente aos dois conjuntos:

\[
P\cap Q=\varnothing.
\]

Dizemos que \(S\) foi **decomposto em duas partes disjuntas**, porque a união das partes recupera o conjunto original e não existe elemento comum a elas.

Essa decomposição não altera os elementos de \(S\). Apenas permite organizar sua contagem em duas parcelas.

O conjunto \(P\) possui três elementos e \(Q\) também possui três. Como nenhum elemento aparece nas duas parcelas, podemos somar suas quantidades:

\[
|S|=|P|+|Q|=3+3=6.
\]

A igualdade é válida porque cada elemento de \(S\) foi contado exatamente uma vez: os elementos ímpares apresentados estão em \(P\), e os elementos pares apresentados estão em \(Q\).

A ideia fundamental não depende de os elementos serem números pares ou ímpares. Qualquer decomposição de um conjunto finito em partes disjuntas permite realizar o mesmo raciocínio.

## Aditividade das cardinalidades de conjuntos disjuntos

A decomposição anterior revela uma propriedade geral.

Se \(A\) e \(B\) são conjuntos finitos e disjuntos, então

\[
A\cap B=\varnothing.
\]

A união \(A\cup B\) contém todos os elementos de \(A\) e todos os elementos de \(B\). Como não existe elemento comum, as duas contagens não se sobrepõem.

Podemos contar primeiro todos os elementos de \(A\) e, em seguida, todos os elementos de \(B\). Nenhum objeto será contado novamente, pois nenhum elemento pertence aos dois conjuntos.

Consequentemente,

\[
\boxed{
A\cap B=\varnothing
\implies
|A\cup B|=|A|+|B|,
}
\]

para conjuntos finitos \(A\) e \(B\).

Essa é a **propriedade aditiva da cardinalidade para conjuntos disjuntos**.

Ela não afirma simplesmente que a cardinalidade de uma união é sempre a soma das cardinalidades dos conjuntos envolvidos. A condição de disjunção é essencial à justificativa: é ela que garante a ausência de contagens repetidas.

> **[R02 — UNIÃO DE CONJUNTOS DISJUNTOS]**
>
> Integrar após esta explicação um diagrama de Venn com dois conjuntos disjuntos \(P=\{1,3,5\}\) e \(Q=\{2,4,6\}\), ambos contidos no conjunto de referência \(S=\{1,2,3,4,5,6\}\). Identificar os elementos de cada região, apresentar \(|P|=3\) e \(|Q|=3\) e relacionar visualmente a união \(P\cup Q=S\) com a soma \(3+3=6\). Nenhum elemento de \(S\) deverá aparecer fora dessas duas regiões. A função do recurso é tornar perceptível que a adição das cardinalidades não provoca duplicação de elementos. As áreas dos círculos não devem sugerir proporções quantitativas.

A propriedade também permanece válida em casos particulares.

Se \(A=\varnothing\), então \(A\) é disjunto de qualquer conjunto finito \(B\), e sua união com \(B\) é o próprio \(B\). Assim,

\[
|\varnothing\cup B|
=
|\varnothing|+|B|
=
0+|B|
=
|B|.
\]

O caso confirma que a propriedade não exige que as duas parcelas possuam elementos. Exige apenas que não compartilhem elementos.

Há, entretanto, uma diferença importante entre a ausência e a presença de sobreposição.

Considere agora

\[
C=\{1,2,3\}
\qquad\text{e}\qquad
D=\{3,4\}.
\]

Temos

\[
|C|=3,
\qquad
|D|=2.
\]

Se somássemos diretamente as duas cardinalidades, obteríamos \(3+2=5\). Mas a união é

\[
C\cup D=\{1,2,3,4\},
\]

e possui apenas quatro elementos:

\[
|C\cup D|=4.
\]

O problema está no elemento \(3\), que pertence aos dois conjuntos. Ao contar separadamente os elementos de \(C\) e os de \(D\), contabilizamos o número \(3\) duas vezes. Na união, entretanto, ele continua sendo um único elemento.

Portanto, a soma direta das cardinalidades funciona quando os conjuntos são disjuntos, mas pode produzir um resultado incorreto quando existe sobreposição.

Para contar os elementos de uma união sem cometer duplicações, precisamos levar em consideração não apenas quantos elementos pertencem a cada conjunto, mas também **quantos pertencem simultaneamente aos conjuntos considerados**.

Essa relação entre a quantidade total e os elementos comuns será o ponto de partida para a contagem de uniões e sobreposições.

---

# PARTE II — CONTAGEM DE UNIÕES E SOBREPOSIÇÕES

## Quando a soma das cardinalidades produz uma contagem duplicada

No exemplo que encerrou a Parte anterior, os conjuntos \(C=\{1,2,3\}\) e \(D=\{3,4\}\) possuem, respectivamente, três e dois elementos. A soma dessas quantidades é cinco, mas sua união contém apenas quatro elementos distintos.

A diferença decorre do elemento \(3\), que pertence aos dois conjuntos e foi contado duas vezes. Como \(C\cap D=\{3\}\), subtrair uma ocorrência desse elemento corrige o resultado:

\[
|C\cup D|=3+2-1=4.
\]

Essa dificuldade não é particular do exemplo. Sempre que dois conjuntos finitos compartilham elementos, a soma de suas cardinalidades contabiliza os elementos comuns duas vezes. Para determinar corretamente a cardinalidade da união, precisamos identificar e corrigir essa duplicação.

## Inclusão-exclusão para dois conjuntos

Considere agora dois conjuntos finitos quaisquer, \(A\) e \(B\).

Os elementos de sua união podem ser distribuídos em três regiões distintas: aqueles que pertencem somente a \(A\), aqueles que pertencem simultaneamente a \(A\) e \(B\) e aqueles que pertencem somente a \(B\).

Em linguagem conjuntista, essas regiões são representadas por

\[
A\setminus B,
\qquad
A\cap B,
\qquad
B\setminus A.
\]

Elas são disjuntas duas a duas: nenhum elemento pode pertencer simultaneamente a duas dessas regiões. Além disso, sua união recupera exatamente \(A\cup B\).

Portanto, utilizando a propriedade aditiva construída na Parte I, podemos escrever

\[
\begin{aligned}
|A\cup B|
={}&|A\setminus B|\\
&+|A\cap B|\\
&+|B\setminus A|.
\end{aligned}
\]

Essa decomposição permite justificar a contagem sem depender de um exemplo particular.

> **[R03 — CONTAGEM DAS REGIÕES DE DOIS CONJUNTOS]**
>
> Integrar aqui um diagrama de Venn com dois conjuntos sobrepostos, \(A\) e \(B\), identificando as três regiões disjuntas: \(A\setminus B\), \(A\cap B\) e \(B\setminus A\). Associar a cada região uma quantidade simbólica, respectivamente \(a\), \(c\) e \(b\). Indicar \(|A|=a+c\), \(|B|=b+c\) e \(|A\cup B|=a+b+c\). Função: tornar perceptível que a soma das cardinalidades individuais conta a região comum duas vezes, enquanto a união a contém uma única vez. As áreas desenhadas não devem representar proporções quantitativas.

A partir dessas três regiões, também podemos reconstruir individualmente os conjuntos \(A\) e \(B\).

O conjunto \(A\) é formado pelos elementos exclusivos de \(A\) e pelos elementos comuns aos dois conjuntos. Como essas partes são disjuntas,

\[
|A|=|A\setminus B|+|A\cap B|.
\]

Pelo mesmo raciocínio,

\[
|B|=|B\setminus A|+|A\cap B|.
\]

Ao somar as duas igualdades, obtemos

\[
\begin{aligned}
|A|+|B|
={}&|A\setminus B|\\
&+2|A\cap B|\\
&+|B\setminus A|.
\end{aligned}
\]

Observe que a cardinalidade da interseção aparece multiplicada por \(2\). Isso acontece porque seus elementos pertencem a \(A\) e também a \(B\), sendo contabilizados nas duas parcelas da soma inicial.

Já a cardinalidade da união é

\[
\begin{aligned}
|A\cup B|
={}&|A\setminus B|\\
&+|A\cap B|\\
&+|B\setminus A|.
\end{aligned}
\]

Comparando as expressões, vemos que a soma \(|A|+|B|\) contém exatamente uma contagem adicional dos elementos comuns.

Assim,

\[
|A|+|B|=|A\cup B|+|A\cap B|.
\]

Isolando a cardinalidade da união, concluímos que

\[
\boxed{
|A\cup B|
=
|A|+|B|-|A\cap B|.
}
\]

Essa igualdade é conhecida como **princípio da inclusão-exclusão para dois conjuntos**.

A soma inicial inclui os elementos dos dois conjuntos, mas conta duas vezes aqueles que pertencem à interseção. A subtração exclui uma dessas duas ocorrências, preservando a outra. Desse modo, cada elemento da união é contabilizado exatamente uma vez.

A demonstração não depende dos valores das cardinalidades, da disposição dos conjuntos em um diagrama ou da natureza de seus elementos. Depende apenas das relações de pertinência que determinam as três regiões disjuntas.

A fórmula também permanece válida quando os conjuntos não possuem elementos comuns. Nesse caso,

\[
A\cap B=\varnothing,
\qquad
|A\cap B|=0,
\]

e a igualdade se reduz a

\[
|A\cup B|=|A|+|B|.
\]

Recuperamos, portanto, a propriedade aditiva dos conjuntos disjuntos como um caso particular da inclusão-exclusão.

O mesmo ocorre quando um conjunto está incluído no outro. Se \(A\subseteq B\), então \(A\cup B=B\) e \(A\cap B=A\). A fórmula fornece

\[
|B|=|A|+|B|-|A|,
\]

confirmando que a inclusão-exclusão continua válida mesmo quando um dos conjuntos não possui região exclusiva.

A subtração da interseção não é, portanto, um procedimento reservado a diagramas com círculos parcialmente sobrepostos. Ela expressa uma propriedade geral da cardinalidade de uniões finitas.

## Interpretação das regiões e das quantidades desconhecidas

A inclusão-exclusão permite determinar a quantidade total de elementos de uma união, mas sua justificativa também fornece informações sobre as regiões que a constituem.

Considere um grupo de \(32\) estudantes. Entre eles, \(18\) estudam uma língua estrangeira \(A\), \(15\) estudam uma língua estrangeira \(B\) e \(6\) estudam ambas.

Representando por \(U\) o conjunto de todos os estudantes considerados, temos

\[
|U|=32,\qquad |A|=18,\qquad |B|=15,
\]

e

\[
|A\cap B|=6.
\]

A quantidade de estudantes que estudam pelo menos uma das duas línguas é

\[
\begin{aligned}
|A\cup B|
&=18+15-6\\
&=27.
\end{aligned}
\]

O resultado corresponde à união, portanto inclui tanto quem estuda apenas uma língua quanto quem estuda as duas.

Para identificar quem estuda somente a língua \(A\), precisamos retirar de \(A\) os estudantes que também pertencem a \(B\). Essa região é \(A\setminus B\), cuja cardinalidade vale

\[
|A\setminus B|=18-6=12.
\]

Da mesma maneira,

\[
|B\setminus A|=15-6=9.
\]

Assim, os \(27\) estudantes da união estão distribuídos em três regiões disjuntas: \(12\) estudam somente \(A\), \(6\) estudam ambas e \(9\) estudam somente \(B\).

A soma dessas quantidades confirma a contagem:

\[
12+6+9=27.
\]

Ainda existem estudantes do universo \(U\) que não pertencem à união. Como \(|U|=32\), a quantidade de estudantes que não estudam nenhuma das duas línguas é

\[
32-27=5.
\]

A decomposição completa do universo fica, portanto, representada pelas quantidades

\[
\underbrace{12+6+9}_{\text{estudam pelo menos uma}}
+
\underbrace{5}_{\text{não estudam nenhuma}}
=32.
\]

Essa última verificação mostra que todas as regiões consideradas são disjuntas e que, reunidas, abrangem o universo.

> **[R04 — CORREÇÃO DA DUPLA CONTAGEM]**
>
> Recurso complementar ao R03. Caso sua integração acrescente clareza, apresentar um esquema compacto associado ao exemplo dos \(32\) estudantes: \(|A|=18\), \(|B|=15\), \(|A\cap B|=6\), soma inicial \(33\) e união corrigida \(27\). Evidenciar que os seis estudantes da interseção foram inicialmente contados duas vezes. Distinguir a região externa, com cinco estudantes, das regiões interiores. Função: relacionar os valores dados para os conjuntos às quantidades exclusivas, comum e externa. Não criar um segundo diagrama redundante se o R03 já desempenhar adequadamente essa função.

O exemplo evidencia ainda uma diferença entre determinar uma região exclusiva e determinar uma interseção.

A expressão \(A\cap B\) representa todos os elementos comuns. Já \(A\setminus B\) representa os elementos de \(A\) que não pertencem a \(B\). Confundir essas condições modifica a região que está sendo contada.

As relações também podem ser utilizadas no sentido inverso. Se conhecemos \(|A|\), \(|B|\) e \(|A\cup B|\), podemos determinar a quantidade de elementos comuns:

\[
|A\cap B|=|A|+|B|-|A\cup B|.
\]

Não se trata de uma nova propriedade, mas da mesma igualdade reorganizada para determinar uma quantidade diferente.

Em contrapartida, conhecer apenas \(|A|\) e \(|B|\) geralmente não basta para determinar \(|A\cup B|\). Dois conjuntos com as mesmas cardinalidades individuais podem ser disjuntos, possuir alguns elementos comuns ou estar relacionados por inclusão. Cada situação pode produzir uma cardinalidade diferente para a união.

A quantidade de elementos comuns é, portanto, uma informação indispensável quando a sobreposição ainda não está determinada.

## Cardinalidade da diferença e do complemento

A contagem de regiões exclusivas pode ser expressa de maneira geral utilizando a decomposição de conjuntos já estabelecida no Bloco III:

\[
A=(A\setminus B)\cup(A\cap B).
\]

As duas parcelas são disjuntas. Um elemento da diferença não pertence a \(B\), enquanto um elemento da interseção necessariamente pertence a \(B\). Portanto, nenhum objeto pode pertencer simultaneamente às duas parcelas.

Como \(A\) é finito, a aditividade das cardinalidades fornece

\[
|A|=|A\setminus B|+|A\cap B|.
\]

Subtraindo a cardinalidade da interseção, obtemos

\[
\boxed{
|A\setminus B|=|A|-|A\cap B|.
}
\]

Essa igualdade expressa uma operação quantitativa correspondente à diferença entre conjuntos. Começamos com todos os elementos de \(A\) e retiramos aqueles que também pertencem a \(B\). O resultado é a quantidade de elementos exclusivos de \(A\).

A direção da diferença continua sendo importante. Para determinar a cardinalidade de \(B\setminus A\), partimos da quantidade de elementos de \(B\):

\[
|B\setminus A|=|B|-|A\cap B|.
\]

As duas diferenças excluem os mesmos elementos comuns, mas partem de conjuntos que podem possuir cardinalidades distintas.

A complementação apresenta uma relação semelhante, agora envolvendo um universo de referência.

Considere um conjunto finito \(U\) e um subconjunto \(A\subseteq U\). O complemento de \(A\) em relação a esse universo contém os elementos de \(U\) que não pertencem a \(A\):

\[
A^c=U\setminus A.
\]

As operações estudadas anteriormente garantem que

\[
U=A\cup A^c
\]

e

\[
A\cap A^c=\varnothing.
\]

Assim, o universo está decomposto em duas partes disjuntas: os elementos que pertencem a \(A\) e os que não pertencem a \(A\).

Pela aditividade,

\[
|U|=|A|+|A^c|.
\]

Consequentemente,

\[
\boxed{
|A^c|=|U|-|A|.
}
\]

A fórmula não determina uma quantidade absoluta de objetos que estão fora de \(A\). Ela determina quantos elementos do universo escolhido não pertencem a \(A\).

Se o universo mudar, a cardinalidade do complemento também poderá mudar, mesmo que o conjunto \(A\) permaneça inalterado.

Essa distinção já era necessária para definir corretamente o complemento. Agora, torna-se igualmente necessária para realizar sua contagem.

## Contagem envolvendo três conjuntos

A inclusão-exclusão para dois conjuntos corrige a duplicação provocada pelos elementos comuns. Entretanto, quando três conjuntos são considerados simultaneamente, um mesmo elemento pode pertencer a um, a dois ou aos três conjuntos.

Isso exige um cuidado adicional: a quantidade de vezes que um elemento aparece na soma inicial depende de quantos conjuntos o contêm.

Considere três conjuntos finitos \(A\), \(B\) e \(C\). Desejamos determinar

\[
|A\cup B\cup C|.
\]

Se somarmos diretamente suas cardinalidades,

\[
|A|+|B|+|C|,
\]

estaremos contando todos os elementos dos três conjuntos, mas alguns deles poderão aparecer mais de uma vez.

Um elemento que pertence somente a \(A\), por exemplo, aparece uma única vez na soma. Já um elemento que pertence a \(A\) e \(B\), mas não a \(C\), aparece duas vezes: uma na contagem de \(A\) e outra na contagem de \(B\).

Um elemento pertencente simultaneamente aos três conjuntos aparece três vezes.

Podemos começar a corrigir essas repetições subtraindo as cardinalidades das interseções duplas:

\[
\begin{aligned}
&|A|+|B|+|C|\\
&\quad-|A\cap B|-|A\cap C|-|B\cap C|.
\end{aligned}
\]

Para compreender o efeito dessas subtrações, precisamos examinar separadamente os elementos conforme suas condições de pertinência.

**Um elemento que pertence a exatamente um conjunto** aparece uma vez na soma inicial e não pertence a nenhuma interseção dupla. Portanto, continua contado uma vez.

**Um elemento que pertence a exatamente dois conjuntos** aparece duas vezes na soma inicial. Entretanto, pertence a uma única interseção dupla: a interseção dos dois conjuntos que o contêm. Sua contagem é reduzida de duas ocorrências para uma.

**Um elemento que pertence aos três conjuntos** apresenta uma situação diferente. Ele aparece três vezes na soma inicial, mas também pertence às três interseções duplas:

\[
A\cap B,\qquad A\cap C,\qquad B\cap C.
\]

Consequentemente, as subtrações retiram esse elemento três vezes. Sua contribuição à contagem passa a ser

\[
3-3=0.
\]

Isso significa que a correção das interseções duplas eliminou todas as ocorrências dos elementos da interseção tripla, quando deveria preservar uma.

Para reparar essa exclusão excessiva, precisamos acrescentar uma vez a cardinalidade de

\[
A\cap B\cap C.
\]

A contagem desses elementos torna-se, então,

\[
3-3+1=1.
\]

Desse modo, todos os elementos pertencentes à união são finalmente contados exatamente uma vez, independentemente de pertencerem a um, dois ou três conjuntos.

Obtemos o **princípio da inclusão-exclusão para três conjuntos finitos**:

\[
\boxed{
\begin{aligned}
|A\cup B\cup C|
={}&|A|+|B|+|C|\\
&-|A\cap B|-|A\cap C|-|B\cap C|\\
&+|A\cap B\cap C|.
\end{aligned}
}
\]

A fórmula não resulta de uma alternância arbitrária entre adições e subtrações. Cada operação possui uma função precisa: a soma inicial reúne as contagens, as subtrações corrigem as duplicações entre pares e a adição final recupera a contribuição dos elementos que pertencem aos três conjuntos.

É importante observar que uma interseção dupla pode conter elementos da interseção tripla.

Por exemplo, \(A\cap B\) reúne **todos** os elementos comuns a \(A\) e \(B\), inclusive aqueles que também pertencem a \(C\). Já a região dos elementos que pertencem a \(A\) e \(B\), mas não a \(C\), é

\[
(A\cap B)\setminus C.
\]

Esses dois conjuntos não são necessariamente iguais. Confundi-los altera a quantidade que deve ser subtraída na fórmula.

### Interpretando as regiões de três conjuntos

Considere os conjuntos

\[
\begin{aligned}
A&=\{1,2,3,4\},\\
B&=\{3,4,5,6\},\\
C&=\{4,6,7\}.
\end{aligned}
\]

Suas cardinalidades são

\[
|A|=4,\qquad |B|=4,\qquad |C|=3.
\]

As interseções duplas são

\[
\begin{aligned}
A\cap B&=\{3,4\},\\
A\cap C&=\{4\},\\
B\cap C&=\{4,6\}.
\end{aligned}
\]

Portanto,

\[
|A\cap B|=2,\qquad
|A\cap C|=1,\qquad
|B\cap C|=2.
\]

A interseção tripla possui somente o elemento \(4\):

\[
A\cap B\cap C=\{4\},
\]

de modo que

\[
|A\cap B\cap C|=1.
\]

Aplicando a inclusão-exclusão,

\[
\begin{aligned}
|A\cup B\cup C|
&=4+4+3-2-1-2+1\\
&=7.
\end{aligned}
\]

Podemos conferir o resultado diretamente:

\[
A\cup B\cup C=\{1,2,3,4,5,6,7\}.
\]

Assim, a união possui realmente sete elementos distintos.

> **[R05 — CONTAGEM DAS REGIÕES DE TRÊS CONJUNTOS]**
>
> Integrar aqui um diagrama de Venn com três conjuntos \(A\), \(B\) e \(C\), utilizando os elementos do exemplo. Identificar as sete regiões interiores pelas seguintes distribuições:
>
> - Somente \(A\): \(\{1,2\}\), cardinalidade \(2\).
> - Somente \(B\): \(\{5\}\), cardinalidade \(1\).
> - Somente \(C\): \(\{7\}\), cardinalidade \(1\).
> - \(A\cap B\), excluindo \(C\): \(\{3\}\), cardinalidade \(1\).
> - \(A\cap C\), excluindo \(B\): \(\varnothing\), cardinalidade \(0\).
> - \(B\cap C\), excluindo \(A\): \(\{6\}\), cardinalidade \(1\).
> - \(A\cap B\cap C\): \(\{4\}\), cardinalidade \(1\).
>
> Função: distinguir as regiões exclusivas das interseções completas e demonstrar visualmente que cada elemento da união deve contribuir uma única vez para sua cardinalidade. A região exclusivamente pertencente a \(A\) e \(C\) deverá permanecer representada e identificada como vazia. Não confundir as cardinalidades de regiões exclusivamente duplas com as cardinalidades das interseções duplas, que incluem o elemento \(4\). O diagrama deverá preservar a possibilidade matemática de regiões vazias; suas áreas não representarão proporções quantitativas.

A distribuição também permite verificar a cardinalidade da união pela soma das sete regiões disjuntas:

\[
2+1+1+1+0+1+1=7.
\]

As duas contagens chegam ao mesmo resultado, mas utilizam informações organizadas de maneiras diferentes.

Na primeira, trabalhamos com as cardinalidades dos conjuntos e de suas interseções, corrigindo os elementos repetidos.

Na segunda, contamos diretamente as regiões disjuntas, nas quais nenhum elemento pode aparecer mais de uma vez.

Essa correspondência revela o fundamento da inclusão-exclusão: **contar corretamente uma união significa garantir que cada elemento que lhe pertence contribua exatamente uma vez para a quantidade total**.

## Da contagem à interpretação dos conjuntos

As relações de cardinalidade permitem conferir resultados e reconhecer quando uma informação quantitativa é incompatível com a estrutura dos conjuntos.

Para dois conjuntos finitos, por exemplo, a interseção não pode possuir mais elementos que qualquer um dos conjuntos que a formam:

\[
|A\cap B|\leq |A|
\qquad\text{e}\qquad
|A\cap B|\leq |B|.
\]

Isso decorre das inclusões

\[
A\cap B\subseteq A,
\qquad
A\cap B\subseteq B.
\]

Pelo mesmo motivo, a união não pode possuir menos elementos que qualquer um dos conjuntos reunidos:

\[
|A|\leq |A\cup B|,
\qquad
|B|\leq |A\cup B|.
\]

Também não pode possuir mais elementos que a soma das duas cardinalidades, pois a inclusão-exclusão apenas retira da soma inicial uma quantidade não negativa:

\[
|A\cup B|\leq |A|+|B|.
\]

Essas relações permitem reconhecer erros de contagem antes mesmo de examinar detalhadamente todos os elementos envolvidos.

Se um cálculo indicar, por exemplo, que a interseção possui mais elementos que um dos conjuntos, ou que a união possui menos elementos que algum deles, o resultado não pode estar correto sob as condições estabelecidas.

O controle quantitativo depende, portanto, da interpretação das relações conjuntistas, e não apenas da execução de operações aritméticas.

Ao longo do Tópico 1.2, a pertinência permitiu identificar elementos; a inclusão e a igualdade permitiram comparar conjuntos; as operações permitiram construir novas coleções a partir de condições de pertencimento. A cardinalidade acrescentou a possibilidade de determinar e relacionar suas quantidades.

Esses conhecimentos se articulam: a quantidade de elementos de uma união depende das condições que determinam quais objetos pertencem a cada conjunto e de como essas condições se sobrepõem.

Assim, a contagem de conjuntos finitos não consiste apenas em somar números. Ela exige compreender **o que está sendo contado, quais elementos são comuns e como organizar a contagem para não duplicar nem omitir objetos**.
