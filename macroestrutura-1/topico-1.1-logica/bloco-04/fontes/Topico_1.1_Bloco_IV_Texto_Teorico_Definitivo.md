# TÓPICO 1.1 — LÓGICA MATEMÁTICA

# BLOCO IV — SENTENÇAS ABERTAS E QUANTIFICADORES

## Texto Teórico

# Parte I — Sentenças Abertas, Variáveis e Domínio

## 1. Da proposição à sentença aberta

Compare as expressões:

\[
5+3=8
\]

e

\[
x+3=8.
\]

Na primeira, tudo aquilo de que precisamos para avaliar a afirmação já está determinado. A operação pode ser efetuada e encontramos \(5+3=8\); portanto, a proposição é verdadeira.

A segunda expressão possui outra estrutura. Enquanto \(x\) não representa um valor específico, ainda não existe um único caso determinado para avaliar. Se colocarmos \(5\) no lugar de \(x\), obtemos \(5+3=8\), que é verdadeira. Se colocarmos \(2\), obtemos \(2+3=8\), que é falsa.

A estrutura

\[
x+3=8
\]

permanece a mesma enquanto variamos o valor atribuído a \(x\). Essa variação é suficiente para produzir afirmações verdadeiras em alguns casos e falsas em outros.

Por isso, enquanto \(x\) continua podendo assumir diferentes valores, não faz sentido atribuir à expressão \(x+3=8\) um único valor lógico. Seu comportamento depende do valor considerado.

Uma expressão declarativa desse tipo recebe o nome de **sentença aberta**.

Podemos dizer, neste estágio, que uma sentença aberta é uma expressão cujo valor lógico depende do valor atribuído a uma variável. Ela contém uma condição que pode ser satisfeita por determinados valores e não satisfeita por outros.

Essa situação não deve ser confundida com simplesmente desconhecer o valor lógico de uma proposição.

Uma proposição pode estar completamente determinada e, ainda assim, sua verificação pode ser difícil. O estudante talvez não saiba imediatamente se uma afirmação matemática complicada é verdadeira ou falsa, mas isso não faz com que a afirmação dependa de uma escolha posterior. Existe uma afirmação específica sendo feita, mesmo antes de sabermos verificá-la.

Em \(x+3=8\), ocorre algo diferente. Não falta apenas conhecimento ao leitor: falta determinar **qual caso está sendo considerado**. A expressão ainda admite diferentes substituições para \(x\), e essas substituições podem modificar seu valor lógico.

A abertura da sentença está, portanto, na própria estrutura da expressão.

### Visual de HTML

**Função conceitual:** tornar perceptível a diferença entre uma proposição determinada e uma sentença aberta, mostrando também que a atribuição de valores à variável produz proposições determinadas que podem ter valores lógicos diferentes.

**Tipo:** tabela comparativa em HTML/CSS.

**Conteúdo exato:**

| Expressão | Situação | Valor lógico |
|---|---|---|
| \(5+3=8\) | proposição determinada | \(V\) |
| \(x+3=8\) | sentença aberta | depende de \(x\) |
| \(2+3=8\) | proposição obtida por atribuição | \(F\) |
| \(5+3=8\) | proposição obtida por atribuição | \(V\) |

**Construção:** três colunas. A primeira apresenta as expressões; a segunda distingue a situação lógica de cada uma; a terceira registra o valor lógico quando ele já está determinado. A linha contendo \(x+3=8\) deve ocupar posição central na comparação, permitindo perceber que ela se distingue das demais justamente porque \(x\) ainda pode variar.

**Ênfase:** a linha da sentença aberta deve receber destaque por estrutura, peso tipográfico ou tratamento discreto de fundo. O destaque deve evidenciar “depende de \(x\)” sem depender apenas de cor.

**Restrições de fidelidade:** não utilizar setas que sugiram uma transformação temporal de \(x\) em números. Não apresentar \(x\) como um valor secreto à espera de descoberta. Não antecipar quantificadores, conjuntos ou conjunto-verdade. A tabela deve permanecer integrada à explicação.

**Implementação preferencial:** HTML/CSS. Não utilizar SVG.

O contraste permite separar duas perguntas que, à primeira vista, poderiam parecer iguais:

> Qual é o valor lógico desta proposição?

e:

> Qual valor lógico obtemos quando determinada escolha é feita para a variável?

A primeira pergunta parte de uma afirmação já determinada. A segunda parte de uma condição aberta a diferentes casos.

## 2. Variável livre, atribuição e predicado

