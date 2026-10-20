# BLOCO III — INTERVALOS REAIS

# PARTE I — INTERVALOS LIMITADOS E SEUS EXTREMOS

## O intervalo como conjunto de números reais

Considere o conjunto

\[
A=\{x\in\mathbb R\mid 1<x<4\}.
\]

A condição \(1<x<4\) determina quais números reais pertencem a \(A\): são todos aqueles maiores que \(1\) e menores que \(4\).

Os números \(2\) e \(3\), por exemplo, pertencem ao conjunto. Entretanto, \(A\) não contém somente esses dois números. Também pertencem a ele \(1{,}5\), \(\frac52\), \(\sqrt2\) e todos os demais números reais situados estritamente entre \(1\) e \(4\).

Na reta real, esses números ocupam uma região contínua, delimitada pelas posições correspondentes a \(1\) e \(4\). Os extremos determinam a região considerada, embora não pertençam ao conjunto, pois a condição exige que \(x\) seja estritamente maior que \(1\) e estritamente menor que \(4\).

Um conjunto dessa natureza é chamado de **intervalo real**.

A característica fundamental de um intervalo é não apresentar lacunas internas na ordem dos números reais. Isso significa que, se dois números pertencem a um intervalo, todos os números reais situados entre eles também pertencem.

Considere, por exemplo, dois números \(u\) e \(v\) pertencentes a um intervalo \(I\), com \(u<v\). Se um número real \(w\) satisfaz

\[
u<w<v,
\]

então ele também deve pertencer a \(I\):

\[
\boxed{
u,v\in I
\quad\text{e}\quad
u<w<v
\quad\Longrightarrow\quad
w\in I.
}
\]

Essa propriedade caracteriza os intervalos como subconjuntos de \(\mathbb R\) sem lacunas entre seus elementos.

O conjunto

\[
B=\{1,2,3,4\}
\]

não constitui um intervalo real. Embora contenha \(1\) e \(4\), deixa de fora números situados entre eles, como \(1{,}5\).

Já o conjunto \(A\) contém todos os reais entre seus extremos e, por isso, satisfaz a propriedade.

A diferença não está na quantidade de números apresentados na escrita do conjunto, mas na condição que determina quais elementos pertencem a ele.

## Extremos e convenções de pertencimento

A região entre dois números reais pode ser considerada de diferentes maneiras, conforme a inclusão ou exclusão dos extremos.

Sejam \(a,b\in\mathbb R\), com \(a<b\).

Quando selecionamos apenas os números estritamente entre \(a\) e \(b\), obtemos o **intervalo aberto**:

\[
\boxed{
(a;b)=\{x\in\mathbb R\mid a<x<b\}.
}
\]

Os parênteses indicam que nem \(a\) nem \(b\) pertencem ao conjunto.

Assim, o conjunto utilizado anteriormente pode ser escrito de forma abreviada:

\[
A=(1;4).
\]

Essa notação representa exatamente os mesmos elementos que a condição \(1<x<4\).

Entretanto, podemos incluir os dois extremos. Nesse caso, temos o **intervalo fechado**:

\[
\boxed{
[a;b]=\{x\in\mathbb R\mid a\leq x\leq b\}.
}
\]

Os colchetes indicam que \(a\) e \(b\) pertencem ao conjunto.

Por exemplo,

\[
[1;4]
\]

contém todos os números de \((1;4)\) e também os próprios números \(1\) e \(4\).

Existem ainda duas situações intermediárias: podemos incluir somente o extremo esquerdo ou somente o direito.

O **intervalo fechado à esquerda e aberto à direita** é

\[
\boxed{
[a;b)=\{x\in\mathbb R\mid a\leq x<b\}.
}
\]

O **intervalo aberto à esquerda e fechado à direita** é

\[
\boxed{
(a;b]=\{x\in\mathbb R\mid a<x\leq b\}.
}
\]

Observe que o símbolo usado em cada extremidade corresponde diretamente à desigualdade que determina o pertencimento daquele número.

No intervalo \([1;4)\), por exemplo, o número \(1\) pertence ao conjunto, mas \(4\) não pertence.

Já em \((1;4]\), ocorre o contrário: \(1\) está excluído e \(4\) está incluído.

As quatro possibilidades podem ser organizadas pela situação de seus extremos:

| Tipo de intervalo | Notação | Condição |
|---|---|---|
| Aberto | \((a;b)\) | \(a<x<b\) |
| Fechado | \([a;b]\) | \(a\leq x\leq b\) |
| Fechado à esquerda | \([a;b)\) | \(a\leq x<b\) |
| Fechado à direita | \((a;b]\) | \(a<x\leq b\) |

Em todas essas condições, considera-se \(x\in\mathbb R\) e \(a<b\).

A utilização do ponto e vírgula separa os extremos, evitando confusão com a vírgula decimal. Assim,

\[
(1{,}5;3{,}5)
\]

representa os números reais estritamente maiores que \(1{,}5\) e menores que \(3{,}5\).

Algumas obras utilizam outras convenções, como \(]a;b[\) para o intervalo aberto. Neste material, adotaremos preferencialmente os parênteses e colchetes apresentados acima.

## Representação dos intervalos na reta real

Os intervalos podem ser representados por regiões da reta real.

Para distinguir os extremos, utilizaremos uma convenção gráfica:

- **Círculo vazio:** o número correspondente não pertence ao intervalo.
- **Círculo preenchido:** o número correspondente pertence ao intervalo.

A região destacada indica todos os números reais selecionados.

<!-- FIGURA 1 — Especificação editorial: quatro retas horizontais paralelas, utilizando a mesma escala e o mesmo alinhamento para as posições 1 e 4. Em cada reta, destacar todo o segmento entre esses números. Na primeira, utilizar círculos vazios em ambos os extremos; na segunda, preenchidos em ambos; na terceira, preenchido em 1 e vazio em 4; na quarta, vazio em 1 e preenchido em 4. Identificar as linhas, respectivamente, por (1;4), [1;4], [1;4) e (1;4]. Preservar legenda para as convenções gráficas e não depender exclusivamente da cor. -->

*Figura 1 — Os quatro intervalos delimitados por \(1\) e \(4\). A região selecionada permanece entre os mesmos extremos; o preenchimento dos círculos indica quais extremos pertencem ao conjunto.*

A diferença entre essas representações concentra-se nos extremos. Todos os números estritamente entre \(1\) e \(4\) pertencem aos quatro conjuntos, mas os próprios números \(1\) e \(4\) podem ou não pertencer, conforme a notação.

Os extremos, portanto, delimitam os intervalos independentemente de estarem incluídos. Um círculo vazio não significa que exista uma região ausente próxima ao extremo: significa somente que aquele número específico não pertence ao conjunto.

---
# PARTE II — INTERVALOS ILIMITADOS E CASOS ESPECIAIS

## Intervalos com apenas um limite numérico

Um intervalo não precisa estar compreendido entre dois números reais determinados.

Considere a condição

\[
x\geq2.
\]

Ela seleciona o número \(2\) e todos os números reais maiores que ele. Na reta, essa região começa em \(2\), incluindo esse extremo, e se prolonga indefinidamente para a direita.

Representamos esse conjunto por

\[
\boxed{
[2;+\infty)
=
\{x\in\mathbb R\mid x\geq2\}.
}
\]

O símbolo \(+\infty\) indica que não existe um limite superior real para a região selecionada. Por maior que seja um número pertencente ao intervalo, existem outros números reais maiores que ele que também pertencem ao conjunto.

O número \(2\) é seu limite inferior e está incluído, razão pela qual utilizamos um colchete à esquerda.

Considere agora a condição

\[
x<3.
\]

Ela seleciona todos os números reais menores que \(3\), sem incluir o próprio número \(3\). Essa região se prolonga indefinidamente para a esquerda e é representada por

\[
\boxed{
(-\infty;3)
=
\{x\in\mathbb R\mid x<3\}.
}
\]

A posição correspondente a \(3\) delimita a região à direita, mas o número está excluído.

<!-- FIGURA 2 — Especificação editorial: apresentar duas retas horizontais na mesma escala, com orientação positiva à direita. Na primeira, marcar o número 2 por círculo preenchido e destacar a região à sua direita, prolongando-a com uma seta; identificar o intervalo [2;+∞). Na segunda, marcar 3 por círculo vazio e destacar a região à sua esquerda, prolongando-a com seta; identificar (−∞;3). Utilizar a origem 0 como referência comum e manter o alinhamento das posições correspondentes. Não representar +∞ ou −∞ por pontos da reta. -->

