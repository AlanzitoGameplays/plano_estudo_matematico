# BLOCO I — CONJUNTOS, ELEMENTOS E REPRESENTAÇÃO

Uma condição matemática pode separar objetos de um domínio. Se uma sentença aberta \(P(x)\) é considerada em um domínio \(D\), alguns objetos de \(D\) satisfazem essa condição e outros não. Até aqui, o interesse pode estar em cada objeto individualmente: para um valor particular de \(x\), pergunta-se se \(P(x)\) é verdadeira ou falsa.

Há, porém, outro passo possível. Em vez de olhar separadamente para cada objeto que satisfaz a condição, podemos considerar **todos eles em conjunto** e tratar essa coleção como uma única entidade matemática.

Essa mudança parece simples, mas é estruturalmente importante. Os objetos não deixam de existir individualmente; eles passam também a ser considerados como elementos de algo novo. É esse novo objeto que chamamos de **conjunto**.

A lógica permite selecionar objetos segundo condições. A linguagem dos conjuntos permite **objetificar essa seleção**: aquilo que antes era apenas uma coleção de objetos que satisfaziam determinada condição passa a poder ser nomeado, representado, comparado e, posteriormente, relacionado a outros conjuntos.

Antes de realizar essas operações, entretanto, é necessário compreender com precisão três ideias elementares: **o que é um conjunto, o que são seus elementos e o que significa um objeto pertencer a um conjunto**.

---

# PARTE I — CONJUNTOS, ELEMENTOS E PERTINÊNCIA

## Conjunto e elemento

Um **conjunto** é uma coleção matematicamente determinada de objetos considerada como uma unidade.

A expressão “matematicamente determinada” é importante. Não basta reunir objetos de maneira vaga: deve existir algum critério que permita compreender quais objetos fazem parte da coleção considerada.

Imagine, por exemplo, que \(A\) seja o conjunto formado pelos números

\[
2,\quad 4,\quad 6,\quad 8.
\]

Cada um desses números é um **elemento** de \(A\).

O número \(4\) é um objeto matemático. O conjunto \(A\), por outro lado, é outro objeto matemático: uma coleção que possui \(4\), além de outros números, como elementos.

Essa diferença entre o conjunto e aquilo que pertence a ele precisa permanecer clara:

\[
\text{objeto}
\qquad\neq\qquad
\text{conjunto que contém o objeto}.
\]

Um conjunto pode receber um nome, normalmente indicado por uma letra maiúscula como \(A\), \(B\) ou \(C\). Seus elementos podem ser números, pontos, palavras, figuras, outros conjuntos ou qualquer outro tipo de objeto cuja presença na coleção esteja suficientemente determinada.

A natureza dos elementos não define, por si só, o que é um conjunto. O aspecto fundamental é que determinados objetos sejam considerados conjuntamente como elementos de uma mesma coleção.

## Pertinência

Para expressar a relação entre um objeto e um conjunto, utiliza-se a relação de **pertinência**.

Se \(a\) é elemento de um conjunto \(A\), escrevemos

\[
a\in A,
\]

e lemos:

> **\(a\) pertence a \(A\)**

ou:

> **\(a\) é elemento de \(A\).**

Voltando ao conjunto formado pelos números \(2,4,6,8\), podemos escrever:

\[
4\in A.
\]

Essa expressão não afirma que \(4\) e \(A\) sejam objetos do mesmo tipo. Pelo contrário: ela relaciona dois níveis diferentes. À esquerda está um objeto; à direita, um conjunto. O símbolo \(\in\) informa que o primeiro aparece como elemento do segundo.

Se um objeto não pertence ao conjunto, utiliza-se o símbolo \(\notin\).

Assim, se \(5\) não é um dos elementos de \(A\),

\[
5\notin A.
\]

A expressão é lida:

> **\(5\) não pertence a \(A\).**

Pertinência é, portanto, uma relação entre:

\[
\boxed{\text{objeto}\longleftrightarrow\text{conjunto}}.
\]

Essa característica será importante mais adiante, porque nem toda relação envolvendo conjuntos será uma relação de pertinência.

## O conjunto é determinado por seus elementos