Na expressão \(x+3=8\), a letra \(x\) ocupa uma posição que pode receber diferentes valores. Nesse papel, \(x\) funciona como uma **variável**.

É comum encontrar letras em problemas nos quais existe um valor que queremos descobrir. Nesse caso, a letra pode funcionar como uma incógnita. Por exemplo, podemos procurar qual valor torna verdadeira a igualdade \(x+3=8\).

Mas a possibilidade de resolver essa igualdade não esgota o significado de variável.

Considere outra condição:

\[
x>4.
\]

Não há aqui a necessidade de existir um único “valor escondido” que resolva o problema. Diversos números tornam a afirmação verdadeira, como \(5\), \(7\) e \(10\). Outros, como \(2\) e \(4\), tornam-na falsa.

A função de \(x\) é permitir que a mesma condição seja examinada em diferentes casos. Por isso, identificar automaticamente toda letra com uma incógnita seria estreito demais. Uma incógnita é um possível papel de uma letra; uma variável pode desempenhar um papel mais geral, representando diferentes objetos que entram numa mesma estrutura.

Para trabalhar com essas condições sem precisar reescrevê-las por extenso a cada vez, podemos nomeá-las.

Considere:

\[
P(x):\quad x>4.
\]

A escrita \(P(x)\) representa a condição:

> \(x\) é maior que 4.

Aqui, a letra \(P\) nomeia a condição, enquanto \(x\) indica o objeto ao qual ela está sendo aplicada.

Se escolhemos \(7\), escrevemos \(P(7)\). Isso representa \(7>4\), uma proposição verdadeira.

Se escolhemos \(2\), temos \(P(2)\), isto é, \(2>4\), uma proposição falsa.

Esse ato de escolher um valor para a variável é uma **atribuição**. A atribuição determina um caso particular da condição aberta.

A diferença entre \(P(x)\) e \(P(7)\) não está na propriedade considerada. Nos dois casos, a condição continua sendo “ser maior que 4”. O que muda é que, em \(P(7)\), o objeto ao qual essa condição está sendo aplicada já foi determinado.

Assim, \(P(x)\) permanece aberta a diferentes casos, enquanto \(P(7)\) já é uma afirmação específica que pode ser classificada como verdadeira ou falsa.

Uma expressão como \(P(x)\), que representa uma propriedade ou condição aplicada ao objeto indicado pela variável, pode ser chamada de **predicado**.

O termo é útil porque permite separar duas estruturas que possuem papéis bastante diferentes:

\[
p
\]

e

\[
P(x).
\]

Quando escrevemos \(p\), a letra representa uma proposição inteira. Por exemplo:

\[
p:\quad 7>4.
\]

Nesse uso, \(p\) nomeia uma afirmação já completa.

Em

\[
P(x):\quad x>4,
\]

a situação é diferente. \(P(x)\) não nomeia uma proposição determinada sobre um caso específico. Ele representa uma condição aplicada a um objeto que ainda pode variar.

Podemos resumir a diferença conceitual assim:

\[
p:\quad \text{uma proposição completa;}
\]

\[
P(x):\quad \text{uma condição dependente de }x.
\]

A semelhança das letras não deve esconder a diferença de função.

Enquanto \(x\) permanece disponível para receber diferentes valores em \(P(x)\), dizemos que \(x\) é uma **variável livre**.

A palavra “livre” indica exatamente o aspecto relevante neste momento: a condição ainda não determinou qual dos diferentes valores possíveis ocupará aquela posição.

Em \(P(x): x>4\), podemos examinar \(P(2)\), \(P(5)\), \(P(7)\), \(P(10)\), entre muitos outros casos. Cada atribuição produz uma proposição particular; antes dessa atribuição, \(P(x)\) permanece uma condição aberta.

Mas essa liberdade não significa que qualquer objeto imaginável possa necessariamente ocupar \(x\). Para saber quais substituições fazem sentido, ainda precisamos especificar quais objetos estamos admitindo.

## 3. Domínio e valores admissíveis

Considere novamente:

\[
P(x):\quad x>4.
\]

Sabemos que diferentes valores podem ocupar \(x\). Resta uma questão indispensável: **quais valores estamos autorizados a considerar?**

Podemos estar trabalhando apenas com números inteiros positivos menores que 10. Nesse contexto, os valores \(1,2,3,4,5,6,7,8,9\) são admissíveis. Entre eles, alguns satisfazem a condição \(x>4\) e outros não.