*Figura 2 — Intervalos ilimitados. O primeiro inclui \(2\) e se prolonga para a direita; o segundo exclui \(3\) e se prolonga para a esquerda. As setas indicam continuidade ilimitada, não pontos correspondentes a números infinitos.*

As demais possibilidades decorrem da mesma distinção entre desigualdades estritas e não estritas.

Para \(a\in\mathbb R\):

| Condição | Intervalo |
|---|---|
| \(x<a\) | \((-\infty;a)\) |
| \(x\leq a\) | \((-\infty;a]\) |
| \(x>a\) | \((a;+\infty)\) |
| \(x\geq a\) | \([a;+\infty)\) |

Em todas as condições, considera-se \(x\in\mathbb R\).

Esses conjuntos são chamados de **intervalos ilimitados**, pois se prolongam indefinidamente em pelo menos um dos sentidos da reta real.

## O significado dos símbolos de infinito

Embora apareçam na notação dos intervalos ilimitados, os símbolos \(+\infty\) e \(-\infty\) não representam números reais.

Portanto,

\[
\boxed{
+\infty\notin\mathbb R
\qquad\text{e}\qquad
-\infty\notin\mathbb R.
}
\]

Eles indicam a ausência de um limite real em determinada direção.

Quando escrevemos

\[
[2;+\infty),
\]

não estamos afirmando que o intervalo possui um elemento chamado \(+\infty\). Estamos indicando que ele contém todos os reais maiores ou iguais a \(2\), sem apresentar um maior elemento.

Por isso, as notações dos intervalos reais permanecem sempre abertas do lado de \(+\infty\) e \(-\infty\). Não utilizamos um colchete para indicar a inclusão desses símbolos.

Também podemos representar toda a reta real por um intervalo sem limite inferior nem superior:

\[
\boxed{
(-\infty;+\infty)=\mathbb R.
}
\]

Nesse caso, nenhum número real é excluído. O intervalo corresponde à totalidade das posições da reta.

## Intervalos vazios e unitários

As quatro formas de intervalos limitados foram apresentadas considerando dois extremos distintos, \(a<b\).

Quando os extremos coincidem, a situação é diferente.

Considere um número real \(a\) e a condição

\[
a\leq x\leq a.
\]

Para satisfazê-la, \(x\) precisa ser simultaneamente maior ou igual e menor ou igual a \(a\). A única possibilidade é

\[
x=a.
\]

Consequentemente,

\[
\boxed{
[a;a]=\{a\}.
}
\]

Esse conjunto possui um único elemento e é chamado de **intervalo unitário**.

Por exemplo,

\[
[3;3]=\{3\}.
\]

Na reta real, ele corresponde exclusivamente ao ponto associado ao número \(3\).

Considere agora a condição estrita

\[
a<x<a.
\]

Nenhum número real pode ser, ao mesmo tempo, estritamente maior e estritamente menor que o mesmo número \(a\).

Logo,

\[
\boxed{
(a;a)=\varnothing.
}
\]

Pelo mesmo motivo, as condições correspondentes aos intervalos semiabertos com extremos coincidentes também não podem ser satisfeitas:

\[
\boxed{
[a;a)=(a;a]=\varnothing.
}
\]

No primeiro caso, seria necessário satisfazer \(a\leq x<a\); no segundo, \(a<x\leq a\). Ambas as condições são impossíveis.

O conjunto vazio e os conjuntos unitários são admitidos como **intervalos especiais**. Isso é compatível com a propriedade fundamental dos intervalos: não existem dois elementos do conjunto com algum número real intermediário indevidamente excluído.

Em um conjunto unitário, não há dois elementos distintos para os quais essa situação possa ocorrer. No conjunto vazio, não há elementos.

Também podem surgir condições incompatíveis entre extremos diferentes. Por exemplo,

\[
5\leq x\leq2
\]

não é satisfeita por nenhum número real, pois exigiria que \(x\) fosse maior ou igual a \(5\) e, simultaneamente, menor ou igual a \(2\).

O conjunto determinado por essa condição é, portanto, vazio.

## Um intervalo limitado pode ter infinitos elementos