Quando um conjunto é considerado, interessa **quais objetos são seus elementos**. A ordem em que esses objetos são mencionados não altera a coleção.

Se uma coleção possui exatamente os elementos \(2\), \(4\), \(6\) e \(8\), mencionar esses objetos na ordem

\[
2,\ 4,\ 6,\ 8
\]

ou na ordem

\[
8,\ 2,\ 6,\ 4
\]

não produz conjuntos diferentes. Os elementos continuam sendo exatamente os mesmos.

Da mesma forma, repetir a menção a um elemento não cria um novo elemento. Se o número \(4\) pertence ao conjunto, escrevê-lo várias vezes não faz com que existam “vários elementos \(4\)” dentro desse conjunto.

Em outras palavras, para determinar um conjunto, interessa **a presença ou ausência de cada elemento**, e não:

- a posição em que ele foi escrito;
- quantas vezes foi repetido na representação.

Essa propriedade diferencia a estrutura de um conjunto de estruturas nas quais ordem ou repetição podem possuir significado próprio.

O ponto essencial é simples:

\[
\boxed{\text{um objeto pertence ou não pertence ao conjunto}.}
\]

A pertinência não possui intensidade nem multiplicidade. Uma vez estabelecido que \(a\in A\), repetir a escrita de \(a\) não altera essa relação.

> **[VISUAL PARA HTML — 1: CONDIÇÃO → CONJUNTO]**  
> Recurso esquemático destinado a tornar perceptível a passagem
> \[
> D\rightarrow P(x)\rightarrow\text{objetos que satisfazem }P\rightarrow A.
> \]
> O esquema deve evidenciar que uma condição seleciona objetos do domínio e que a coleção formada pelos objetos selecionados passa a ser considerada como um único conjunto. A fidelidade exigida é relacional, não métrica.

Compreendida a relação entre um objeto e um conjunto, surge uma questão natural: **como indicar precisamente quais elementos formam determinado conjunto?**

É isso que exige formas adequadas de representação.

---

# PARTE II — FORMAS DE REPRESENTAR UM CONJUNTO

Um conjunto é um objeto matemático; sua escrita é uma **representação** desse objeto.

Essa distinção evita uma confusão importante. As chaves, os símbolos e as palavras utilizadas para apresentar um conjunto não são o próprio conjunto. São maneiras de indicar quais objetos o constituem.

Dependendo da natureza do conjunto, algumas formas de representação são mais convenientes do que outras.

## Representação por enumeração

Quando os elementos de um conjunto podem ser apresentados explicitamente, podemos escrevê-los entre chaves.

Se \(A\) possui como elementos os números \(2,4,6,8\), escrevemos:

\[
A=\{2,4,6,8\}.
\]

Essa forma é chamada de **representação por enumeração**.

As chaves indicam que os objetos escritos em seu interior estão sendo considerados conjuntamente como elementos do conjunto.

Agora a relação de pertinência pode ser lida diretamente na representação:

\[
2\in A,\qquad
6\in A,
\]

enquanto:

\[
3\notin A,\qquad
10\notin A.
\]

É importante não confundir as chaves com uma ideia de ordem. Como a ordem dos elementos não altera o conjunto,

\[
\{2,4,6,8\}
=
\{8,6,4,2\}.
\]

A igualdade escrita aqui apenas registra o fato intuitivo de que ambas as expressões apresentam a mesma coleção de elementos.

Também não há efeito matemático em repetir elementos:

\[
\{2,4,4,6,8,8\}
=
\{2,4,6,8\}.
\]

A segunda escrita é naturalmente preferível porque evita informação visual redundante, mas ambas indicam os mesmos elementos.

A enumeração funciona muito bem quando a coleção possui poucos elementos e todos podem ser escritos sem dificuldade.

Entretanto, nem sempre isso é conveniente.

Suponha que desejemos considerar, dentro de um domínio muito grande, todos os objetos que satisfazem determinada propriedade. Listá-los individualmente pode ser trabalhoso ou até impossível.

Nesse caso, em vez de perguntar:

> **Quais elementos devo escrever um por um?**

podemos perguntar:

> **Que condição caracteriza exatamente os elementos do conjunto?**

Essa mudança leva a outra forma de representação.

## Representação por propriedade

Considere um domínio \(D\) e uma condição \(P(x)\).

Dentro de \(D\), alguns objetos satisfazem \(P(x)\). Podemos formar um conjunto \(A\) contendo precisamente esses objetos.

Escrevemos:

\[
A=\{x\in D\mid P(x)\}.
\]

Essa expressão pode ser lida como:

> **\(A\) é o conjunto dos objetos \(x\) pertencentes ao domínio \(D\) tais que \(P(x)\) é verdadeira.**

Cada parte da escrita possui uma função.

Em

\[
\{x\in D\mid P(x)\},
\]

o símbolo \(x\) representa um objeto variável do domínio.

A expressão

\[
x\in D
\]

informa onde esse objeto está sendo considerado.

A barra vertical

\[
\mid
\]

é lida como **“tal que”**.

Por fim,

\[
P(x)
\]

é a condição utilizada para selecionar, entre os objetos do domínio, aqueles que serão elementos do conjunto.

A representação por propriedade realiza, portanto, a passagem:

\[
\boxed{
\text{domínio}
\rightarrow
\text{condição}
\rightarrow
\text{elementos selecionados}
\rightarrow
\text{conjunto}.
}
\]

Essa é precisamente a ligação entre a linguagem lógica e a linguagem dos conjuntos.

## Condição e pertinência

Se

\[
A=\{x\in D\mid P(x)\},
\]

então, para um objeto \(a\) pertencente ao domínio \(D\), perguntar se \(a\) pertence a \(A\) é o mesmo que perguntar se \(a\) satisfaz a condição utilizada para formar o conjunto.

Assim:

\[
a\in A
\iff
P(a),
\qquad\text{para }a\in D.
\]

Essa equivalência merece ser lida, e não apenas observada simbolicamente.

O lado esquerdo,

\[
a\in A,
\]

é uma afirmação sobre **pertinência**.

O lado direito,

\[
P(a),
\]

é uma afirmação sobre a **condição**.

A equivalência mostra que essas duas perspectivas descrevem a mesma seleção.

### Um exemplo

Considere como domínio \(D\) os números inteiros de \(1\) a \(10\), e seja \(P(x)\) a condição:

> \(x\) é par.

Podemos formar o conjunto:

\[
A=\{x\in D\mid x\text{ é par}\}.
\]

Pela própria condição,

\[
A=\{2,4,6,8,10\}.
\]

As duas expressões representam o mesmo conjunto.

Na primeira, seus elementos são determinados por uma propriedade:

\[
A=\{x\in D\mid x\text{ é par}\}.
\]

Na segunda, os elementos são apresentados explicitamente:

\[
A=\{2,4,6,8,10\}.
\]

Agora considere o objeto \(6\).

Como \(6\in D\) e \(6\) satisfaz a condição “ser par”,

\[
6\in A.
\]

Para \(7\), ocorre o contrário. Embora \(7\in D\), a condição não é satisfeita. Logo,

\[
7\notin A.
\]

O exemplo mostra que a representação por propriedade não cria outro conjunto. Ela apenas descreve a mesma coleção por meio da condição que determina seus elementos.

## Um mesmo conjunto, diferentes representações

Um conjunto pode ser comunicado de diferentes maneiras.

Considere novamente o conjunto dos números pares entre \(1\) e \(10\).

Podemos descrevê-lo verbalmente:

> o conjunto dos números pares de \(1\) a \(10\);

podemos enumerá-lo:

\[
\{2,4,6,8,10\};
\]

ou podemos expressá-lo por propriedade:

\[
\{x\in D\mid x\text{ é par}\},
\]

onde \(D\) é o domínio formado pelos números inteiros de \(1\) a \(10\).

O objeto matemático é o mesmo. O que muda é a maneira pela qual seus elementos são especificados.

Essa capacidade de passar de uma representação para outra será importante ao longo da Matemática. Algumas propriedades ficam mais visíveis em uma forma; outras ficam mais claras em outra.

A enumeração evidencia diretamente cada elemento. A representação por propriedade evidencia o **critério comum** que os reúne.