Mas poderíamos adotar outro contexto e considerar apenas números inteiros negativos. A condição \(x>4\) continua exatamente a mesma, porém os casos disponíveis mudam. Nesse novo contexto, nenhum dos valores considerados satisfaz a propriedade.

A condição não foi alterada:

\[
P(x):\quad x>4.
\]

O que mudou foi a coleção de objetos que admitimos como possíveis valores de \(x\).

Essa coleção recebe o nome de **domínio**.

O domínio determina quais objetos podem ocupar a posição da variável. Ele não é apenas uma informação auxiliar acrescentada depois da sentença aberta; faz parte da maneira como a condição deve ser interpretada.

Se um valor não pertence ao contexto que estamos considerando, ele não entra na investigação daquela sentença aberta.

Isso também mostra por que conhecer apenas \(P(x)\) nem sempre é suficiente para saber quais casos estão em jogo. A condição informa o que deve ser testado; o domínio informa **sobre quais objetos esse teste está sendo realizado**.

Considere novamente os dois contextos para \(P(x): x>4\).

Se os valores admissíveis são números inteiros positivos menores que 10, podemos examinar casos como \(P(2)\), \(P(5)\) e \(P(8)\). Alguns são falsos e outros verdadeiros.

Se os valores admissíveis são números inteiros negativos, os casos examinados serão diferentes, e nenhum deles satisfará \(x>4\).

Portanto, mudar o domínio não modifica a propriedade expressa por \(P(x)\), mas modifica os objetos que podem ser colocados à prova. Como consequência, também pode mudar quais valores admissíveis satisfazem aquela condição.

O domínio funciona, assim, como a fronteira dentro da qual a variável pode variar.

Em uma sentença aberta como \(P(x)\), há três elementos que precisam permanecer distintos:

- a **condição** expressa por \(P\);
- a **variável** \(x\), que indica o lugar ocupado pelo objeto considerado;
- o **domínio**, que determina quais objetos podem ocupar esse lugar.

Quando escolhemos um desses objetos e o atribuímos a \(x\), a condição deixa de estar aberta naquele caso particular e obtemos uma proposição determinada, como \(P(7)\).

Enquanto nenhum caso específico é fixado, \(P(x)\) permanece uma condição aberta sobre os valores admissíveis do domínio.

# Parte II — Quantificadores Universal e Existencial

## 1. Da atribuição particular à quantificação

Considere novamente a condição:

\[
P(x):\quad x>4.
\]

Se escolhemos um valor específico para \(x\), obtemos uma proposição determinada. Por exemplo, \(P(7)\) representa \(7>4\), que é verdadeira.

Já \(P(2)\) representa \(2>4\), que é falsa.

Cada uma dessas expressões responde a uma pergunta sobre **um caso particular**. \(P(7)\) informa o que acontece quando o valor considerado é 7; \(P(2)\), quando o valor considerado é 2.

Mas escolher valores um a um não é a única maneira de utilizar uma condição como \(P(x)\).

Podemos querer fazer uma afirmação de outro tipo:

> todos os valores admissíveis satisfazem \(P\);

ou:

> pelo menos um valor admissível satisfaz \(P\).

Nesses casos, não estamos mais fixando previamente um único valor para \(x\). Estamos determinando **como os valores do domínio devem ser considerados em relação à condição**.

Essa operação recebe o nome de **quantificação**.

Um **quantificador** estabelece uma exigência sobre os valores admissíveis da variável. Em vez de escolher um caso específico, ele determina se a condição deve valer para todos os casos ou se basta a existência de ao menos um caso favorável.

Essa mudança altera o papel da variável.

Em \(P(x)\), a variável \(x\) permanece livre: diferentes valores ainda podem ocupar sua posição sem que uma afirmação única tenha sido estabelecida.

Quando a variável é submetida a um quantificador, dizemos que ela está **quantificada**. O quantificador determina de que maneira \(x\) participa da afirmação.

No contexto simples de uma única variável considerado aqui, essa quantificação transforma a condição aberta em uma proposição sobre o domínio. A pergunta deixa de ser apenas:

> o que acontece para este valor de \(x\)?

e passa a ser algo como:

> a condição vale para todos?

ou:

> existe ao menos um caso em que ela vale?

## 2. Quantificador universal

Considere uma condição \(P(x)\) e um domínio já determinado.

Uma possibilidade é exigir que **todos os valores admissíveis** satisfaçam a condição.

Essa exigência pode ser expressa verbalmente como:

> Para todo \(x\), \(P(x)\).

ou, de forma mais explícita:

