# BLOCO II — SUBCONJUNTOS, INCLUSÃO E IGUALDADE

Saber se um objeto pertence a um conjunto permite examinar seus elementos individualmente. Para comparar dois conjuntos, porém, precisamos responder a uma pergunta mais abrangente: **todos os elementos de um deles também pertencem ao outro?**

A pertinência continua sendo a base do raciocínio. O que muda é o alcance da afirmação: deixamos de verificar apenas um objeto e passamos a estabelecer uma condição sobre todos os elementos de uma coleção. Essa passagem permite reconhecer quando um conjunto está incluído em outro e quando ambos possuem exatamente os mesmos elementos.

---

# PARTE I — SUBCONJUNTOS E INCLUSÃO

## De elementos individuais à comparação entre conjuntos

Considere os conjuntos

\[
A=\{2,4\}
\qquad\text{e}\qquad
B=\{1,2,3,4,5\}.
\]

O número \(2\) pertence a \(B\), assim como o número \(4\). Como esses são todos os elementos de \(A\), podemos reunir as duas verificações em uma única afirmação:

> Todo elemento de \(A\) também pertence a \(B\).

O ponto decisivo é a palavra **todo**. A afirmação não trata apenas de alguns elementos escolhidos de \(A\): ela exige que nenhum elemento de \(A\) deixe de pertencer a \(B\).

Em linguagem lógica, essa condição é expressa por

\[
\forall x\,(x\in A\rightarrow x\in B).
\]

Quando ela é satisfeita, dizemos que **\(A\) é subconjunto de \(B\)**, ou que **\(A\) está incluído em \(B\)**, e escrevemos \(A\subseteq B\). Assim, a definição de inclusão é:

\[
\boxed{A\subseteq B
\iff
\forall x\,(x\in A\rightarrow x\in B).}
\]

A direção da implicação importa. Partimos da hipótese de que um objeto pertence a \(A\) e exigimos que ele também pertença a \(B\). Não exigimos que todo elemento de \(B\) pertença a \(A\): no exemplo, \(1\), \(3\) e \(5\) pertencem a \(B\), mas não a \(A\), sem impedir a inclusão.

Objetos que não pertencem a \(A\) não podem contrariar essa condição. Uma falha só ocorreria se algum objeto pertencesse a \(A\) e não pertencesse a \(B\).

Por isso, inclusão não deve ser entendida apenas como uma imagem de algo “dentro” de outra coisa. Seu significado matemático é uma condição de pertencimento: **cada elemento do primeiro conjunto deve ser também elemento do segundo**.

## Pertinência e inclusão: duas perguntas diferentes

Para \(A=\{2,4\}\), compare:

\[
2\in A,
\qquad
\{2\}\subseteq A,
\qquad
\{2\}\notin A.
\]

A primeira afirmação pergunta se o objeto \(2\) é um dos elementos de \(A\). A resposta é afirmativa.

A segunda pergunta se **todos os elementos de \(\{2\}\)** pertencem a \(A\). O único elemento desse conjunto é \(2\), que pertence a \(A\); portanto, a inclusão também é verdadeira.

A terceira pergunta se **o próprio conjunto \(\{2\}\)** é um dos elementos de \(A\). Não é: os elementos de \(A\) são os números \(2\) e \(4\), e nenhum deles é o conjunto \(\{2\}\).

As relações não são intercambiáveis. Em \(a\in A\), examinamos o objeto \(a\) como possível elemento de \(A\). Em \(C\subseteq A\), examinamos os elementos de \(C\) e verificamos se todos pertencem a \(A\).

Essa distinção não significa que um conjunto nunca possa aparecer à esquerda de \(\in\). Considere

\[
C=\{\{2\},4\}.
\]

Agora, \(\{2\}\in C\), pois o conjunto \(\{2\}\) é um dos elementos diretamente indicados entre as chaves externas. Entretanto, \(\{2\}\nsubseteq C\): seu elemento \(2\) não pertence a \(C\).

Portanto, mesmo quando os dois objetos comparados são conjuntos, é preciso distinguir as perguntas: **um deles é elemento do outro, ou todos os seus elementos pertencem ao outro?** A escolha do símbolo depende da relação afirmada, não apenas da presença de chaves.

## Não inclusão e testemunha

Para negar uma inclusão, não precisamos mostrar que todos os elementos do primeiro conjunto estão ausentes do segundo. Precisamos mostrar que a exigência de que **todos pertençam** falha.

Considere

\[
E=\{2,4,6\}
\qquad\text{e}\qquad
F=\{2,4,5\}.
\]

