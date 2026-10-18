# BLOCO II — NÚMEROS IRRACIONAIS, REAIS E RETA NUMÉRICA

# PARTE I — A INSUFICIÊNCIA DOS RACIONAIS E OS NÚMEROS IRRACIONAIS

## Quando a representação decimal não é periódica

Os números racionais podem ser representados por expansões decimais finitas ou infinitas eventualmente periódicas. Em outras palavras, um número racional admite uma escrita decimal que termina ou que, a partir de determinada posição, repete indefinidamente um mesmo bloco de algarismos.

Por exemplo,

\[
\frac13=0{,}333333\ldots
\]

possui uma representação decimal infinita, mas seu período é o algarismo \(3\). Já em

\[
\frac16=0{,}166666\ldots,
\]

a repetição começa depois do primeiro algarismo decimal.

A quantidade infinita de casas decimais, portanto, não impede que um número seja racional. A propriedade decisiva é a existência de um período que se repete indefinidamente, ainda que essa repetição comece depois de alguns algarismos iniciais.

Uma expansão decimal infinita, porém, não precisa apresentar essa regularidade. Na interpretação usual dos números como posições de uma reta numérica, também podemos considerar números representados por expansões que nunca se tornam periódicas. Estamos, nesse caso, considerando um domínio numérico mais abrangente que \(\mathbb Q\). Para determinar se um desses números é racional, precisamos verificar se sua representação satisfaz a caracterização decimal dos racionais.

Considere a seguinte representação decimal:

\[
\boxed{
0{,}101001000100001000001\ldots
}
\]

Sua regra de formação é precisa: entre dois algarismos \(1\) consecutivos, colocamos blocos de zeros com comprimentos progressivamente maiores. Primeiro aparece um zero, depois dois, depois três, depois quatro, e assim sucessivamente.

Como o comprimento desses blocos continua crescendo, a escrita possui infinitos algarismos e não apresenta uma repetição periódica.

Para compreender por quê, suponha que, a partir de determinada posição, existisse um período fixo.

Esse período precisaria reproduzir todos os algarismos seguintes. Se fosse formado exclusivamente por zeros, a expansão não poderia apresentar novos algarismos \(1\), contrariando sua regra de formação.

Se o período contivesse pelo menos um algarismo \(1\), a repetição desse bloco produziria uma distância máxima fixa entre algarismos \(1\) consecutivos. Entretanto, na expansão construída, os blocos de zeros tornam-se cada vez maiores, ultrapassando qualquer comprimento previamente estabelecido.

Portanto, **não existe um bloco fixo de algarismos que possa repetir-se indefinidamente para produzir essa expansão**.

A representação é infinita e não eventualmente periódica.

Pela caracterização decimal dos racionais, um número com essa representação não pode ser escrito como quociente de dois inteiros com denominador não nulo. Trata-se, assim, de um número que não pertence a \(\mathbb Q\).

Os números dessa natureza são chamados de **números irracionais**.

Nesse domínio numérico mais abrangente, um número é irracional quando não pode ser representado na forma

\[
\frac pq,
\qquad
p,q\in\mathbb Z,\quad q\neq0.
\]

Sua representação decimal é infinita e não eventualmente periódica.

A expansão que construímos constitui um exemplo cuja irracionalidade pode ser justificada pela regra de formação. Não estamos apenas observando alguns algarismos e supondo que não haverá repetição: conhecemos uma regra que determina toda a expansão e impede a existência de um período.

A distinção entre os dois casos pode ser sintetizada pela comparação:

\[
\begin{aligned}
0{,}333333\ldots
&\quad \text{infinita e periódica},\\[4pt]
0{,}101001000100001\ldots
&\quad \text{infinita e não periódica}.
\end{aligned}
\]

A primeira representa um número racional; a segunda, um irracional.

Em particular, **a ausência de um período entre os primeiros algarismos conhecidos de um número não permite concluir que ele seja irracional**. Uma expansão pode apresentar um trecho inicial muito longo e somente depois começar a repetir um bloco.