> Para todo valor admissível de \(x\), a condição \(P(x)\) é satisfeita.

Essa estrutura é representada por:

\[
\forall x\,P(x).
\]

O símbolo \(\forall\) representa o **quantificador universal**.

A palavra “universal” corresponde justamente à força da afirmação: nenhum valor admissível pode ficar de fora da condição.

Assim, \(\forall x\,P(x)\) não significa que muitos valores, a maioria dos valores ou apenas todos os casos examinados até então satisfazem \(P\). A exigência é mais forte:

> **todo valor admissível do domínio deve satisfazer \(P\).**

Considere, por exemplo, um domínio formado apenas pelos números \(1,2,3,4\) e a condição:

\[
P(x):\quad x<5.
\]

Temos \(P(1)\), \(P(2)\), \(P(3)\) e \(P(4)\), e todos esses casos são verdadeiros.

Nesse domínio, a afirmação

\[
\forall x\,P(x)
\]

é verdadeira.

O ponto central, porém, não é o fato de o domínio escolhido possuir poucos valores. O significado lógico de \(\forall\) é que **todos os casos admissíveis precisam respeitar a condição**, seja o domínio pequeno ou muito maior.

Por isso, não devemos confundir o significado de uma afirmação universal com uma técnica de verificação. Em um domínio pequeno, pode ser possível examinar cada caso diretamente. Em outros contextos, isso pode não ser prático ou sequer possível dessa maneira.

O quantificador universal descreve a exigência da afirmação; ele não determina, por si só, como essa afirmação será demonstrada.

O domínio continua sendo indispensável.

A expressão \(\forall x\,P(x)\) deve ser entendida relativamente aos valores que \(x\) pode assumir. “Para todo \(x\)” significa, neste contexto:

> para todo \(x\) admissível no domínio considerado.

Mudar o domínio pode mudar o valor lógico da proposição, mesmo quando a condição \(P(x)\) permanece a mesma.

## 3. Quantificador existencial

Há outra maneira de transformar uma condição aberta numa afirmação sobre o domínio.

Em vez de exigir que todos os valores satisfaçam \(P(x)\), podemos afirmar apenas que existe algum caso favorável.

Verbalmente:

> Existe pelo menos um \(x\) tal que \(P(x)\).

Essa estrutura é representada por:

\[
\exists x\,P(x).
\]

O símbolo \(\exists\) representa o **quantificador existencial**.

A exigência agora é muito diferente da universal.

Em \(\exists x\,P(x)\), não é necessário que todos os valores admissíveis satisfaçam \(P\). Basta que exista **ao menos um** valor admissível para o qual \(P(x)\) seja verdadeira.

Retome:

\[
P(x):\quad x>4.
\]

Considere um domínio em que valores como \(2\), \(5\) e \(7\) sejam admissíveis.

Temos \(P(2): 2>4\), que é falsa, mas \(P(5): 5>4\) e \(P(7): 7>4\) são verdadeiras.

Portanto, nesse domínio,

\[
\exists x\,P(x)
\]

é verdadeira.

A palavra “existe” precisa ser interpretada com cuidado. A afirmação existencial não diz que existe **exatamente um** valor favorável.

Ela permanece verdadeira se houver um, dois, vários ou até mesmo todos os valores do domínio satisfazendo \(P\). Sua exigência é apenas:

> existe pelo menos um.

Quando apresentamos um valor admissível \(a\) para o qual \(P(a)\) é verdadeira, esse caso funciona como um **testemunho** da afirmação existencial.

No exemplo, \(P(7)\) é verdadeira. Assim, o valor \(7\) serve como testemunho de:

\[
\exists x\,P(x).
\]

A palavra “testemunho” apenas registra o papel desempenhado por esse caso: ele mostra concretamente que a existência afirmada não está vazia de exemplos.

A diferença entre os dois quantificadores pode agora ser percebida com precisão.

Em \(\forall x\,P(x)\), todos os valores admissíveis precisam satisfazer \(P\).

Em \(\exists x\,P(x)\), um único caso favorável já é suficiente para satisfazer a exigência existencial.

### Visual de HTML

**Função conceitual:** permitir a comparação simultânea entre as exigências dos quantificadores universal e existencial, tornando perceptível que eles tratam os mesmos valores do domínio de maneiras logicamente diferentes.

**Tipo:** tabela comparativa em HTML/CSS.

**Conteúdo exato:**