Embora \(2\) e \(4\) pertençam a ambos, o número \(6\) pertence a \(E\) e não pertence a \(F\). Isso basta para concluir que \(E\) não está incluído em \(F\), o que escrevemos como \(E\nsubseteq F\).

O número \(6\) é uma **testemunha da não inclusão**: ele torna concreta a falha da condição universal. Também é um contraexemplo à afirmação de que todo elemento de \(E\) pertence a \(F\).

Em geral, negar que todo elemento de \(A\) pertence a \(B\) equivale a afirmar que existe pelo menos um elemento de \(A\) que não pertence a \(B\):

\[
\boxed{A\nsubseteq B
\iff
\exists x\,(x\in A\land x\notin B).}
\]

Essa equivalência resulta da negação da definição de inclusão. A implicação \(x\in A\rightarrow x\in B\) falha precisamente quando sua hipótese é verdadeira e sua conclusão é falsa. A negação da afirmação universal exige que isso aconteça para algum \(x\).

Não inclusão significa, portanto, **“pelo menos um não pertence”**, e não “nenhum pertence”. Os elementos comuns a \(E\) e \(F\) não anulam o contraexemplo \(6\).

A direção também deve ser preservada na escolha da testemunha. Para refutar \(A\subseteq B\), o elemento precisa estar em \(A\) e faltar em \(B\). Encontrar um elemento de \(B\) ausente de \(A\) refuta a inclusão inversa, \(B\subseteq A\).

## Como justificar uma inclusão

Quando todos os elementos de um conjunto estão enumerados, podemos verificar cada um deles. Foi o que fizemos com \(A=\{2,4\}\). Mas uma inclusão também pode ser justificada diretamente pelas condições que determinam os conjuntos, sem listar seus elementos.

A definição indica o caminho. Para provar \(A\subseteq B\), precisamos mostrar que um objeto, **se pertencer a \(A\)**, necessariamente pertencerá a \(B\). Por isso, começamos com um objeto \(x\) arbitrário e supomos \(x\in A\). A partir dessa hipótese, procuramos concluir \(x\in B\).

**Arbitrário** significa que não escolhemos um elemento com uma característica especial que favoreça a conclusão. O argumento deve valer para qualquer objeto que satisfaça a hipótese \(x\in A\). É isso que permite passar do raciocínio com a letra \(x\) à afirmação sobre todos os elementos.

Considere um domínio \(D\) de números inteiros e os conjuntos

\[
P=\{x\in D\mid x>5\},
\qquad
Q=\{x\in D\mid x>2\}.
\]

Para provar \(P\subseteq Q\), seja \(x\) arbitrário e suponha \(x\in P\). Pela condição que define \(P\), temos \(x\in D\) e \(x>5\). Como todo número maior que \(5\) também é maior que \(2\), segue que \(x>2\). Logo, \(x\) satisfaz as duas condições necessárias para pertencer a \(Q\): está em \(D\) e é maior que \(2\). Portanto, \(x\in Q\).

O raciocínio não dependeu de um valor particular de \(x\). Assim, todo elemento de \(P\) pertence a \(Q\), e concluímos \(P\subseteq Q\).

Verificar apenas que, por exemplo, \(6\) e \(7\) pertencem aos dois conjuntos não substituiria esse argumento. Isso confirmaria casos particulares, mas não explicaria por que nenhum elemento de \(P\) pode ficar fora de \(Q\).

Há uma assimetria entre provar e refutar: **uma inclusão exige cobrir todos os elementos do primeiro conjunto; uma única testemunha basta para refutá-la**. Cobrir todos não significa necessariamente enumerá-los. Um argumento que vale para um elemento arbitrário realiza justamente esse trabalho.

## O próprio conjunto e o conjunto vazio

A inclusão não exige que os conjuntos comparados sejam diferentes. Para qualquer conjunto \(A\),

\[
A\subseteq A.
\]

De fato, todo elemento de \(A\) pertence ao próprio \(A\). A condição da definição está satisfeita. Portanto, o símbolo \(\subseteq\) **permite a igualdade**: afirmar \(A\subseteq B\) não obriga \(B\) a possuir algum elemento além dos que pertencem a \(A\).

Outra consequência da definição é que, para qualquer conjunto \(A\),

\[
\varnothing\subseteq A.
\]

Para compreender essa afirmação, considere o que seria necessário para refutá-la: encontrar um elemento que pertencesse a \(\varnothing\) e não pertencesse a \(A\). Isso é impossível, pois não existe elemento algum em \(\varnothing\). Assim, não há elemento do vazio que viole a condição de inclusão, qualquer que seja o conjunto \(A\).

A definição exige que nenhum elemento do primeiro conjunto fique fora do segundo; ela não exige que o primeiro conjunto tenha elementos. Por isso, a conclusão também vale quando \(A=\varnothing\).