Para estabelecer a irracionalidade, é necessário algum fundamento que assegure que nenhuma repetição periódica ocorrerá, não importa quantas casas decimais sejam consideradas.

## Outros números irracionais

A expansão decimal construída anteriormente mostra que a existência de números irracionais não depende de uma escrita fracionária ou de uma operação numérica específica.

Entretanto, existem irracionais que também surgem em relações matemáticas conhecidas.

Um exemplo é \(\sqrt2\), símbolo que representa o número positivo cujo quadrado é igual a \(2\):

\[
(\sqrt2)^2=2.
\]

Esse número é irracional. Isso significa que não existem inteiros \(p\) e \(q\), com \(q\neq0\), tais que

\[
\sqrt2=\frac pq.
\]

Sua irracionalidade é um resultado matemático que pode ser demonstrado, mas a demonstração exige propriedades da divisibilidade que não precisamos desenvolver neste momento.

Outro exemplo é \(\pi\), número conhecido no estudo das circunferências e também irracional. Assim como ocorre com \(\sqrt2\), sua irracionalidade não é estabelecida pela simples observação de uma aproximação decimal.

Esses exemplos também mostram que a classificação depende do valor do número, e não da presença de um símbolo particular. A escrita \(\sqrt2\) representa um irracional, mas isso não significa que todo número escrito com o símbolo de raiz quadrada seja irracional. Por exemplo,

\[
\sqrt4=2,
\]

e o número \(2\) é natural, inteiro e racional.

A propriedade que distingue os irracionais permanece a mesma: a impossibilidade de representar o número como quociente de dois inteiros com denominador diferente de zero.

Os racionais, portanto, não abrangem todos os números representados por expansões decimais. Para considerar conjuntamente os racionais e os irracionais, utilizamos um domínio numérico mais abrangente.

---

# PARTE II — O CONJUNTO DOS NÚMEROS REAIS

## O domínio dos números reais

O conjunto dos números racionais contém todos os naturais, todos os inteiros e os demais números que podem ser representados como quocientes de inteiros. Entretanto, o exemplo decimal construído anteriormente mostra que existem números que não satisfazem essa condição.

Para considerar ambos os tipos de números em um mesmo domínio, utilizamos o **conjunto dos números reais**, representado por

\[
\boxed{\mathbb R.}
\]

No tratamento matemático escolar, os números reais são compreendidos como os números associados às posições de uma reta numérica idealizada, considerada em toda a sua extensão e sem lacunas.

Essa reta não é formada apenas pelas posições correspondentes aos inteiros ou aos racionais. Números irracionais também correspondem a suas posições.

Assim, o conjunto \(\mathbb R\) abrange os racionais e os irracionais. A distinção fundamental é que **o conjunto dos racionais não esgota o domínio real**.

Um número como \(\frac12\) é real porque é racional. A expansão não periódica

\[
0{,}101001000100001\ldots
\]

também representa um número real, embora não represente um racional.

Não estamos estabelecendo a existência dos reais por meio de uma demonstração formal de todas as propriedades desse sistema numérico. Estamos utilizando sua apresentação escolar, que associa o domínio real à reta e permite compreender a organização dos números que nela são representados.

A correspondência entre números e posições será examinada geometricamente na Parte III.

## Racionais e irracionais como subconjuntos dos reais

Como todo racional pertence ao conjunto dos reais, temos

\[
\mathbb Q\subseteq\mathbb R.
\]

A inclusão é própria, pois existem números reais que não pertencem a \(\mathbb Q\). O decimal não periódico anteriormente construído fornece um exemplo dessa diferença.

Portanto,

\[
\boxed{\mathbb Q\subsetneq\mathbb R.}
\]

Uma vez estabelecido o domínio \(\mathbb R\), podemos representar precisamente o conjunto dos irracionais utilizando a operação de diferença entre conjuntos:

\[
\boxed{
\mathbb R\setminus\mathbb Q.
}
\]

Essa expressão indica todos os elementos de \(\mathbb R\) que não pertencem a \(\mathbb Q\). Em outras palavras, para um número \(x\),