Os termos *limitado* e *finito* expressam propriedades diferentes.

Um conjunto de números reais é **limitado** quando existem números reais que servem como limites inferior e superior para todos os seus elementos.

Isso não exige que esses limites pertençam ao conjunto.

Por exemplo,

\[
[1;2]
\]

é um intervalo limitado, pois todos os seus elementos são maiores ou iguais a \(1\) e menores ou iguais a \(2\).

Entretanto, esse intervalo não é um conjunto finito.

Entre \(1\) e \(2\) encontramos \(1{,}5\); entre \(1\) e \(1{,}5\), encontramos \(1{,}25\); e o mesmo procedimento pode continuar indefinidamente.

A propriedade de existência de números intermediários garante que, entre dois números reais distintos, sempre há outros números reais. Portanto, qualquer intervalo com extremos distintos contém infinitos elementos.

Isso vale tanto para

\[
[1;2]
\]

quanto para

\[
(1;2).
\]

A exclusão dos extremos não altera essa característica.

Assim, um intervalo pode possuir limites numéricos bem determinados e, ainda assim, conter infinitos números reais.

Da mesma forma, não devemos confundir o comprimento da região desenhada com a quantidade de elementos do conjunto. Um segmento pequeno da reta real pode representar infinitos números.

---
# PARTE III — OPERAÇÕES E RELAÇÕES ENTRE INTERVALOS

## Pertinência e inclusão de intervalos

Um intervalo é um conjunto de números reais. Portanto, as relações de pertinência e inclusão também se aplicam a ele.

Para determinar se um número pertence a um intervalo, basta verificar se esse número satisfaz as condições que o definem.

Considere

\[
A=(1;3).
\]

Como \(2\) está estritamente entre \(1\) e \(3\), temos

\[
2\in A.
\]

Entretanto,

\[
1\notin A
\qquad\text{e}\qquad
3\notin A,
\]

pois os extremos estão excluídos.

A relação de inclusão exige uma verificação diferente. Um intervalo \(A\) está contido em outro intervalo \(B\) quando **todos os elementos de \(A\) também pertencem a \(B\)**.

Considere os intervalos

\[
A=(1;3)
\qquad\text{e}\qquad
B=[1;3].
\]

Todo número real que satisfaz \(1<x<3\) também satisfaz \(1\leq x\leq3\).

Portanto,

\[
A\subseteq B.
\]

A inclusão é própria porque \(B\) possui elementos que não pertencem a \(A\): os números \(1\) e \(3\).

Assim,

\[
\boxed{
(1;3)\subsetneq[1;3].
}
\]

Esse exemplo mostra que intervalos com os mesmos extremos numéricos não representam necessariamente o mesmo conjunto.

A relação de inclusão depende dos elementos que cada intervalo contém, inclusive de seus extremos.

## Interseção: elementos que satisfazem duas condições

A interseção de dois intervalos reúne os números reais que pertencem simultaneamente a ambos.

Considere

\[
A=[1;4]
\qquad\text{e}\qquad
B=[3;6].
\]

Para pertencer a \(A\cap B\), um número \(x\) precisa satisfazer as duas condições:

\[
1\leq x\leq4
\]

e

\[
3\leq x\leq6.
\]

Os números que satisfazem ambas são aqueles compreendidos entre \(3\) e \(4\), incluindo os dois extremos.

Consequentemente,

\[
\boxed{
[1;4]\cap[3;6]=[3;4].
}
\]

A região comum pode ser identificada diretamente na reta.

<!-- FIGURA 3 — Especificação editorial: três retas horizontais paralelas, com a mesma orientação e escala. Marcar as posições 1, 3, 4 e 6 de maneira alinhada entre as retas. Na primeira, destacar [1;4]; na segunda, [3;6]; na terceira, [3;4], correspondente a A∩B. Utilizar círculos preenchidos em todos os extremos dos segmentos representados, pois os intervalos são fechados. A região comum deverá aparecer na mesma posição nas três retas. -->

*Figura 3 — Interseção de \(A=[1;4]\) e \(B=[3;6]\). A terceira reta destaca somente a região comum aos dois intervalos.*

A interseção também pode conter apenas um elemento.

Considere

\[
C=[1;3]
\qquad\text{e}\qquad
D=[3;5].
\]