> **[VISUAL PARA HTML — 2: DIFERENTES REPRESENTAÇÕES DO MESMO CONJUNTO]**  
> Composição simples relacionando três registros de um mesmo conjunto:
> - descrição verbal;
> - enumeração;
> - representação por propriedade.  
> O objetivo é tornar perceptível que as três formas apontam para o mesmo objeto matemático. O recurso deve ser conceitual e simbólico, sem decoração adicional.

Até aqui, os exemplos utilizados podem sugerir que um conjunto sempre precisa possuir vários elementos simples. Essa impressão é enganosa.

Um conjunto pode não possuir elemento algum. Pode possuir exatamente um elemento. E esse elemento pode ser, ele próprio, outro conjunto.

Compreender esses casos exige atenção aos diferentes **níveis de estrutura**.

---

# PARTE III — CONJUNTO VAZIO, CONJUNTO UNITÁRIO E NÍVEIS DE ESTRUTURA

## Quando nenhum objeto satisfaz a condição

Considere um domínio \(D\) e uma condição \(P(x)\).

É possível que nenhum objeto do domínio satisfaça essa condição.

Nesse caso, a coleção formada pelos objetos que satisfazem \(P(x)\) não possui elementos.

Ainda assim, essa coleção é um conjunto perfeitamente legítimo.

O conjunto que não possui nenhum elemento é chamado de **conjunto vazio** e é representado por:

\[
\varnothing.
\]

Pode-se encontrar também a escrita

\[
\{\},
\]

mas adotaremos \(\varnothing\) como notação principal.

O conjunto vazio não é uma espécie de “nada fora da Matemática”. Ele é um objeto matemático bem determinado: o conjunto caracterizado justamente pela ausência de elementos.

Isso significa que, para qualquer objeto \(a\),

\[
a\notin\varnothing.
\]

Não existe objeto algum que pertença ao conjunto vazio.

É importante também observar que o símbolo

\[
\varnothing
\]

representa o próprio conjunto vazio. Não é necessário colocar esse símbolo dentro de chaves para “transformá-lo em conjunto”. Fazer isso produziria outra estrutura, como veremos adiante.

## Quando existe exatamente um elemento

Um conjunto também pode possuir apenas um elemento.

Se o único elemento de um conjunto \(A\) é o objeto \(a\), escrevemos:

\[
A=\{a\}.
\]

Um conjunto desse tipo é chamado de **conjunto unitário**.

Aqui aparece uma distinção estrutural decisiva:

\[
a
\neq
\{a\}.
\]

O objeto \(a\) e o conjunto cujo único elemento é \(a\) não são a mesma coisa.

Se \(a\) for, por exemplo, o número \(5\), então

\[
5
\]

é um número, enquanto

\[
\{5\}
\]

é um conjunto que possui o número \(5\) como elemento.

Podemos expressar a relação entre eles escrevendo:

\[
5\in\{5\}.
\]

Mas isso não autoriza substituir um pelo outro.

A presença das chaves modifica o nível estrutural do objeto considerado.

## Um conjunto pode ser elemento de outro conjunto

Nada exige que os elementos de um conjunto sejam objetos que não sejam conjuntos.

Um conjunto pode aparecer como elemento de outro.

Considere:

\[
a,
\qquad
\{a\},
\qquad
\{\{a\}\}.
\]

Essas três expressões representam três objetos diferentes.

Primeiro:

\[
a
\]

é simplesmente o objeto \(a\).

Depois:

\[
\{a\}
\]

é um conjunto cujo elemento é \(a\).

Finalmente:

\[
\{\{a\}\}
\]

é um conjunto cujo elemento é o conjunto \(\{a\}\).

A estrutura pode ser acompanhada camada por camada:

\[
a\in\{a\},
\]

porque \(a\) é elemento do conjunto \(\{a\}\).

Entretanto,

\[
a\notin\{\{a\}\},
\]

porque o elemento diretamente presente em \(\{\{a\}\}\) não é \(a\), mas sim \(\{a\}\).

Por isso,

\[
\{a\}\in\{\{a\}\}.
\]