| Aspecto | Universal | Existencial |
|---|---|---|
| Símbolo | \(\forall\) | \(\exists\) |
| Leitura principal | para todo | existe pelo menos um |
| Forma | \(\forall x\,P(x)\) | \(\exists x\,P(x)\) |
| Exigência | todos os valores admissíveis satisfazem \(P\) | ao menos um valor admissível satisfaz \(P\) |
| Caso concreto relevante | cada caso precisa respeitar a condição | um caso favorável já testemunha a existência |

**Construção:** três colunas. A primeira apresenta o aspecto comparado; as duas seguintes colocam universal e existencial lado a lado. As linhas “Exigência” e “Caso concreto relevante” devem receber maior destaque tipográfico, pois concentram a diferença conceitual principal.

**Ênfase:** tornar perceptível a oposição entre **todos** e **pelo menos um**. A diferença deve ser comunicada por alinhamento, peso tipográfico e organização, não apenas por cor.

**Restrições de fidelidade:** não incluir regras formais de negação. Não escrever \(\neg\forall\) ou \(\neg\exists\). Não introduzir contraexemplo como categoria desta seção. Não sugerir que \(\forall\) significa “muitos” ou que \(\exists\) significa “exatamente um”. Não utilizar diagramas de conjuntos.

**Implementação preferencial:** HTML/CSS. Não utilizar SVG.

O contraste entre os dois quantificadores não é apenas terminológico. Ele altera profundamente aquilo que precisa ocorrer para que a proposição seja verdadeira.

## 4. Quantificação e forma lógica

Uma condição quantificada pode possuir estrutura interna mais rica do que um único predicado \(P(x)\).

Considere duas condições:

\[
A(x):\quad \text{\(x\) possui a propriedade \(A\);}
\]

\[
B(x):\quad \text{\(x\) possui a propriedade \(B\).}
\]

Podemos querer expressar verbalmente:

> Todo \(A\) é \(B\).

Essa frase não afirma que todo objeto do domínio satisfaz simultaneamente \(A\) e \(B\).

Ela estabelece outra relação:

> sempre que um objeto admissível satisfaz \(A\), ele também satisfaz \(B\).

Para cada valor considerado, temos uma estrutura condicional:

\[
A(x)\to B(x).
\]

Como essa relação deve valer para todos os valores admissíveis, escrevemos:

\[
\forall x\,(A(x)\to B(x)).
\]

A expressão reúne duas estruturas com funções diferentes.

O quantificador \(\forall x\) determina que a condição deve ser considerada para todos os valores admissíveis de \(x\).

Já o condicional \(A(x)\to B(x)\) expressa a relação exigida entre as duas propriedades.

Por isso, a forma lógica de:

> Todo \(A\) é \(B\)

não é:

\[
\forall x\,(A(x)\land B(x)).
\]

Essa expressão afirmaria que todo objeto do domínio é simultaneamente \(A\) e \(B\), o que é uma afirmação muito mais forte e diferente.

O condicional permite restringir a exigência àqueles casos em que \(A(x)\) é satisfeita:

\[
\forall x\,(A(x)\to B(x)).
\]

Considere agora outra frase:

> Existe pelo menos um \(A\) que é \(B\).

Aqui não estamos exigindo uma relação condicional para todos os valores do domínio.

Estamos afirmando a existência de um caso específico que reúna simultaneamente as duas propriedades.

O objeto procurado precisa satisfazer \(A(x)\) e \(B(x)\). Por isso, a conjunção aparece:

\[
A(x)\land B(x).
\]

Como basta a existência de ao menos um caso com essas duas propriedades, escrevemos:

\[
\exists x\,(A(x)\land B(x)).
\]

Novamente, quantificador e conectivo realizam trabalhos diferentes.

Em \(\forall x\,(A(x)\to B(x))\), o quantificador estabelece a extensão da afirmação sobre o domínio; o condicional organiza a relação entre \(A(x)\) e \(B(x)\).

Em \(\exists x\,(A(x)\land B(x))\), o quantificador exige a existência de algum valor admissível; a conjunção estabelece que esse mesmo valor deve satisfazer as duas condições ao mesmo tempo.

O conceito de alcance ajuda a tornar essa organização precisa.

Em \(\forall x\,(A(x)\to B(x))\), a expressão \(A(x)\to B(x)\) está sob o alcance do quantificador universal.

Da mesma forma, em \(\exists x\,(A(x)\land B(x))\), a expressão \(A(x)\land B(x)\) está sob o alcance do quantificador existencial.

Os parênteses tornam visível qual estrutura está sendo quantificada.