Os intervalos compartilham o número \(3\), mas nenhum outro número pertence aos dois.

Portanto,

\[
\boxed{
[1;3]\cap[3;5]=\{3\}.
}
\]

O resultado é um conjunto unitário.

Entretanto, se o segundo intervalo excluir o número \(3\), a interseção mudará.

Considere

\[
E=(3;5].
\]

O número \(3\) pertence a \([1;3]\), mas não pertence a \(E\). Além disso, todos os números de \(E\) são maiores que \(3\), enquanto os números de \([1;3]\) são menores ou iguais a \(3\).

Não existe, portanto, número real comum aos dois conjuntos:

\[
\boxed{
[1;3]\cap(3;5]=\varnothing.
}
\]

Esses intervalos são chamados de **disjuntos**, pois não possuem elementos em comum.

A comparação evidencia que a interseção não depende apenas da posição geral das regiões na reta. Quando dois intervalos se encontram em uma mesma posição, a inclusão ou exclusão desse número pode determinar se a interseção é unitária ou vazia.

## União: elementos que satisfazem pelo menos uma condição

A união de dois intervalos reúne todos os números reais que pertencem a pelo menos um deles.

Considere

\[
A=[1;3]
\qquad\text{e}\qquad
B=[3;5).
\]

O primeiro intervalo contém todos os números de \(1\) a \(3\), incluindo ambos os extremos. O segundo contém todos os números de \(3\) a \(5\), incluindo \(3\) e excluindo \(5\).

A união reúne essas duas regiões:

\[
\boxed{
[1;3]\cup[3;5)=[1;5).
}
\]

O resultado é um único intervalo. Não há nenhum número real entre \(1\) e \(5\) que tenha sido excluído da união.

Entretanto, **a união de dois intervalos não precisa constituir um único intervalo**.

Considere

\[
C=(1;3)
\qquad\text{e}\qquad
D=(3;5).
\]

O primeiro conjunto contém os reais estritamente entre \(1\) e \(3\); o segundo contém os reais estritamente entre \(3\) e \(5\).

Nenhum deles contém o número \(3\).

Consequentemente,

\[
C\cup D=(1;3)\cup(3;5)
\]

não contém \(3\), embora contenha números menores e maiores que ele.

Como existe uma lacuna nessa posição, o conjunto resultante não é um único intervalo.

A situação muda quando um dos conjuntos inclui o ponto de contato.

Por exemplo,

\[
[1;3]\cap(3;5]=\varnothing,
\]

mas

\[
\boxed{
[1;3]\cup(3;5]=[1;5].
}
\]

A interseção é vazia porque o primeiro intervalo termina em \(3\), enquanto o segundo contém apenas números maiores que \(3\).

Apesar disso, a união não possui lacuna: o número \(3\) pertence ao primeiro intervalo, e todos os números maiores que \(3\) até \(5\) pertencem ao segundo.

Dois intervalos podem, portanto, ser disjuntos e ainda formar um único intervalo quando reunidos.

<!-- FIGURA 4 — Especificação editorial: duas retas paralelas, com escala idêntica e posições 1, 3 e 5 alinhadas. Na primeira, representar a união [1;3]∪(3;5]=[1;5], destacando toda a região de 1 a 5, com círculos preenchidos nos extremos externos. O ponto 3 deverá estar incluído, sem interrupção do segmento selecionado. Na segunda, representar (1;3)∪(3;5) por duas regiões destacadas, uma entre 1 e 3 e outra entre 3 e 5, com círculos vazios em 1, 3 e 5. Tornar perceptível que a exclusão do único ponto 3 impede que o resultado seja um intervalo único. -->

*Figura 4 — Comparação entre duas uniões. A primeira contém o número \(3\) e forma um único intervalo; a segunda exclui esse número e mantém uma lacuna.*

O critério fundamental é verificar se a união contém todos os números reais situados entre quaisquer dois de seus elementos.

Se houver uma lacuna interna, a união não constitui um intervalo único, mesmo que as regiões estejam muito próximas na representação.

## Diferença: elementos preservados após uma exclusão

A diferença entre dois conjuntos reúne os elementos que pertencem ao primeiro, mas não pertencem ao segundo.