\[
x\in\mathbb R\setminus\mathbb Q
\]

significa que

\[
x\in\mathbb R
\quad\text{e}\quad
x\notin\mathbb Q.
\]

A caracterização dos irracionais fica, assim, vinculada ao domínio dos reais: são precisamente os números reais que não satisfazem a condição de racionalidade.

Como os números racionais e irracionais pertencem aos reais, e todo real pertence a uma dessas duas categorias, podemos escrever

\[
\boxed{
\mathbb R
=
\mathbb Q\cup(\mathbb R\setminus\mathbb Q).
}
\]

A união reúne todos os números racionais e todos os números reais não racionais. Nenhum número real fica de fora dessa reunião.

Por outro lado, um número não pode ser simultaneamente racional e irracional. Para pertencer a \(\mathbb Q\), precisa admitir representação como quociente de inteiros; para pertencer a \(\mathbb R\setminus\mathbb Q\), precisa não admitir essa representação.

As duas condições não podem ser satisfeitas ao mesmo tempo. Logo,

\[
\boxed{
\mathbb Q\cap(\mathbb R\setminus\mathbb Q)
=
\varnothing.
}
\]

A união e a interseção expressam duas propriedades complementares: **racionais e irracionais, juntos, constituem todos os reais; separadamente, não possuem elementos em comum**.

Essas identidades são relações entre conjuntos. Elas descrevem a composição de um domínio já considerado, mas não constituem, por si sós, uma demonstração da existência ou da completude dos números reais.

## A organização dos conjuntos numéricos

As inclusões estudadas permitem reunir os principais domínios numéricos em uma mesma estrutura:

\[
\boxed{
\mathbb N
\subsetneq
\mathbb Z
\subsetneq
\mathbb Q
\subsetneq
\mathbb R.
}
\]

Cada inclusão indica que todos os elementos do conjunto menor pertencem ao conjunto maior, mas existem elementos do maior que não pertencem ao menor.

A posição dos irracionais nessa organização exige uma distinção: eles não formam outro conjunto que contenha os racionais, nem estão contidos em \(\mathbb Q\). Constituem a parte de \(\mathbb R\) que fica fora de \(\mathbb Q\).

<!-- FIGURA 1 — Diagrama de conjuntos: região externa ℝ; em seu interior, região ℚ contendo regiões aninhadas ℤ e ℕ, com inclusões próprias. A região ℝ fora de ℚ representa ℝ∖ℚ. Posicionar 2 em ℕ, −2 em ℤ fora de ℕ, 1/2 em ℚ fora de ℤ e √2 em ℝ fora de ℚ. As regiões não representam proporções de cardinalidades. -->

*Figura 1 — Diagrama de inclusão dos conjuntos numéricos. Os racionais e os irracionais são regiões disjuntas dentro de \(\mathbb R\). As áreas desenhadas não representam quantidades de elementos.*

O diagrama evidencia que \(2\) pertence simultaneamente aos naturais, inteiros, racionais e reais. O número \(-2\) pertence aos inteiros, racionais e reais, mas não aos naturais.

Já \(\frac12\) pertence aos racionais e reais, sem pertencer aos inteiros. Por sua vez, \(\sqrt2\) pertence aos reais, mas não aos racionais.

Assim, embora os naturais, inteiros e racionais formem uma sequência de conjuntos encaixados, a distinção entre racional e irracional estabelece uma separação dentro de \(\mathbb R\).

Isso também esclarece duas afirmações diferentes: um número natural é necessariamente racional e real; um número irracional, por definição, não pode ser racional.

---

# PARTE III — RETA REAL E RELAÇÕES DE ORDEM

## A representação geométrica dos números reais

Os números reais podem ser representados geometricamente por pontos de uma reta. Para estabelecer essa representação, começamos escolhendo uma reta e um ponto que será associado ao número \(0\), chamado **origem**.

Em seguida, escolhemos um sentido positivo, convencionalmente da esquerda para a direita, e um segmento que servirá como **unidade de comprimento**.