Essa organização também evidencia a mudança sofrida pela variável.

Em \(P(x)\), \(x\) permanece livre.

Em \(\forall x\,P(x)\) ou \(\exists x\,P(x)\), \(x\) está quantificada: seu papel dentro da afirmação é determinado pelo quantificador.

No contexto simples de uma única variável considerado aqui, as expressões quantificadas já constituem proposições. Seu valor lógico depende de duas coisas que devem ser mantidas juntas: a condição expressa internamente e o domínio sobre o qual a variável está sendo considerada.

# Parte III — Negação dos Quantificadores e Estrutura do Contraexemplo

## 1. A negação de uma afirmação universal

Considere a condição:

\[
P(x):\quad x<5
\]

e, como valores admissíveis, os números \(1,2,3,4\).

Nesse domínio, todos os valores satisfazem \(P(x)\). Portanto,

\[
\forall x\,P(x)
\]

é verdadeira.

Se incluirmos agora o número \(5\) entre os valores admissíveis, a situação muda. Para esse caso, \(P(5)\) representa \(5<5\), que é falsa.

A afirmação universal exige que **todos** os valores admissíveis satisfaçam \(P\). Por isso, não é necessário encontrar várias falhas para torná-la falsa. Um único valor que não satisfaça a condição já rompe a exigência universal.

No novo domínio, basta o caso \(x=5\).

Assim, negar a afirmação:

> Todos os valores admissíveis satisfazem \(P\)

significa afirmar:

> Existe pelo menos um valor admissível que não satisfaz \(P\).

Essa diferença é importante. A negação de “todos” não é “nenhum”.

Se alguns valores satisfazem \(P\) e um deles não satisfaz, já é verdade dizer:

> Nem todos satisfazem \(P\).

Mas seria falso dizer:

> Nenhum satisfaz \(P\).

No exemplo, \(1\), \(2\), \(3\) e \(4\) satisfazem \(x<5\), enquanto \(5\) não satisfaz. Portanto, a falha da universal não elimina os casos favoráveis; ela exige apenas a existência de ao menos uma exceção.

Podemos traduzir essa estrutura simbolicamente.

A afirmação original é:

\[
\forall x\,P(x).
\]

Sua negação afirma que existe pelo menos um valor admissível para o qual \(P(x)\) é falsa. Em outras palavras, existe um \(x\) que satisfaz \(\neg P(x)\).

Logo,

\[
\neg(\forall x\,P(x))
\equiv
\exists x\,\neg P(x).
\]

As duas mudanças na escrita correspondem exatamente à mudança de significado.

O quantificador passa de \(\forall\) para \(\exists\), porque deixamos de exigir algo sobre todos os casos e passamos a afirmar a existência de uma exceção.

Ao mesmo tempo, \(P(x)\) passa para \(\neg P(x)\), porque o valor procurado deve justamente ser um caso em que a condição original falha.

A equivalência

\[
\neg(\forall x\,P(x))
\equiv
\exists x\,\neg P(x)
\]

não é, portanto, uma regra arbitrária de troca de símbolos. Ela registra aquilo que significa tornar falsa uma afirmação universal.

Essa estrutura também esclarece o papel de um **contraexemplo**.

Se \(\forall x\,P(x)\) afirma que todos os valores admissíveis satisfazem \(P\), então um valor específico \(a\) para o qual \(P(a)\) é falsa mostra que a afirmação universal não pode ser verdadeira.

Nesse caso, \(\neg P(a)\) é verdadeira.

O valor \(a\) funciona, ao mesmo tempo, como uma exceção à universal e como um testemunho da afirmação:

\[
\exists x\,\neg P(x).
\]

É exatamente por isso que ele constitui um contraexemplo.

Um contraexemplo não é apenas “um exemplo diferente” nem qualquer caso que pareça desfavorável. Ele é um caso admissível que realiza concretamente a condição necessária para que a afirmação universal falhe.

## 2. A negação de uma afirmação existencial

Considere novamente:

\[
P(x):\quad x>4.
\]

Suponha que, entre os valores admissíveis, estejam \(2\), \(5\) e \(7\).

Temos \(P(2)\) falsa, mas \(P(5)\) e \(P(7)\) verdadeiras.

Portanto,

\[
\exists x\,P(x)
\]

é verdadeira.

Esse exemplo mostra uma diferença profunda em relação à afirmação universal.

Para tornar falsa uma universal, bastava uma exceção.

Para tornar falsa uma existencial, um caso desfavorável não basta.