Esse argumento esclarece igualmente o uso do elemento arbitrário: supor \(x\in A\) para examinar suas consequências não é afirmar que \(A\) possui algum elemento. Se \(A\) for vazio, a inclusão já está assegurada pela ausência de qualquer possível contraexemplo.

É essencial distinguir

\[
\varnothing\subseteq A
\qquad\text{de}\qquad
\varnothing\in A.
\]

A primeira afirmação vale para todo conjunto \(A\). A segunda só vale se o próprio conjunto vazio for um elemento de \(A\). Por exemplo, para \(A=\{2,4\}\), temos \(\varnothing\subseteq A\), mas \(\varnothing\notin A\). Já em \(\{\varnothing\}\), o vazio aparece como elemento:

\[
\varnothing\in\{\varnothing\}.
\]

Essa pertinência depende de quais objetos formam o conjunto considerado; a inclusão do vazio não depende disso.

## Encadeando inclusões

Suponha que \(A\subseteq B\) e \(B\subseteq C\). Um elemento de \(A\) pertence a \(B\) pela primeira inclusão; ao pertencer a \(B\), pertence também a \(C\) pela segunda. Portanto,

\[
A\subseteq B
\quad\text{e}\quad
B\subseteq C
\quad\Longrightarrow\quad
A\subseteq C.
\]

Podemos explicitar a demonstração tomando um \(x\) arbitrário e supondo \(x\in A\). As hipóteses fornecem a cadeia

\[
x\in A\ \Longrightarrow\ x\in B\ \Longrightarrow\ x\in C.
\]

Como a conclusão vale para qualquer \(x\) que pertença a \(A\), fica demonstrada a inclusão \(A\subseteq C\). Essa propriedade é chamada de **transitividade da inclusão**.

O encadeamento permite comparar o primeiro e o último conjunto por meio de um conjunto intermediário. Outra situação surge quando o percurso retorna ao conjunto inicial: **o que acontece se \(A\subseteq B\) e também \(B\subseteq A\)?**

---

# PARTE II — IGUALDADE, DUPLA INCLUSÃO E INCLUSÃO PRÓPRIA

## Igualdade: exatamente os mesmos elementos

Se \(A\subseteq B\), nenhum elemento de \(A\) falta em \(B\). Se também \(B\subseteq A\), nenhum elemento de \(B\) falta em \(A\). As duas condições eliminam qualquer possibilidade de um dos conjuntos possuir um elemento que o outro não possua.

Como um conjunto é determinado por seus elementos, essa coincidência significa que \(A\) e \(B\) são o mesmo conjunto.

O **critério extensional de igualdade** expressa precisamente essa ideia: dois conjuntos são iguais se, e somente se, possuem exatamente os mesmos elementos. Em símbolos,

\[
\boxed{A=B
\iff
\forall x\,(x\in A\leftrightarrow x\in B).}
\]

O bicondicional reúne as duas direções: pertencer a \(A\) implica pertencer a \(B\), e pertencer a \(B\) implica pertencer a \(A\). Nenhum objeto pode pertencer a apenas um deles.

Por isso,

\[
\{1,2,3\}=\{3,1,2\}=\{1,2,2,3\}.
\]

A ordem e a repetição modificam a escrita, mas não modificam quais objetos pertencem ao conjunto. O mesmo critério vale quando a diferença entre as representações é maior, como na comparação de uma enumeração com uma descrição por propriedade. O que deve coincidir são os elementos determinados por cada representação.

## Dupla inclusão: critério e método de prova

O critério extensional permite obter um resultado particularmente útil:

\[
\boxed{A=B
\iff
\bigl(A\subseteq B\land B\subseteq A\bigr).}
\]

Esse é o **critério da dupla inclusão**. Ele decorre do significado de igualdade e de inclusão, e sua demonstração exige verificar as duas direções da equivalência.

Primeiro, suponha \(A=B\). Se \(x\in A\), então \(x\in B\), pois os dois nomes indicam o mesmo conjunto. Logo, \(A\subseteq B\). Pelo mesmo motivo, se \(x\in B\), então \(x\in A\), de modo que \(B\subseteq A\). Portanto, a igualdade implica as duas inclusões.

Reciprocamente, suponha \(A\subseteq B\) e \(B\subseteq A\). Para qualquer objeto \(x\), a primeira inclusão garante \(x\in A\rightarrow x\in B\), e a segunda garante \(x\in B\rightarrow x\in A\). Juntas, elas fornecem

\[
x\in A\leftrightarrow x\in B.
\]

Como isso vale para todo \(x\), os conjuntos possuem exatamente os mesmos elementos. Pelo critério extensional, \(A=B\).