Essas escolhas permitem estabelecer posições numéricas a partir da origem.

O número \(1\) é representado pelo ponto localizado uma unidade à direita do zero; o número \(2\), pelo ponto localizado duas unidades à direita. No sentido oposto, encontramos os pontos associados a \(-1\), \(-2\) e aos demais números negativos.

Essa representação constitui a **reta real**, também chamada de reta numérica.

<!-- FIGURA 2 — Reta real horizontal, com origem em 0, sentido positivo à direita e unidade uniforme. Marcar, na mesma escala, −2, −1, 0, 1/2, 1, 2 e 3; destacar a unidade entre 0 e 1. Assinalar √2 aproximadamente em 1,414, entre 1 e 2, distinguindo-o das marcações exatas. Prolongar a reta nos dois sentidos, sem sugerir que somente os números rotulados possuem posições. -->

*Figura 2 — Reta real orientada, com origem em \(0\), unidade de comprimento e algumas posições numéricas. As distâncias seguem a mesma escala; a posição de \(\sqrt2\) é indicada aproximadamente.*

A unidade escolhida é fundamental. A distância entre os pontos que representam \(0\) e \(1\) deve ser igual à distância entre aqueles que representam \(1\) e \(2\), pois ambas correspondem a uma unidade.

Os números racionais não inteiros também podem ser representados nessa reta.

Por exemplo, o número \(\frac12\) corresponde à posição situada exatamente na metade do segmento entre \(0\) e \(1\). Da mesma forma, \(-\frac12\) corresponde à posição situada na metade do segmento entre \(0\) e \(-1\).

A correspondência não se limita aos racionais. O número irracional \(\sqrt2\), por exemplo, também possui uma posição na reta real. Como é positivo e está entre \(1\) e \(2\), seu ponto representativo encontra-se à direita de \(1\) e à esquerda de \(2\).

A diferença entre racionais e irracionais não determina regiões separadas da reta. Não existe um trecho reservado aos racionais e outro reservado aos irracionais. Ambos possuem posições ao longo da mesma reta real.

### Números e pontos representativos

É importante distinguir o número real do ponto utilizado para representá-lo.

O número \(2\) é um objeto matemático. Quando escolhemos uma origem, uma orientação e uma unidade, associamos esse número a uma posição determinada na reta.

Chamamos o ponto correspondente de **imagem do número**. Reciprocamente, o número real associado a um ponto é sua **abscissa**.

Assim, se um ponto \(P\) representa o número \(2\), dizemos que a abscissa de \(P\) é \(2\).

Números e pontos são objetos de naturezas diferentes, embora a correspondência permita trabalhar com eles conjuntamente.

Na apresentação escolar dos reais, consideramos que cada número real corresponde a um único ponto da reta e que cada ponto corresponde a um único número real, desde que origem, orientação e unidade estejam fixadas.

Isso não significa que uma figura desenhada represente visualmente todos esses números. Uma reta marcada apenas com \(-2,-1,0,1,2\) não contém somente cinco posições matemáticas.

As marcações são referências. Entre elas existem outras posições, correspondentes a números que não foram explicitamente escritos.

A reta real idealizada é considerada sem lacunas: suas posições não se limitam às imagens dos números naturais, inteiros ou racionais. A correspondência completa entre os pontos e os números reais faz parte dessa apresentação geométrica do domínio, não de uma demonstração formal de sua completude.

## Relações de ordem na reta real

A orientação da reta permite interpretar geometricamente a comparação entre números.

Na convenção adotada, **um número é menor que outro quando seu ponto representativo está à esquerda do ponto que representa o outro número**.

Por exemplo, o ponto correspondente a \(1\) está à esquerda do ponto correspondente a \(3\). Expressamos essa relação por

\[
1<3.
\]

O símbolo \(<\) significa *menor que*.

Da mesma forma, podemos afirmar que \(3\) é maior que \(1\):

\[
3>1.
\]

O símbolo \(>\) significa *maior que*.