Essas relações podem parecer sutis no início, mas resultam de uma única pergunta:

> **Qual é exatamente o objeto que aparece como elemento entre as chaves externas?**

Essa pergunta permite “ler” estruturas com vários níveis sem depender apenas da aparência visual.

### Lendo as chaves

Considere:

\[
\{\{a\}\}.
\]

As chaves externas delimitam o conjunto que estamos examinando.

Dentro delas aparece um único objeto:

\[
\{a\}.
\]

Esse objeto já é, por sua vez, um conjunto.

Logo, o elemento do conjunto externo é:

\[
\{a\},
\]

e não \(a\).

O objeto \(a\) aparece um nível mais profundamente: ele é elemento de \(\{a\}\), que por sua vez é elemento de \(\{\{a\}\}\).

É útil imaginar essas camadas não como simples “parênteses decorativos”, mas como mudanças reais no objeto matemático.

Cada novo par de chaves cria um novo conjunto.

Assim, em geral, não devemos identificar:

\[
a,\qquad
\{a\},\qquad
\{\{a\}\}.
\]

Eles ocupam níveis estruturais diferentes.

## O conjunto vazio e o conjunto que contém o vazio

A mesma distinção permite compreender um caso especialmente importante:

\[
\varnothing
\]

e:

\[
\{\varnothing\}.
\]

O primeiro é o conjunto vazio.

Ele não possui elemento algum.

O segundo é um conjunto que possui um elemento — e esse elemento é justamente o conjunto vazio.

Portanto:

\[
\varnothing
\neq
\{\varnothing\}.
\]

Além disso,

\[
\varnothing\in\{\varnothing\}.
\]

Essa última expressão não contradiz o fato de que o conjunto vazio não possui elementos.

Ela afirma algo diferente.

Dizer que

\[
\varnothing
\]

não possui elementos significa que **nenhum objeto pertence a \(\varnothing\)**.

Dizer que

\[
\varnothing\in\{\varnothing\}
\]

significa que o próprio conjunto vazio foi colocado como elemento de outro conjunto.

Os dois enunciados tratam de conjuntos diferentes.

Essa distinção é um exemplo claro de por que a leitura estrutural das chaves é mais importante do que uma interpretação apenas visual da expressão.

> **[VISUAL PARA HTML — 3: NÍVEIS DE ESTRUTURA]**  
> Recurso estrutural destinado a tornar perceptíveis as diferenças entre
> \[
> a,\qquad \{a\},\qquad \{\{a\}\}
> \]
> e entre
> \[
> \varnothing,\qquad\{\varnothing\}.
> \]
> A composição deve evidenciar as camadas de chaves e identificar somente os elementos diretamente pertencentes a cada conjunto. A fidelidade requerida é estrutural e relacional; proporção ou tamanho visual não possui significado matemático.

A linguagem construída até aqui já permite tratar conjuntos como objetos matemáticos com identidade própria. Podemos:

- reconhecer seus elementos;
- afirmar pertinência ou não pertinência;
- representá-los de diferentes maneiras;
- considerar conjuntos sem elementos;
- considerar conjuntos com um único elemento;
- considerar conjuntos cujos elementos também são conjuntos.

Em particular, a expressão

\[
A=\{x\in D\mid P(x)\}
\]

pode agora ser lida estruturalmente.

\(A\) nomeia um conjunto.

\(D\) é o domínio no qual os objetos estão sendo considerados.

\(x\) representa um possível objeto desse domínio.

\(P(x)\) é a condição que seleciona quais desses objetos serão elementos de \(A\).

Para um objeto \(a\in D\),

\[
a\in A
\iff
P(a).
\]

O conjunto transforma, assim, uma seleção determinada por uma condição em um objeto matemático que pode ser nomeado e estudado.

Até aqui, a relação fundamental ocorreu entre **um objeto e um conjunto**:

\[
a\in A.
\]

O próximo problema nasce quando deixamos de perguntar apenas se um objeto pertence a uma coleção e passamos a comparar **uma coleção inteira com outra**.

A pertinência continuará sendo a base dessa comparação, mas a relação entre conjuntos exigirá uma nova linguagem.