A demonstração também fornece um método. Para estabelecer uma igualdade entre conjuntos, podemos dividir o trabalho em duas inclusões. Em uma direção, partimos de um elemento arbitrário do primeiro conjunto e mostramos que ele pertence ao segundo. Na outra, partimos de um elemento arbitrário do segundo e mostramos que ele pertence ao primeiro.

A segunda direção precisa ser justificada: não é consequência automática da primeira. Uma única inclusão ainda permite que o segundo conjunto possua elementos ausentes do primeiro.

Considere, por exemplo,

\[
D=\{1,2,3,4,5\},
\qquad
E=\{2,3,4\},
\]

e

\[
F=\{x\in D\mid 1<x<5\}.
\]

Para mostrar que \(E=F\), é necessário verificar tanto que os elementos enumerados satisfazem a condição quanto que a condição não seleciona nenhum outro elemento do domínio.

**De \(E\) para \(F\).** Seja \(x\in E\). Então \(x\) é \(2\), \(3\) ou \(4\). Em qualquer desses casos, \(x\in D\) e \(1<x<5\). Portanto, \(x\in F\), o que prova \(E\subseteq F\).

**De \(F\) para \(E\).** Seja \(x\in F\). Então \(x\in D\) e \(1<x<5\). Entre os elementos de \(D\), o número \(1\) não satisfaz \(1<x\), e o número \(5\) não satisfaz \(x<5\). Restam apenas \(2\), \(3\) e \(4\), todos pertencentes a \(E\). Logo, \(x\in E\), o que prova \(F\subseteq E\).

Pela dupla inclusão, \(E=F\). As duas direções desempenharam funções complementares: a primeira mostrou que a condição não deixa de selecionar nenhum elemento enumerado; a segunda mostrou que ela não seleciona elementos adicionais.

## Inclusão própria: inclusão sem igualdade

Uma inclusão \(A\subseteq B\) admite duas situações: os conjuntos podem ser iguais, ou \(B\) pode possuir algum elemento que não pertence a \(A\). Para distinguir a segunda situação, dizemos que **\(A\) é subconjunto próprio de \(B\)** e escrevemos \(A\subsetneq B\).

Por definição,

\[
\boxed{A\subsetneq B
\iff
\bigl(A\subseteq B\land A\neq B\bigr).}
\]

Não basta afirmar que os conjuntos são diferentes. É preciso também garantir que todos os elementos de \(A\) pertencem a \(B\).

Uma vez estabelecido \(A\subseteq B\), a desigualdade só pode ocorrer porque algum elemento de \(B\) não pertence a \(A\). De fato, a inclusão já impede que exista um elemento de \(A\) ausente de \(B\). Se também não existisse elemento de \(B\) ausente de \(A\), teríamos a inclusão inversa e, pela dupla inclusão, a igualdade.

Obtemos, assim, uma caracterização útil para justificar a inclusão própria:

\[
A\subsetneq B
\iff
\Bigl(A\subseteq B\land
\exists x\,(x\in B\land x\notin A)\Bigr).
\]

As duas exigências têm funções distintas: a inclusão garante que nenhum elemento de \(A\) fica fora de \(B\); a testemunha em \(B\) garante que os conjuntos não são iguais.

Retome

\[
A=\{2,4\},
\qquad
B=\{1,2,3,4,5\}.
\]

Já sabemos que \(A\subseteq B\). Além disso, \(1\in B\) e \(1\notin A\). Portanto, \(A\subsetneq B\). Bastaria qualquer uma dessas testemunhas: \(1\), \(3\) ou \(5\); não é necessário apresentar todas.

Observe a direção da testemunha: um elemento de \(B\) ausente de \(A\) refuta \(B\subseteq A\). Junto de \(A\subseteq B\), isso estabelece a inclusão própria. Se a testemunha estivesse em \(A\) e faltasse em \(B\), ela destruiria a própria inclusão que pretendíamos provar.

O conjunto vazio também permite reconhecer essa distinção. Se \(B\) possui algum elemento, então \(\varnothing\subsetneq B\): o vazio está incluído em \(B\), e qualquer elemento de \(B\) testemunha que eles são diferentes. Se \(B=\varnothing\), há inclusão e igualdade, mas não inclusão própria.

Portanto, \(A\subseteq B\) afirma que todo elemento de \(A\) pertence a \(B\), deixando em aberto a possibilidade de igualdade. A inclusão inversa resolve essa possibilidade afirmativamente, produzindo \(A=B\). Já uma testemunha em \(B\) ausente de \(A\), acompanhada da inclusão inicial, estabelece \(A\subsetneq B\).