O fato de \(P(2)\) ser falsa não elimina a possibilidade de que outro valor satisfaça \(P\). Enquanto houver pelo menos um caso favorável, a afirmação existencial continuará verdadeira.

Assim, para que \(\exists x\,P(x)\) seja falsa, **nenhum** valor admissível pode satisfazer \(P\).

Isso significa que cada valor admissível deve satisfazer a negação da condição:

\[
\neg P(x).
\]

A negação de:

> Existe pelo menos um valor admissível que satisfaz \(P\)

é, portanto:

> Todos os valores admissíveis deixam de satisfazer \(P\).

Simbolicamente,

\[
\neg(\exists x\,P(x))
\equiv
\forall x\,\neg P(x).
\]

Novamente, as duas mudanças na fórmula possuem uma razão precisa.

O quantificador passa de \(\exists\) para \(\forall\), porque negar a existência de qualquer caso favorável exige que a falha ocorra em todos os valores admissíveis.

Ao mesmo tempo, \(P(x)\) passa para \(\neg P(x)\), porque cada um desses valores deve deixar de satisfazer a propriedade original.

A exigência agora pode ser vista de outra maneira.

Para confirmar \(\exists x\,P(x)\), um único testemunho favorável é suficiente.

Para negar essa mesma afirmação, porém, precisamos eliminar a possibilidade de **qualquer** testemunho. Por isso, a negação existencial assume forma universal.

Essa estrutura também permite distinguir duas afirmações que podem parecer semelhantes:

\[
\neg(\exists x\,P(x))
\]

e

\[
\exists x\,\neg P(x).
\]

A primeira significa:

> Nenhum valor admissível satisfaz \(P\).

A segunda significa:

> Existe pelo menos um valor admissível que não satisfaz \(P\).

Retome o domínio com \(2\), \(5\) e \(7\), e a condição \(P(x): x>4\).

Como \(2>4\) é falsa, temos \(\exists x\,\neg P(x)\) verdadeira.

Há pelo menos um valor que não satisfaz \(P\).

Mas \(\neg(\exists x\,P(x))\) é falsa, porque existem valores que satisfazem \(P\), como \(5\) e \(7\).

Portanto, \(\exists x\,\neg P(x)\) não significa que nenhum valor satisfaça \(P\). Significa apenas que ao menos um valor não satisfaz.

Essa diferença revela por que negar somente a propriedade interna, mantendo o mesmo quantificador, não produz a negação correta da proposição inteira.

### Visual de HTML

**Função conceitual:** organizar visualmente a dualidade entre os quantificadores sob negação, mostrando que a negação modifica simultaneamente o quantificador e a propriedade interna.

**Tipo:** tabela comparativa em HTML/CSS.

**Conteúdo exato:**

| Afirmação negada | Forma equivalente | Leitura |
|---|---|---|
| \(\neg(\forall x\,P(x))\) | \(\exists x\,\neg P(x)\) | existe pelo menos uma exceção |
| \(\neg(\exists x\,P(x))\) | \(\forall x\,\neg P(x)\) | todos os casos deixam de satisfazer \(P\) |

**Construção:** três colunas. A primeira apresenta a proposição quantificada sob negação; a segunda apresenta sua forma equivalente; a terceira registra a interpretação verbal que justifica a equivalência.

**Ênfase:** tornar perceptível que as duas equivalências envolvem conjuntamente duas alterações: o quantificador muda entre universal e existencial, e a condição \(P(x)\) passa para \(\neg P(x)\). Essa correspondência deve ser percebida pela organização, pelo alinhamento e por tratamento tipográfico discreto, não apenas por cor.

**Restrições de fidelidade:** não apresentar a tabela como regra mnemônica. Não utilizar setas decorativas entre os símbolos. Não empregar diagramas de conjuntos, múltiplos quantificadores, existência única ou regras de inferência. Não utilizar SVG.

**Implementação preferencial:** HTML/CSS.

A razão das duas equivalências pode ser condensada sem recorrer à memorização.

A universal é negada por uma existência contrária porque uma única exceção basta para romper uma exigência sobre todos:

\[
\neg(\forall x\,P(x))
\equiv
\exists x\,\neg P(x).
\]

A existencial é negada por uma universal contrária porque, para eliminar qualquer testemunho possível, todos os casos precisam falhar:

\[
\neg(\exists x\,P(x))
\equiv
\forall x\,\neg P(x).
\]

## 3. Domínio, alcance e negação da propriedade interna