Essas expressões descrevem a mesma comparação, observada em sentidos diferentes.

A orientação também permite compreender os números negativos. Como \(-3\) está à esquerda de \(-1\), temos

\[
-3<-1.
\]

O sinal negativo, portanto, não determina sozinho qual número é menor. Na comparação entre \(-3\) e \(-1\), o número \(-3\) é menor porque ocupa a posição mais à esquerda na reta.

De maneira semelhante,

\[
-2<0<2.
\]

O zero separa os números negativos, localizados à sua esquerda, dos positivos, localizados à sua direita.

### Desigualdades estritas e não estritas

As relações \(<\) e \(>\) são chamadas de **desigualdades estritas**. Elas afirmam que os números comparados são diferentes e que existe uma relação de ordem determinada entre eles.

A afirmação

\[
a<b
\]

não permite que \(a=b\).

Entretanto, também podemos considerar condições que admitem a igualdade.

O símbolo \(\leq\) significa *menor ou igual a*. Assim,

\[
a\leq b
\]

é verdadeiro quando \(a<b\) ou quando \(a=b\).

Por exemplo,

\[
2\leq5
\]

é verdadeiro porque \(2<5\). A afirmação

\[
2\leq2
\]

também é verdadeira, mas agora porque os números são iguais.

Analogamente, o símbolo \(\geq\) significa *maior ou igual a*. Portanto,

\[
a\geq b
\]

é verdadeiro quando \(a>b\) ou \(a=b\).

Essa diferença entre desigualdades estritas e não estritas altera quais valores satisfazem uma condição.

Se exigimos \(x>2\), o número \(2\) não satisfaz a condição. Se exigimos \(x\geq2\), ele passa a satisfazê-la.

A inclusão ou exclusão da igualdade não é apenas uma diferença de escrita: modifica o conjunto de números considerados.

## Propriedades fundamentais da ordem

A ordem dos números reais permite estabelecer relações gerais que não dependem dos valores particulares escolhidos.

### Tricotomia: três possibilidades mutuamente exclusivas

Considere dois números reais quaisquer, \(a\) e \(b\).

Ao compará-los, exatamente uma das três possibilidades ocorre:

\[
\boxed{
a<b,\qquad a=b,\qquad a>b.
}
\]

Essa propriedade é chamada de **tricotomia da ordem**.

Se os dois números são diferentes, um deles ocupa uma posição à esquerda do outro. Se representam o mesmo número, correspondem à mesma posição.

As três possibilidades não podem ocorrer simultaneamente.

Por exemplo, como \(2<5\), não podemos afirmar ao mesmo tempo que \(2=5\) ou \(2>5\).

Da mesma forma, quando \(a=b\), nenhuma das desigualdades estritas entre eles é verdadeira.

A tricotomia assegura, portanto, que dois números reais podem sempre ser comparados e que a comparação possui uma única dessas três possibilidades.

### Transitividade: conservar a ordem entre três números

Considere agora três números reais \(a\), \(b\) e \(c\).

Se \(a\) está à esquerda de \(b\) e \(b\) está à esquerda de \(c\), então \(a\) necessariamente está à esquerda de \(c\).

Essa relação é expressa pela **transitividade da ordem**:

\[
\boxed{
a<b
\quad\land\quad
b<c
\quad\Longrightarrow\quad
a<c.
}
\]

Por exemplo,

\[
-2<1
\qquad\text{e}\qquad
1<4.
\]

Consequentemente,

\[
-2<4.
\]

Não precisamos comparar novamente \(-2\) e \(4\) de maneira independente. As duas primeiras desigualdades já estabelecem a terceira.

A transitividade permite compreender sequências de comparações e interpretar condições que relacionam mais de dois números.

Assim, a expressão

\[
a<b<c
\]

reúne as condições \(a<b\) e \(b<c\). Pela transitividade, também podemos concluir que \(a<c\).

## A existência de números entre dois reais distintos

Nos números naturais, existem elementos consecutivos.

Por exemplo, \(2\) e \(3\) são naturais consecutivos: não existe número natural maior que \(2\) e menor que \(3\).