Para intervalos \(A\) e \(B\), essa condição pode ser expressa por

\[
\boxed{
x\in A\setminus B
\quad\Longleftrightarrow\quad
x\in A\ \text{e}\ x\notin B.
}
\]

A ordem dos conjuntos é importante: \(A\setminus B\) representa os elementos retirados de \(A\) porque pertencem a \(B\), não o contrário.

Considere

\[
A=[1;5]
\qquad\text{e}\qquad
B=(2;4).
\]

O intervalo \(A\) contém todos os números reais de \(1\) a \(5\), incluindo os extremos.

O intervalo \(B\) contém somente os números estritamente entre \(2\) e \(4\).

Para determinar \(A\setminus B\), precisamos retirar de \(A\) todos os números que pertencem a \(B\).

Isso significa excluir os números que satisfazem

\[
2<x<4.
\]

Os números \(2\) e \(4\), entretanto, não pertencem a \(B\). Como ambos pertencem a \(A\), permanecem no resultado.

Restam duas regiões:

\[
[1;2]
\qquad\text{e}\qquad
[4;5].
\]

Consequentemente,

\[
\boxed{
[1;5]\setminus(2;4)
=
[1;2]\cup[4;5].
}
\]

O resultado não é um único intervalo, porque todos os números estritamente entre \(2\) e \(4\) foram excluídos.

<!-- FIGURA 5 — Especificação editorial: três retas horizontais, com orientação e escala idênticas, mantendo as posições 1, 2, 4 e 5 alinhadas verticalmente. Na primeira, destacar [1;5], com círculos preenchidos em 1 e 5. Na segunda, destacar (2;4), com círculos vazios em 2 e 4. Na terceira, destacar separadamente [1;2] e [4;5], com círculos preenchidos em 1, 2, 4 e 5. Identificar as retas por A, B e A\setminus B, respectivamente. A separação entre as duas regiões restantes deve coincidir exatamente com os números removidos de A. -->

*Figura 5 — Diferença entre \(A=[1;5]\) e \(B=(2;4)\). A terceira reta mostra os elementos que permanecem em \(A\) depois da retirada de \(B\).*

A representação evidencia por que os extremos do conjunto retirado permanecem: não pertenciam a \(B\) e, portanto, não satisfazem a condição de exclusão.

Se o conjunto retirado fosse \([2;4]\), os números \(2\) e \(4\) também desapareceriam. Nesse caso, teríamos

\[
[1;5]\setminus[2;4]
=
[1;2)\cup(4;5].
\]

A alteração dos colchetes modifica os elementos da diferença, embora as regiões gerais representadas continuem semelhantes.

## A forma dos resultados das operações

As operações conjuntistas não precisam produzir conjuntos com a mesma forma dos conjuntos originais.

A interseção de dois intervalos pode ser outro intervalo, um conjunto unitário ou o conjunto vazio. Como admitimos os casos unitários e vazios como intervalos especiais, a interseção continua sendo um intervalo nesse sentido.

Já a união pode produzir um intervalo único ou um conjunto formado por regiões separadas.

A diferença também pode produzir um intervalo, o conjunto vazio ou duas regiões separadas, conforme os elementos removidos.

A distinção pode ser observada nos exemplos:

| Operação | Resultado |
|---|---|
| \([1;4]\cap[3;6]\) | \([3;4]\) |
| \([1;3]\cap[3;5]\) | \(\{3\}\) |
| \([1;3]\cap(3;5]\) | \(\varnothing\) |
| \([1;3]\cup(3;5]\) | \([1;5]\) |
| \((1;3)\cup(3;5)\) | União de dois intervalos separados |
| \([1;5]\setminus(2;4)\) | \([1;2]\cup[4;5]\) |

Esses resultados decorrem das condições de pertencimento de cada operação.

Para a interseção, um número precisa pertencer a ambos os conjuntos. Para a união, basta pertencer a pelo menos um. Para a diferença, precisa pertencer ao primeiro e não ao segundo.

Em todos os casos, **a inclusão ou exclusão dos extremos deve ser verificada pelas condições que definem os conjuntos**, e não apenas pela aparência das regiões desenhadas.

Uma operação entre intervalos sempre produz um conjunto de números reais, mas esse conjunto não precisa ser representável por uma única notação de intervalo.