Ao negar uma afirmação quantificada, a negação não altera silenciosamente o contexto em que a proposição está sendo interpretada.

Considere:

\[
\forall x\,P(x).
\]

Se o domínio estabelece quais valores são admissíveis para \(x\), então sua negação continua falando **desses mesmos valores**.

Negar:

> Todos os valores admissíveis satisfazem \(P\)

significa:

> Entre esses mesmos valores admissíveis, existe pelo menos um que não satisfaz \(P\).

Não seria uma negação correta mudar o domínio e depois procurar uma exceção em outro contexto. A afirmação original e sua negação precisam referir-se aos mesmos objetos admissíveis.

A posição da negação também importa.

Em

\[
\neg(\forall x\,P(x)),
\]

a negação atua sobre a afirmação quantificada completa.

A equivalência

\[
\neg(\forall x\,P(x))
\equiv
\exists x\,\neg P(x)
\]

reorganiza essa estrutura: o quantificador universal torna-se existencial, enquanto a negação passa a atuar sobre a condição \(P(x)\).

Por isso, não basta escrever \(\exists x\,P(x)\). Essa expressão apenas afirma que existe algum caso favorável a \(P\); ela não procura uma exceção à universal.

Da mesma forma, \(\forall x\,\neg P(x)\) é mais forte do que a simples negação da universal. Ela afirma que nenhum valor admissível satisfaz \(P\), quando, para negar a universal, bastaria uma única exceção.

A necessidade de respeitar o alcance torna-se ainda mais visível quando a condição interna possui sua própria estrutura lógica.

Considere:

\[
\forall x\,(A(x)\to B(x)).
\]

Essa proposição expressa:

> Todo \(A\) é \(B\).

Para cada valor admissível, a afirmação exige que, se \(A(x)\) for satisfeita, então \(B(x)\) também seja.

Para negar essa proposição, começamos pela estrutura universal completa:

\[
\neg\left(\forall x\,(A(x)\to B(x))\right).
\]

A negação da universal afirma que existe pelo menos um valor admissível para o qual a condição interna falha:

\[
\neg\left(\forall x\,(A(x)\to B(x))\right)
\equiv
\exists x\,\neg(A(x)\to B(x)).
\]

Agora a questão está concentrada na condição \(A(x)\to B(x)\).

Sua negação já possui uma forma conhecida:

\[
\neg(A(x)\to B(x))
\equiv
A(x)\land\neg B(x).
\]

Substituindo essa equivalência na expressão quantificada, obtemos:

\[
\neg\left(\forall x\,(A(x)\to B(x))\right)
\equiv
\exists x\,\neg(A(x)\to B(x))
\equiv
\exists x\,(A(x)\land\neg B(x)).
\]

O resultado possui uma interpretação precisa.

A expressão

\[
\exists x\,(A(x)\land\neg B(x))
\]

afirma que existe pelo menos um valor admissível que satisfaz \(A\) e, ao mesmo tempo, não satisfaz \(B\).

É exatamente esse tipo de caso que torna falsa a afirmação:

> Todo \(A\) é \(B\).

Não basta encontrar um valor para o qual \(B(x)\) seja falsa. Se esse valor também não satisfizer \(A(x)\), ele não viola a relação condicional.

Também não basta encontrar um valor que satisfaça \(A(x)\). Se ele satisfizer \(B(x)\) igualmente, a exigência continua respeitada.

O contraexemplo precisa reunir as duas condições no **mesmo valor**.

Para um valor admissível \(a\), \(A(a)\) deve ser verdadeira e \(B(a)\) deve ser falsa. Portanto,

\[
A(a)\land\neg B(a)
\]

deve ser verdadeira.

É essa combinação que realiza concretamente a falha do condicional dentro da afirmação universal.

Assim, o padrão

\[
p\land\neg q,
\]

que descreve a falha de um condicional, reaparece agora numa estrutura quantificada. Em vez de trabalhar apenas com proposições inteiras \(p\) e \(q\), procuramos um valor concreto \(a\) do domínio que faça

\[
A(a)\land\neg B(a)
\]

ser verdadeira.

Esse valor é um contraexemplo a:

\[
\forall x\,(A(x)\to B(x)).
\]

Ao mesmo tempo, ele é um testemunho da negação dessa afirmação:

\[
\exists x\,(A(x)\land\neg B(x)).
\]

O contraexemplo, portanto, não constitui uma exceção informal acrescentada de fora do raciocínio. Ele é precisamente um valor do domínio que satisfaz a condição expressa pela negação da afirmação universal.