Essa propriedade não se mantém quando consideramos todos os números reais.

Entre \(2\) e \(3\), encontramos o número \(2{,}5\):

\[
2<2{,}5<3.
\]

Entre \(2\) e \(2{,}5\), também encontramos outro número real:

\[
2<2{,}25<2{,}5.
\]

E podemos repetir esse procedimento, encontrando novos números em regiões progressivamente menores da reta.

Entretanto, a propriedade não depende desses valores específicos.

Considere quaisquer números reais \(a\) e \(b\), com

\[
a<b.
\]

Na reta, suas posições são distintas. Entre elas existe um segmento de comprimento positivo.

Esse segmento possui um ponto médio, situado estritamente entre suas extremidades. O número real correspondente a esse ponto é a média dos extremos:

\[
m=\frac{a+b}{2}.
\]

Pelo significado de ponto médio, sua posição está à direita de \(a\) e à esquerda de \(b\). Portanto,

\[
\boxed{
a<m<b.
}
\]

Assim, **entre quaisquer dois números reais distintos existe pelo menos outro número real**.

Essa propriedade permite repetir o procedimento indefinidamente. Depois de encontrar um número intermediário, podemos encontrar outro entre ele e um dos extremos, depois outro, e assim sucessivamente.

Consequentemente, entre dois números reais distintos existem infinitos números reais.

Não há, portanto, dois números reais consecutivos.

Essa característica distingue a organização da reta real daquela dos naturais. Os naturais possuem uma sucessão discreta de elementos, enquanto a ordem dos reais permite encontrar novas posições entre quaisquer duas posições distintas.

É importante, contudo, não confundir essa propriedade com a ausência de lacunas da reta real. Os próprios números racionais também possuem números racionais intermediários entre quaisquer dois racionais distintos, mas não correspondem a todos os pontos da reta.

A existência de números intermediários descreve uma propriedade da ordem; **não demonstra, sozinha, que um conjunto numérico preencha completamente a reta**.

## Condições simultâneas de ordem

As relações de ordem podem ser utilizadas não apenas para comparar números determinados, mas também para estabelecer condições que selecionam números reais.

Considere a desigualdade

\[
x>1.
\]

Ela é satisfeita por todos os números reais maiores que \(1\).

O número \(2\) satisfaz essa condição, assim como \(1{,}5\). Entretanto, \(1\) não a satisfaz, pois a desigualdade é estrita.

De maneira semelhante, a condição

\[
x<4
\]

é satisfeita por todos os números reais menores que \(4\).

Podemos exigir que um número satisfaça as duas condições simultaneamente:

\[
x>1
\qquad\text{e}\qquad
x<4.
\]

A conjunção dessas condições pode ser escrita de forma abreviada:

\[
\boxed{1<x<4.}
\]

Essa expressão significa que \(x\) deve estar à direita de \(1\) e à esquerda de \(4\) na reta real.

O número \(2\), por exemplo, satisfaz a condição:

\[
1<2<4.
\]

O mesmo ocorre com \(3{,}5\). Já \(1\) e \(4\) não satisfazem a desigualdade, pois ela exige valores estritamente maiores que o primeiro extremo e estritamente menores que o segundo.

Se a condição for alterada para

\[
1\leq x\leq4,
\]

os próprios números \(1\) e \(4\) também passam a satisfazê-la.

Outras condições podem selecionar números de apenas um lado de uma posição.

Por exemplo,

\[
x\geq2
\]

representa todos os números reais que estão na posição correspondente a \(2\) ou à sua direita.

Já

\[
x<0
\]

representa todos os números reais negativos, localizados à esquerda da origem.

Em cada caso, uma condição de ordem determina quais números pertencem à coleção considerada. A mudança de \(<\) para \(\leq\), ou de \(>\) para \(\geq\), altera a pertinência do número que estabelece o limite da condição.

Dessa maneira, as desigualdades permitem descrever subconjuntos dos números reais por propriedades de suas posições na reta.
