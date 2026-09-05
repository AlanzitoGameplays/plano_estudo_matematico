# TÓPICO 1.1 — LÓGICA MATEMÁTICA

# BLOCO IV — SENTENÇAS ABERTAS E QUANTIFICADORES

## Texto Prático

# Exemplos Resolvidos

## Exemplo 1 — Do domínio às afirmações quantificadas

Considere a condição:

\[
P(x):\quad x+1>0.
\]

Os valores admissíveis para \(x\) são:

\[
-2,\quad -1,\quad 0,\quad 2,\quad 5.
\]

Organize a investigação desses casos e, a partir dela, determine:

- quais atribuições tornam \(P(x)\) verdadeira;
- quais a tornam falsa;
- o valor lógico de
  \[
  \forall x\,P(x);
  \]
- o valor lógico de
  \[
  \exists x\,P(x);
  \]
- quais valores podem funcionar como testemunhos da afirmação existencial;
- quais valores constituem exceções à afirmação universal.

A ideia é construir **uma única análise do domínio** e utilizá-la para responder às diferentes perguntas.

### Resolução

A condição

\[
P(x):\quad x+1>0
\]

ainda depende do valor atribuído a \(x\). Por isso, antes de decidir qualquer afirmação global, precisamos saber como \(P(x)\) se comporta nos casos que realmente pertencem ao problema.

Os únicos valores admissíveis são:

\[
-2,\quad -1,\quad 0,\quad 2,\quad 5.
\]

Não precisamos procurar outros números. Toda a investigação será feita com esses cinco casos.

Comecemos pelas atribuições.

Para \(x=-2\),

\[
P(-2)
\]

representa:

\[
-2+1>0,
\]

isto é,

\[
-1>0.
\]

Essa proposição é falsa. Portanto,

\[
P(-2)=F.
\]

Para \(x=-1\),

\[
P(-1)
\]

representa:

\[
-1+1>0,
\]

isto é,

\[
0>0,
\]

que também é falsa. Logo,

\[
P(-1)=F.
\]

Os demais casos podem ser avaliados da mesma maneira:

\[
P(0):\quad 0+1>0,
\]

portanto,

\[
P(0)=V;
\]

\[
P(2):\quad 2+1>0,
\]

portanto,

\[
P(2)=V;
\]

\[
P(5):\quad 5+1>0,
\]

portanto,

\[
P(5)=V.
\]

Assim, o perfil completo das avaliações é:

\[
P(-2)=F,\qquad
P(-1)=F,\qquad
P(0)=V,\qquad
P(2)=V,\qquad
P(5)=V.
\]

Agora não precisamos começar uma nova investigação para cada quantificador. Podemos simplesmente **ler esse perfil de maneiras diferentes**.

Para a afirmação universal:

\[
\forall x\,P(x),
\]

a pergunta relevante é:

> Todos os valores admissíveis produziram uma proposição verdadeira?

Não.

Os valores:

\[
-2
\]

e:

\[
-1
\]

produziram proposições falsas.

Logo,

\[
\boxed{\forall x\,P(x)\text{ é falsa}.}
\]

Os valores \(-2\) e \(-1\) constituem exceções à exigência universal.

Agora considere a afirmação existencial:

\[
\exists x\,P(x).
\]

A pergunta passa a ser:

> Existe pelo menos um valor admissível para o qual \(P(x)\) é verdadeira?

Sim.

Temos, por exemplo,

\[
P(0)=V.
\]

Portanto,

\[
\boxed{\exists x\,P(x)\text{ é verdadeira}.}
\]

O valor \(0\) já seria suficiente como testemunho. Mas ele não é o único:

\[
0,\quad2,\quad5
\]

são todos testemunhos possíveis da afirmação existencial.

### Visual para HTML

**Função conceitual:** mostrar que uma única tabela de avaliações individuais pode servir de base para duas leituras globais diferentes: a universal e a existencial.

**Tipo:** tabela de investigação de domínio.

**Conteúdo exato:**

| Valor admissível \(a\) | \(P(a)\) | Valor lógico |
|---:|---|:---:|
| \(-2\) | \(-2+1>0\) | \(F\) |
| \(-1\) | \(-1+1>0\) | \(F\) |
| \(0\) | \(0+1>0\) | \(V\) |
| \(2\) | \(2+1>0\) | \(V\) |
| \(5\) | \(5+1>0\) | \(V\) |

Abaixo da tabela, apresentar dois campos de leitura.

**UNIVERSAL**

\[
\forall x\,P(x)
\]

**Pergunta de leitura:**

> Todos os casos são verdadeiros?

**Resultado:**

> **Falsa.**

**Exceções à universal:**

\[
-2,\quad-1.
\]

---

**EXISTENCIAL**

\[
\exists x\,P(x)
\]

**Pergunta de leitura:**

> Existe pelo menos um caso verdadeiro?

**Resultado:**

> **Verdadeira.**

**Testemunhos possíveis:**

\[
0,\quad2,\quad5.
\]

**Construção:** utilizar três colunas principais. Todos os valores admissíveis devem aparecer simultaneamente. Abaixo da tabela, os campos “Universal” e “Existencial” devem aparecer lado a lado quando a largura permitir, deixando claro que ambos são leituras da mesma investigação já realizada.

**Ênfase:** destacar estruturalmente a coluna “Valor lógico” e a passagem da leitura linha a linha para as duas conclusões globais. O objetivo é tornar perceptível que, uma vez organizados os casos, não é necessário reconstruir a análise desde o início para cada quantificador.

**Restrições de fidelidade:** não utilizar setas decorativas. Não depender exclusivamente de cor. Não utilizar diagramas de conjuntos. Não introduzir conjunto-verdade. Não acrescentar valores externos aos cinco valores admissíveis. Não utilizar ícones decorativos. Preservar \(V\) e \(F\) na notação já construída. Não incluir regras formais de negação dos quantificadores nem múltiplos quantificadores.

**Implementação preferencial:** HTML/CSS. Não utilizar SVG.

O ganho do procedimento está em organizar primeiro os **casos admissíveis** e só depois fazer a leitura global.

Com o mesmo perfil:

\[
F,\quad F,\quad V,\quad V,\quad V,
\]

podemos perceber imediatamente que a afirmação universal falha porque nem todos os casos são verdadeiros, enquanto a afirmação existencial é satisfeita porque há casos favoráveis.

Assim, uma investigação bem organizada do domínio fornece, ao mesmo tempo, as atribuições verdadeiras e falsas, os possíveis testemunhos da existencial e as exceções à universal.

# Quiz

## Questão 1

Considere as expressões:

**I.**

\[
17^2<300.
\]

**II.**

\[
y-4=9.
\]

**III.**

\[
36=6\cdot6.
\]

Um estudante afirma:

> “A expressão I deve ser uma sentença aberta enquanto eu ainda não souber se ela é verdadeira ou falsa.”

Qual alternativa analisa corretamente as três expressões?

**A)** I e II são sentenças abertas, porque seus valores lógicos precisam ser descobertos.

**B)** Apenas II é uma sentença aberta; I e III são proposições determinadas, independentemente de a verificação ser imediata.

**C)** Apenas III é uma proposição; I e II permanecem abertas até que seus resultados sejam calculados.

**D)** As três são proposições determinadas, pois todas utilizam linguagem matemática.

## Questão 2

Considere:

\[
P(x):\quad x\text{ é múltiplo de }4
\]

e:

\[
p:\quad 12\text{ é múltiplo de }4.
\]

Suponha ainda que \(8\) seja um valor admissível para \(x\).

Qual afirmação é correta?

**A)** \(P(x)\) e \(p\) possuem a mesma função: ambos nomeiam proposições já determinadas.

**B)** \(P(8)\) continua sendo uma sentença aberta porque a letra \(P\) permanece na expressão.

**C)** \(P(x)\) representa uma condição dependente de \(x\), \(P(8)\) representa uma proposição determinada e \(p\) nomeia uma proposição completa.

**D)** \(P(x)\) e \(P(8)\) possuem o mesmo status lógico, pois expressam a mesma propriedade.

## Questão 3

Qual afirmação descreve corretamente o quantificador existencial?

**A)** \(\exists x\,P(x)\) afirma que exatamente um valor admissível satisfaz \(P\).

**B)** \(\exists x\,P(x)\) afirma que a maioria dos valores admissíveis satisfaz \(P\).

**C)** \(\exists x\,P(x)\) exige que pelo menos um valor admissível satisfaça \(P\), podendo haver vários casos favoráveis.

**D)** \(\exists x\,P(x)\) só é verdadeira quando todos os valores admissíveis satisfazem \(P\).

## Questão 4

Considere:

**\(A(x)\):** \(x\) possui a propriedade \(A\).

**\(B(x)\):** \(x\) possui a propriedade \(B\).

Qual par representa corretamente as frases:

**I.** Todo \(A\) é \(B\).

**II.** Existe pelo menos um \(A\) que é \(B\).

**A)**

\[
\forall x\,(A(x)\land B(x))
\]

e:

\[
\exists x\,(A(x)\to B(x)).
\]

**B)**

\[
\forall x\,(A(x)\to B(x))
\]

e:

\[
\exists x\,(A(x)\land B(x)).
\]

**C)**

\[
\exists x\,(A(x)\to B(x))
\]

e:

\[
\forall x\,(A(x)\land B(x)).
\]

**D)**

\[
\forall x\,(A(x)\to B(x))
\]

e:

\[
\exists x\,(A(x)\to B(x)).
\]

## Questão 5

Qual expressão é logicamente equivalente a:

\[
\neg(\exists x\,P(x))?
\]

**A)**

\[
\exists x\,\neg P(x)
\]

**B)**

\[
\forall x\,\neg P(x)
\]

**C)**

\[
\forall x\,P(x)
\]

**D)**

\[
\neg(\forall x\,P(x))
\]

# Exercícios

## Exercício 1 — Aberta, determinada ou apenas não verificada?

Analise as expressões declarativas abaixo.

### I

\[
14+9=23.
\]

### II

\[
t^2=25.
\]

### III

\[
17^2<300.
\]

### IV

\[
(-5)^2=25.
\]

### V

> O número inteiro \(n\) é par.

### a)

Classifique cada expressão como:

- **proposição determinada**;
- **sentença aberta**.

### b)

Identifique todas as expressões cujo valor lógico depende da escolha de um valor para uma variável.

Explique o que permanece indeterminado em sua estrutura.

### c)

Compare as expressões II e IV.

Na expressão IV, um valor específico já ocupa a posição que, em II, pode variar. Explique o que essa diferença provoca no status lógico das duas expressões.

### d)

Considere agora a expressão III.

Um estudante ainda não efetuou o cálculo necessário para decidir se ela é verdadeira ou falsa e afirma:

> “Enquanto eu não fizer a conta, a sentença continua aberta.”

Analise essa afirmação. Sua resposta deve distinguir:

- desconhecer o valor lógico de uma proposição;
- depender de uma atribuição ainda não realizada.

## Exercício 2 — Predicado, atribuição e variável livre

Considere como valores admissíveis para \(x\):

\[
-4,\quad -3,\quad -2,\quad 0,\quad 1,\quad 4
\]

e o predicado:

\[
P(x):\quad x^2<10.
\]

### a)

Escreva em linguagem verbal a condição representada por \(P(x)\).

### b)

Em \(P(x)\), qual elemento ainda pode receber diferentes valores?

Explique por que, nesse estágio, a expressão continua aberta.

### c)

Avalie:

\[
P(-4),\qquad P(-2),\qquad P(1).
\]

Em cada caso:

1. faça a atribuição;
2. escreva a proposição obtida;
3. determine seu valor lógico.

### d)

Escolha, entre os valores admissíveis fornecidos:

- um valor diferente dos utilizados no item **c** que torne \(P(x)\) verdadeira;
- um valor diferente dos utilizados no item **c** que torne \(P(x)\) falsa.

Quando houver mais de uma possibilidade, basta apresentar uma escolha válida para cada caso.

### e)

Considere:

\[
p:\quad (-2)^2<10.
\]

Compare as funções de:

\[
p
\]

e:

\[
P(x).
\]

Explique por que a semelhança das letras utilizadas para nomeá-los não faz com que representem o mesmo tipo de estrutura lógica.

### f)

Após uma atribuição admissível \(a\), a expressão:

\[
P(a)
\]

continua aberta da mesma maneira que \(P(x)\)?

Justifique.

## Exercício 3 — O mesmo predicado em domínios diferentes

Considere o predicado:

\[
P(x):\quad x>1.
\]

Ele será investigado em três contextos diferentes.

### Domínio I

Os valores admissíveis são:

\[
-2,\quad0,\quad2,\quad4.
\]

### Domínio II

Os valores admissíveis são:

\[
0,\quad1,\quad2,\quad3.
\]

### Domínio III

Os valores admissíveis são:

\[
-3,\quad-2,\quad-1,\quad0.
\]

### Visual para HTML

**Função conceitual:** permitir a comparação simultânea do mesmo predicado em diferentes domínios, tornando perceptível que a condição investigada permanece fixa enquanto os valores admissíveis mudam.

**Tipo:** painel comparativo em três blocos paralelos.

**Conteúdo exato:**

Apresentar uma única vez, acima dos três painéis:

\[
P(x):\quad x>1.
\]

Abaixo, organizar:

| Domínio I | Domínio II | Domínio III |
|---|---|---|
| Valores admissíveis: \(-2,\ 0,\ 2,\ 4\) | Valores admissíveis: \(0,\ 1,\ 2,\ 3\) | Valores admissíveis: \(-3,\ -2,\ -1,\ 0\) |
| Valores que satisfazem \(P\): ______ | Valores que satisfazem \(P\): ______ | Valores que satisfazem \(P\): ______ |

**Construção:** o predicado deve aparecer como elemento comum aos três painéis. Os três domínios devem possuir dimensões equivalentes e permanecer visualmente comparáveis. A linha destinada às respostas deve possuir espaço para preenchimento manual.

**Ênfase:** destacar estruturalmente a permanência de \(P(x)\) e a mudança dos valores admissíveis. Essa relação deve ser comunicada pela organização espacial e pela repetição controlada dos painéis, não por setas.

**Restrições de fidelidade:** não marcar previamente quais valores satisfazem \(P\). Não depender exclusivamente de cor. Não utilizar diagramas de conjuntos. Não introduzir conjunto-verdade. Não acrescentar valores que não aparecem no enunciado. Não utilizar ilustrações decorativas.

**Implementação preferencial:** HTML/CSS. Não utilizar SVG.

### a)

Para cada domínio, identifique quais valores admissíveis satisfazem \(P(x)\).

### b)

Considere o valor:

\[
4.
\]

Ele satisfaz a condição \(x>1\).

Em quais dos três domínios esse valor pode ser utilizado como uma atribuição admissível na investigação apresentada?

Explique por que satisfazer o predicado, por si só, não basta para que um valor participe de determinado contexto.

### c)

Faça a mesma análise para o valor:

\[
3.
\]

### d)

Compare os Domínios I e III.

Há algum valor admissível que satisfaça \(P(x)\) em cada um deles?

Registre o resultado sem alterar a condição \(P(x)\).

### e)

Depois das três investigações, responda:

- o que mudou de um domínio para outro?
- o que permaneceu igual?

Justifique utilizando os casos analisados, e não apenas os nomes “predicado” e “domínio”.

## Exercício 4 — Uma investigação, duas leituras

Considere:

\[
Q(x):\quad x<8
\]

e, como valores admissíveis:

\[
-3,\quad0,\quad2,\quad5,\quad7.
\]

Organize a investigação desses casos na tabela:

| Valor admissível \(a\) | \(Q(a)\) | Valor lógico |
|---:|---|:---:|
| \(-3\) |  |  |
| \(0\) |  |  |
| \(2\) |  |  |
| \(5\) |  |  |
| \(7\) |  |  |

### a)

Complete a tabela.

### b)

A partir do perfil obtido, determine o valor lógico de:

\[
\forall x\,Q(x).
\]

Justifique a decisão usando os casos do domínio.

### c)

Determine também o valor lógico de:

\[
\exists x\,Q(x).
\]

### d)

Se a afirmação existencial for verdadeira, apresente um valor admissível que possa funcionar como testemunho.

Se houver mais de uma possibilidade, basta escolher uma.

### e)

Existe algum valor admissível que funcione como exceção à exigência universal?

Justifique sua resposta a partir da tabela.

### f)

Compare o papel desempenhado pela mesma tabela nos itens **b** e **c**.

Que pergunta diferente fazemos ao perfil dos casos quando analisamos a universal e quando analisamos a existencial?

## Exercício 5 — Do valor global aos casos

Em todos os quatro cenários abaixo, considere que o domínio possui **pelo menos dois valores admissíveis** e que \(P(x)\) é um predicado já determinado.

Considere as seguintes afirmações sobre os casos:

**I.** Todo valor admissível satisfaz \(P\).

**II.** Existe pelo menos um valor admissível que satisfaz \(P\).

**III.** Existe pelo menos um valor admissível que não satisfaz \(P\).

**IV.** Nenhum valor admissível satisfaz \(P\).

Para cada cenário, analise as afirmações I–IV e classifique cada uma como:

- **obrigatoriamente verdadeira**;
- **possível, mas não obrigatória**;
- **impossível**.

### Cenário A

Sabe-se que:

\[
\forall x\,P(x)=V.
\]

### Cenário B

Sabe-se que:

\[
\forall x\,P(x)=F.
\]

### Cenário C

Sabe-se que:

\[
\exists x\,P(x)=V.
\]

### Cenário D

Sabe-se que:

\[
\exists x\,P(x)=F.
\]

### a)

Faça as classificações para os quatro cenários.

### b)

No Cenário B, é possível determinar exatamente **quantos** valores admissíveis deixam de satisfazer \(P\)?

Explique o que a informação fornecida obriga e o que ela deixa em aberto.

### c)

No Cenário C, é possível concluir que todos os valores admissíveis satisfazem \(P\)?

Se sua resposta for negativa, descreva dois perfis diferentes de valores \(V/F\) compatíveis com a informação dada.

### d)

Compare os Cenários A e C.

Explique por que a verdade de uma proposição universal fornece uma informação mais restritiva sobre os casos do que a simples verdade de uma proposição existencial.

## Exercício 6 — Traduzindo a quantificação

Considere o predicado:

\[
P(x):\quad x>2.
\]

O domínio já está fixado, e \(x\) representa sempre um valor admissível desse domínio.

### a)

Represente simbolicamente:

> Todo valor admissível é maior que 2.

### b)

Represente simbolicamente:

> Existe pelo menos um valor admissível maior que 2.

### c)

Traduza para linguagem verbal:

\[
\forall x\,P(x).
\]

Escreva uma frase que preserve exatamente a força do quantificador utilizado.

### d)

Traduza:

\[
\exists x\,P(x).
\]

Sua frase não deve sugerir que existe exatamente um caso favorável.

### e)

Considere agora:

\[
R(x):\quad x+4=10.
\]

Escreva em linguagem verbal:

\[
\exists x\,R(x).
\]

Depois identifique separadamente:

- a informação fornecida pelo quantificador;
- a condição interna expressa por \(R(x)\).

### f)

Compare:

\[
P(5)
\]

e:

\[
\exists x\,P(x).
\]

Ambas podem produzir proposições determinadas, mas fazem afirmações do mesmo tipo sobre o domínio?

Explique a diferença entre fixar um caso particular e quantificar sobre os valores admissíveis.

## Exercício 7 — “Todo \(A\) é \(B\)” e “Existe um \(A\) que é \(B\)”

Considere como valores admissíveis os números:

\[
1,\quad2,\quad3,\quad4,\quad5,\quad6,\quad7.
\]

Defina:

\[
A(x):\quad x\text{ é par}
\]

e:

\[
B(x):\quad x<7.
\]

Queremos representar corretamente duas afirmações.

### Afirmação I

> Todo número admissível que é par é menor que 7.

### Afirmação II

> Existe pelo menos um número admissível que é par e menor que 7.

### a)

Represente simbolicamente a Afirmação I utilizando:

\[
A(x),\qquad B(x),\qquad\forall,\qquad\to.
\]

### b)

Um estudante propõe para a Afirmação I:

\[
\forall x\,(A(x)\land B(x)).
\]

Compare essa fórmula com a frase original.

Examine especialmente o que ela afirma sobre os valores admissíveis que **não** satisfazem \(A(x)\).

Explique por que as duas estruturas não dizem a mesma coisa.

### c)

Represente simbolicamente a Afirmação II utilizando:

\[
A(x),\qquad B(x),\qquad\exists,\qquad\land.
\]

### d)

Outro estudante propõe:

\[
\exists x\,(A(x)\to B(x))
\]

para representar a Afirmação II.

Considere um valor admissível \(a\) para o qual:

\[
A(a)=F
\]

e:

\[
B(a)=F.
\]

Avalie, nesse mesmo caso:

\[
A(a)\to B(a)
\]

e:

\[
A(a)\land B(a).
\]

Depois explique por que uma condicional verdadeira nesse tipo de caso não fornece necessariamente o objeto exigido pela frase:

> Existe pelo menos um \(A\) que é \(B\).

### e)

Nas fórmulas corretas dos itens **a** e **c**, identifique:

- o quantificador;
- a expressão que aparece entre parênteses;
- o conectivo utilizado dentro dessa expressão.

### f)

Compare as funções de:

\[
\forall x\,(A(x)\to B(x))
\]

e:

\[
\exists x\,(A(x)\land B(x)).
\]

Explique por que a primeira organiza uma exigência sobre todos os valores admissíveis, enquanto a segunda procura um mesmo valor que reúna simultaneamente as duas propriedades.

## Exercício 8 — O que está sob o alcance do quantificador?

Considere as três expressões:

### I

\[
\forall x\,(P(x)\to Q(x)).
\]

### II

\[
\exists x\,(P(x)\land Q(x)).
\]

### III

\[
P(x)\to Q(x).
\]

### a)

Nas expressões I e II, identifique:

- o quantificador;
- a expressão completa que aparece sob seu alcance;
- o conectivo que organiza a estrutura interna.

### b)

Compare o papel de \(x\) nas expressões I e III.

Em qual delas \(x\) permanece livre para receber diferentes valores? Em qual delas seu papel já é determinado pelo quantificador?

Explique a diferença sem alterar as condições \(P(x)\) e \(Q(x)\).

### c)

Faça a mesma comparação entre II e:

\[
P(x)\land Q(x).
\]

O que muda quando acrescentamos o quantificador existencial à estrutura?

### d)

Observe os parênteses em:

\[
\forall x\,(P(x)\to Q(x))
\]

e:

\[
\exists x\,(P(x)\land Q(x)).
\]

Explique o que eles ajudam a tornar visível em relação ao alcance do quantificador.

### e)

Construa simbolicamente a afirmação:

> Existe pelo menos um valor admissível para o qual \(P(x)\) e \(Q(x)\) são simultaneamente verdadeiras.

Utilize apenas:

\[
P(x),\qquad Q(x),\qquad\exists,\qquad\land.
\]

### f)

Agora considere as seguintes informações separadas:

- a afirmação deve tratar **todos** os valores admissíveis;
- para cada valor considerado, queremos exigir que, se \(P(x)\) for satisfeita, \(Q(x)\) também seja;
- a relação interna deve ser condicional.

Construa a fórmula correspondente e indique qual parte está sob o alcance do quantificador.

## Exercício 9 — Quando uma exceção rompe a universal

Considere como valores admissíveis para \(x\):

\[
0,\quad1,\quad2,\quad4
\]

e o predicado:

\[
P(x):\quad 2x<7.
\]

### a)

Avalie:

\[
P(0),\qquad P(1),\qquad P(2),\qquad P(4).
\]

Registre o valor lógico de cada proposição obtida.

### b)

Com base nesses casos, determine o valor lógico de:

\[
\forall x\,P(x).
\]

Justifique utilizando os valores admissíveis.

### c)

Escreva em linguagem verbal a **negação** da afirmação:

\[
\forall x\,P(x).
\]

Sua frase deve preservar o mesmo domínio.

### d)

Represente simbolicamente a negação construída no item anterior.

Depois registre a equivalência entre a afirmação universal negada e a forma que você encontrou.

### e)

Entre os valores admissíveis, identifique qual deles pode funcionar como testemunho da proposição existencial presente na negação.

Verifique explicitamente que, para esse valor,

\[
\neg P(x)
\]

é verdadeira.

### f)

Explique por que um único valor com essa característica já é suficiente para que a afirmação universal do item **b** seja falsa, mesmo que os demais casos satisfaçam \(P(x)\).

### g)

Compare as duas funções desempenhadas pelo mesmo valor encontrado:

- como exceção à afirmação universal;
- como testemunho da afirmação existencial que expressa sua negação.

Explique por que essas duas descrições são compatíveis.

## Exercício 10 — Um caso desfavorável elimina uma existência?

Considere como valores admissíveis:

\[
1,\quad2,\quad3,\quad4
\]

e o predicado:

\[
P(x):\quad x\text{ é múltiplo de }3.
\]

Um estudante afirma:

> “Como o número \(2\) não é múltiplo de 3, encontrei um caso em que \(P(x)\) é falsa. Portanto, é falso que exista algum valor admissível que satisfaça \(P\).”

### a)

Avalie \(P(x)\) para os quatro valores admissíveis.

### b)

Determine o valor lógico de:

\[
\exists x\,P(x).
\]

Indique quais casos do domínio são suficientes para sustentar sua decisão.

### c)

Analise o raciocínio do estudante.

Em que ponto a existência de um caso desfavorável foi utilizada de maneira incorreta?

### d)

Explique verbalmente o que precisaria ocorrer com **todos os valores admissíveis** para que:

\[
\exists x\,P(x)
\]

fosse falsa.

### e)

Escreva simbolicamente a negação de:

\[
\exists x\,P(x).
\]

Depois registre a equivalência correspondente.

### f)

Considere agora:

\[
\exists x\,\neg P(x).
\]

Determine seu valor lógico no domínio apresentado.

### g)

Compare:

\[
\exists x\,\neg P(x)
\]

e:

\[
\neg(\exists x\,P(x)).
\]

Explique por que a primeira expressão pode ser verdadeira ao mesmo tempo que a segunda é falsa.

## Exercício 11 — Trocar só uma parte não basta

### Parte I

Considere a afirmação:

\[
\forall x\,P(x).
\]

Três estudantes propuseram as seguintes fórmulas para representar sua negação.

### Proposta I

\[
\exists x\,P(x)
\]

### Proposta II

\[
\forall x\,\neg P(x)
\]

### Proposta III

\[
\exists x\,\neg P(x)
\]

### a)

Identifique qual proposta representa corretamente a negação de:

\[
\forall x\,P(x).
\]

### b)

Nas duas propostas incorretas, determine o que foi alterado e o que permaneceu indevidamente inalterado em relação à proposição original.

### c)

Traduza cada uma das três propostas para linguagem verbal.

Sua tradução deve tornar perceptível que as fórmulas incorretas ainda possuem significados matemáticos próprios, embora não sejam a negação procurada.

---

### Parte II

Considere agora:

\[
\exists x\,Q(x).
\]

Outras três propostas foram apresentadas.

### Proposta I

\[
\exists x\,\neg Q(x)
\]

### Proposta II

\[
\forall x\,\neg Q(x)
\]

### Proposta III

\[
\forall x\,Q(x)
\]

### d)

Identifique qual proposta representa corretamente a negação da afirmação existencial.

### e)

Para cada proposta incorreta, explique se ocorreu:

- alteração apenas do quantificador;
- alteração apenas da condição interna;
- ou outra transformação inadequada.

### f)

Traduza as três fórmulas para linguagem verbal e compare aquilo que cada uma realmente afirma sobre os valores admissíveis.

### g)

Complete, com suas próprias palavras, a ideia abaixo:

> Para negar uma afirmação quantificada deste tipo, não basta alterar apenas __________. É necessário observar conjuntamente __________ e __________.

Não é necessário reproduzir uma frase específica; sua resposta deve preservar a relação lógica envolvida.

## Exercício 12 — A negação permanece no mesmo domínio

Considere como valores admissíveis para \(x\):

\[
2,\quad4,\quad6,\quad8
\]

e o predicado:

\[
P(x):\quad x<10.
\]

Queremos avaliar:

\[
\forall x\,P(x).
\]

Dois estudantes iniciaram a análise de maneiras diferentes.

### Ana

> “Vou examinar somente \(2\), \(4\), \(6\) e \(8\), pois são os valores admissíveis informados pelo problema.”

### Bruno

> “O número \(12\) não satisfaz \(x<10\). Portanto, encontrei uma exceção e a afirmação universal é falsa.”

### a)

Avalie \(P(x)\) para todos os valores admissíveis e determine o valor lógico de:

\[
\forall x\,P(x).
\]

### b)

Existe alguma exceção à exigência universal entre os valores:

\[
2,\quad4,\quad6,\quad8?
\]

Justifique.

### c)

Analise o procedimento de Ana.

Por que a restrição aos quatro valores indicados é importante para interpretar corretamente a proposição?

### d)

Analise a conclusão de Bruno.

O cálculo envolvendo \(12\) está matematicamente correto, mas pode ser utilizado para decidir a proposição considerada?

Explique.

### e)

Escreva verbalmente a negação de:

\[
\forall x\,P(x)
\]

de modo que fique explícito que ela continua tratando dos mesmos valores admissíveis.

### f)

O que precisaria existir **entre \(2\), \(4\), \(6\) e \(8\)** para que essa negação fosse verdadeira?

### g)

Explique por que mudar o domínio durante a procura por uma exceção significa passar a investigar outra situação, e não negar corretamente a proposição original.

## Exercício 13 — O verdadeiro contraexemplo de “Todo \(A\) é \(B\)”

Considere como valores admissíveis:

\[
2,\quad3,\quad5,\quad6.
\]

Defina:

\[
A(x):\quad x\text{ é múltiplo de }3
\]

e:

\[
B(x):\quad x>4.
\]

Considere a afirmação:

> Todo número admissível que é múltiplo de 3 é maior que 4.

Sua forma simbólica é:

\[
\forall x\,(A(x)\to B(x)).
\]

### Visual para HTML

**Função conceitual:** permitir investigar, caso a caso, qual combinação entre \(A(a)\) e \(B(a)\) realmente satisfaz a condição necessária para refutar a afirmação universal.

**Tipo:** tabela estrutural de candidatos a contraexemplo.

**Conteúdo exato:**

| Valor admissível \(a\) | \(A(a)\) | \(B(a)\) | \(A(a)\to B(a)\) | \(A(a)\land\neg B(a)\) |
|---:|:---:|:---:|:---:|:---:|
| \(2\) |  |  |  |  |
| \(3\) |  |  |  |  |
| \(5\) |  |  |  |  |
| \(6\) |  |  |  |  |

**Construção:** utilizar cinco colunas. As colunas \(A(a)\) e \(B(a)\) devem aparecer lado a lado. A coluna \(A(a)\to B(a)\) deve permitir verificar a condição interna da afirmação universal. A coluna \(A(a)\land\neg B(a)\) deve aparecer por último, favorecendo a comparação entre a falha do condicional e a estrutura exigida pela negação. Todas as células derivadas devem permanecer vazias.

**Ênfase:** tornar perceptível a relação entre:

\[
A(a)\to B(a)
\]

e:

\[
A(a)\land\neg B(a).
\]

O visual deve favorecer a identificação do caso que realiza exatamente a falha necessária, sem destacá-lo antecipadamente.

**Restrições de fidelidade:** não preencher respostas. Não destacar previamente qualquer valor. Não utilizar setas decorativas. Não depender exclusivamente de cor. Não utilizar diagramas de conjuntos. Não introduzir símbolos novos. Não acrescentar valores nem alterar sua ordem sem necessidade.

**Implementação preferencial:** HTML/CSS. Não utilizar SVG.

### a)

Complete a tabela.

### b)

Determine o valor lógico de:

\[
\forall x\,(A(x)\to B(x)).
\]

Justifique utilizando as avaliações obtidas.

### c)

Identifique o valor admissível que constitui um contraexemplo à afirmação universal.

### d)

Para o valor escolhido no item **c**, verifique explicitamente:

\[
A(a)
\]

e:

\[
B(a).
\]

Que combinação de valores lógicos aparece?

### e)

Há um valor admissível no qual \(B(a)\) é falsa, mas que **não** constitui contraexemplo.

Identifique-o e explique por que a falsidade de \(B(a)\), isoladamente, não basta.

### f)

Comece pela negação da proposição completa:

\[
\neg\left(\forall x\,(A(x)\to B(x))\right).
\]

Reescreva-a em duas etapas.

Na primeira, utilize a negação da afirmação universal para obter uma proposição existencial cuja condição interna ainda contenha:

\[
\neg(A(x)\to B(x)).
\]

Na segunda, utilize a forma já conhecida da negação de um condicional.

Complete:

\[
\neg\left(\forall x\,(A(x)\to B(x))\right)
\equiv
\underline{\hspace{5cm}}
\equiv
\underline{\hspace{5cm}}.
\]

### g)

Traduza verbalmente a **forma final** obtida no item anterior.

Sua frase deve explicitar que o mesmo valor admissível precisa:

- satisfazer \(A\);
- deixar de satisfazer \(B\).

### h)

Compare o valor identificado no item **c** com a forma existencial obtida no item **f**.

Explique por que ele pode ser descrito simultaneamente como:

- contraexemplo à afirmação universal;
- testemunho de sua negação.

---

Considere agora outra situação.

Os valores admissíveis são:

\[
1,\quad2,\quad3,\quad4,\quad5,\quad6,\quad7,\quad8.
\]

Defina:

\[
C(x):\quad x\text{ é par}
\]

e:

\[
D(x):\quad x\text{ é múltiplo de }4.
\]

Considere:

\[
\forall x\,(C(x)\to D(x)).
\]

### i)

Encontre **um** contraexemplo para essa afirmação.

Não é necessário encontrar todos.

### j)

Para o valor escolhido, verifique explicitamente:

\[
C(a)=V
\]

e:

\[
D(a)=F.
\]

Explique por que essas duas condições, satisfeitas pelo mesmo valor, são suficientes para que sua escolha seja válida.

## Exercício 14 — Diagnóstico e integração

Considere como valores admissíveis:

\[
-2,\quad-1,\quad0,\quad1,\quad2.
\]

Defina:

\[
P(x):\quad x^2\leq1
\]

e:

\[
Q(x):\quad x>0.
\]

### a)

Complete a tabela:

| \(a\) | \(P(a)\) | \(Q(a)\) |
|---:|:---:|:---:|
| \(-2\) |  |  |
| \(-1\) |  |  |
| \(0\) |  |  |
| \(1\) |  |  |
| \(2\) |  |  |

### b)

Utilizando os mesmos dados, investigue as quatro proposições:

**I.**

\[
\exists x\,P(x)
\]

**II.**

\[
\forall x\,P(x)
\]

**III.**

\[
\exists x\,Q(x)
\]

**IV.**

\[
\forall x\,(P(x)\to Q(x)).
\]

Para cada uma:

- determine seu valor lógico;
- indique quais casos do domínio sustentam sua decisão;
- escolha autonomamente se é mais útil procurar casos favoráveis, exceções ou outra informação pertinente à estrutura.

### c)

Escreva simbolicamente a negação de:

\[
\exists x\,Q(x).
\]

Depois traduza a negação para linguagem verbal e determine seu valor lógico no mesmo domínio.

### d)

Examine:

\[
\forall x\,(P(x)\to Q(x)).
\]

Se ela for falsa, apresente **um** contraexemplo.

Verifique, para o mesmo valor escolhido:

\[
P(a)=V
\]

e:

\[
Q(a)=F.
\]

Se houver mais de uma resposta válida, basta apresentar uma delas.

### e)

Explique por que o valor encontrado no item anterior é suficiente para decidir a afirmação universal, mesmo sem utilizar todos os casos como contraexemplos.

---

Quatro estudantes analisaram partes da situação.

### Ana

> “Como \(P(1)\) é verdadeira, então \(\forall x\,P(x)\) é verdadeira.”

### Bruno

> “Como \(Q(-2)\) é falsa, então \(\exists x\,Q(x)\) é falsa.”

### Carla

> “Como \(Q(1)\) é verdadeira e \(1\) é um valor admissível, esse valor pode funcionar como testemunho de \(\exists x\,Q(x)\).”

### Diego

> “Para verificar se \(\forall x(P(x)\to Q(x))\) falha, procurei um valor admissível para o qual \(P(a)\) fosse verdadeira e \(Q(a)\) fosse falsa. O valor \(-1\) possui essas duas características.”

### f)

Analise separadamente as quatro falas.

Para cada estudante:

1. determine se a conclusão é sustentada;
2. indique quais valores do domínio são relevantes;
3. quando houver erro, localize precisamente a falha do raciocínio;
4. reescreva a conclusão de forma correta quando necessário.

Não responda apenas “certo” ou “errado”.

### g)

Compare os erros presentes nas falas de Ana e Bruno.

Embora ambos utilizem apenas um caso, por que um único caso favorável não estabelece uma universal e um único caso desfavorável não elimina uma existencial?

### h)

Compare as falas de Carla e Diego.

Que papel o valor concreto exerce em cada uma delas?

Sua resposta deve distinguir a função de um testemunho de uma afirmação existencial da função de um contraexemplo a uma afirmação universal.

### i)

Escolha uma das proposições quantificadas **falsas** investigadas no item **b**.

Explique:

- qual estrutura lógica ela possui;
- qual valor admissível você utiliza para revelar sua falsidade;
- que condição esse valor satisfaz ou deixa de satisfazer;
- por que esse único caso é suficiente para a conclusão.

# Gabarito Comentado

## Quiz

### Questão 1

**Alternativa correta: B.**

A expressão

\[
17^2<300
\]

já é uma proposição determinada: não depende da escolha posterior de nenhum valor. O fato de ainda não termos efetuado o cálculo não a torna aberta.

Já

\[
y-4=9
\]

depende do valor atribuído a \(y\).

### Questão 2

**Alternativa correta: C.**

\[
P(x)
\]

representa uma condição dependente de \(x\);

\[
P(8)
\]

representa uma proposição determinada;

e \(p\) nomeia uma proposição completa.

### Questão 3

**Alternativa correta: C.**

O quantificador

\[
\exists
\]

exige a existência de **pelo menos um** caso favorável. Pode haver um, vários ou mesmo todos os valores satisfazendo a condição.

### Questão 4

**Alternativa correta: B.**

As formas corretas são:

\[
\forall x\,(A(x)\to B(x))
\]

para “Todo \(A\) é \(B\)” e:

\[
\exists x\,(A(x)\land B(x))
\]

para “Existe pelo menos um \(A\) que é \(B\)”.

### Questão 5

**Alternativa correta: B.**

\[
\neg(\exists x\,P(x))
\equiv
\forall x\,\neg P(x).
\]

## Exercício 1

### a)

**I.**

\[
14+9=23
\]

é uma **proposição determinada** e verdadeira.

**II.**

\[
t^2=25
\]

é uma **sentença aberta**, pois diferentes valores atribuídos a \(t\) podem produzir proposições verdadeiras ou falsas.

**III.**

\[
17^2<300
\]

é uma **proposição determinada**. De fato,

\[
17^2=289
\]

e:

\[
289<300,
\]

portanto ela é verdadeira.

**IV.**

\[
(-5)^2=25
\]

é uma **proposição determinada** e verdadeira.

**V.**

> O número inteiro \(n\) é par.

é uma **sentença aberta**, pois seu valor lógico depende do valor atribuído a \(n\).

### b)

As expressões cujo valor lógico depende de uma atribuição são:

\[
\boxed{\text{II e V}}.
\]

Em II, ainda é necessário determinar qual valor ocupa \(t\). Em V, é necessário determinar qual número inteiro ocupa \(n\).

### c)

Em:

\[
t^2=25,
\]

\(t\) ainda pode assumir diferentes valores. Por isso, a sentença permanece aberta.

Em:

\[
(-5)^2=25,
\]

o valor já foi determinado. Existe uma afirmação específica a avaliar, portanto temos uma proposição.

### d)

A afirmação do estudante está incorreta.

Não ter calculado ainda \(17^2\) significa apenas que o estudante talvez ainda **não saiba** o valor lógico da proposição.

Isso é diferente de uma sentença aberta, na qual o próprio valor lógico depende de uma atribuição ainda não fixada.

## Exercício 2

### a)

\[
P(x):\quad x^2<10
\]

pode ser lido como:

> O quadrado de \(x\) é menor que 10.

### b)

A variável \(x\) ainda pode receber diferentes valores admissíveis. Por isso, \(P(x)\) permanece uma condição aberta.

### c)

Para \(x=-4\):

\[
P(-4):\quad (-4)^2<10,
\]

isto é,

\[
16<10.
\]

Logo,

\[
P(-4)=F.
\]

Para \(x=-2\):

\[
P(-2):\quad (-2)^2<10,
\]

isto é,

\[
4<10.
\]

Logo,

\[
P(-2)=V.
\]

Para \(x=1\):

\[
P(1):\quad1^2<10,
\]

isto é,

\[
1<10.
\]

Logo,

\[
P(1)=V.
\]

### d)

Uma resposta possível para uma atribuição verdadeira é:

\[
x=-3,
\]

pois:

\[
(-3)^2=9<10.
\]

Também seria válida a escolha \(x=0\).

Para uma atribuição falsa, podemos escolher:

\[
x=4,
\]

pois:

\[
4^2=16>10.
\]

### e)

Em:

\[
p:\quad(-2)^2<10,
\]

\(p\) nomeia uma proposição completa e determinada.

Já:

\[
P(x):\quad x^2<10
\]

representa uma condição cujo resultado ainda depende do valor atribuído a \(x\).

### f)

Não. Depois que uma atribuição admissível \(a\) é fixada, \(P(a)\) representa uma proposição determinada.

## Exercício 3

### a)

Para:

\[
P(x):\quad x>1,
\]

temos:

**Domínio I**

\[
-2,\quad0,\quad2,\quad4.
\]

Satisfazem \(P\):

\[
\boxed{2,\;4}.
\]

**Domínio II**

\[
0,\quad1,\quad2,\quad3.
\]

Satisfazem \(P\):

\[
\boxed{2,\;3}.
\]

**Domínio III**

\[
-3,\quad-2,\quad-1,\quad0.
\]

Nenhum dos valores satisfaz \(P\).

### b)

O valor \(4\) é admissível apenas no **Domínio I**.

Embora \(4>1\) seja verdadeiro, isso não permite utilizar \(4\) em qualquer investigação. Para participar de determinado contexto, o valor também precisa ser admissível naquele domínio.

### c)

O valor \(3\) é admissível apenas no **Domínio II**.

Ele satisfaz \(P(x)\), pois:

\[
3>1,
\]

mas não pertence aos casos considerados nos outros dois domínios.

### d)

No Domínio I, existem casos que satisfazem \(P\):

\[
2,\quad4.
\]

No Domínio III, nenhum valor admissível satisfaz \(P\).

### e)

O que mudou foram os **valores admissíveis**.

O que permaneceu igual foi a condição:

\[
P(x):\quad x>1.
\]

Assim, a propriedade investigada não mudou; mudaram os objetos aos quais ela pôde ser aplicada.

## Exercício 4

### a)

| Valor admissível \(a\) | \(Q(a)\) | Valor lógico |
|---:|---|:---:|
| \(-3\) | \(-3<8\) | \(V\) |
| \(0\) | \(0<8\) | \(V\) |
| \(2\) | \(2<8\) | \(V\) |
| \(5\) | \(5<8\) | \(V\) |
| \(7\) | \(7<8\) | \(V\) |

### b)

Todos os valores admissíveis satisfazem \(Q(x)\). Portanto,

\[
\boxed{\forall x\,Q(x)=V}.
\]

### c)

Como existem valores admissíveis que satisfazem \(Q(x)\),

\[
\boxed{\exists x\,Q(x)=V}.
\]

### d)

Qualquer valor do domínio pode funcionar como testemunho.

Por exemplo:

\[
a=2.
\]

Como:

\[
Q(2)=V,
\]

\(2\) testemunha a afirmação existencial.

### e)

Não existe exceção à universal nesse domínio, pois todos os cinco casos produzem \(V\).

### f)

Na leitura universal, perguntamos se **todos** os casos do perfil são verdadeiros.

Na leitura existencial, perguntamos se há **pelo menos um** caso verdadeiro.

A mesma investigação dos casos permite responder às duas perguntas.

## Exercício 5

### Cenário A

Se:

\[
\forall x\,P(x)=V,
\]

então:

| Afirmação | Classificação |
|---|---|
| I. Todos satisfazem \(P\) | obrigatoriamente verdadeira |
| II. Existe pelo menos um que satisfaz \(P\) | obrigatoriamente verdadeira |
| III. Existe pelo menos um que não satisfaz \(P\) | impossível |
| IV. Nenhum satisfaz \(P\) | impossível |

Todos os valores admissíveis são favoráveis.

### Cenário B

Se:

\[
\forall x\,P(x)=F,
\]

temos:

| Afirmação | Classificação |
|---|---|
| I. Todos satisfazem \(P\) | impossível |
| II. Existe pelo menos um que satisfaz \(P\) | possível, mas não obrigatória |
| III. Existe pelo menos um que não satisfaz \(P\) | obrigatoriamente verdadeira |
| IV. Nenhum satisfaz \(P\) | possível, mas não obrigatória |

A falsidade da universal garante uma falha, mas não informa se existem também casos favoráveis.

### Cenário C

Se:

\[
\exists x\,P(x)=V,
\]

temos:

| Afirmação | Classificação |
|---|---|
| I. Todos satisfazem \(P\) | possível, mas não obrigatória |
| II. Existe pelo menos um que satisfaz \(P\) | obrigatoriamente verdadeira |
| III. Existe pelo menos um que não satisfaz \(P\) | possível, mas não obrigatória |
| IV. Nenhum satisfaz \(P\) | impossível |

A existencial verdadeira garante ao menos um caso favorável, mas os demais podem ser favoráveis ou desfavoráveis.

### Cenário D

Se:

\[
\exists x\,P(x)=F,
\]

temos:

| Afirmação | Classificação |
|---|---|
| I. Todos satisfazem \(P\) | impossível |
| II. Existe pelo menos um que satisfaz \(P\) | impossível |
| III. Existe pelo menos um que não satisfaz \(P\) | obrigatoriamente verdadeira |
| IV. Nenhum satisfaz \(P\) | obrigatoriamente verdadeira |

Nenhum valor admissível satisfaz \(P\).

### b)

No Cenário B, não é possível saber exatamente quantos valores não satisfazem \(P\).

A única exigência é que exista **pelo menos um** caso desfavorável.

### c)

Não.

Considerando, por exemplo, dois valores admissíveis, ambos os perfis abaixo seriam compatíveis com:

\[
\exists x\,P(x)=V:
\]

\[
V,\quad V
\]

e:

\[
V,\quad F.
\]

Outros perfis também são possíveis.

### d)

Em:

\[
\forall x\,P(x)=V,
\]

todos os casos ficam determinados como favoráveis.

Em:

\[
\exists x\,P(x)=V,
\]

sabemos apenas que pelo menos um caso é favorável. Os demais permanecem indeterminados por essa informação.

## Exercício 6

### a)

\[
\boxed{\forall x\,P(x)}
\]

### b)

\[
\boxed{\exists x\,P(x)}
\]

### c)

Uma tradução adequada é:

> Todo valor admissível é maior que 2.

### d)

Uma tradução adequada é:

> Existe pelo menos um valor admissível maior que 2.

Outras redações são aceitáveis desde que não transformem “pelo menos um” em “exatamente um”.

### e)

Para:

\[
R(x):\quad x+4=10,
\]

a expressão:

\[
\exists x\,R(x)
\]

pode ser lida como:

> Existe pelo menos um valor admissível \(x\) para o qual \(x+4=10\).

O quantificador:

\[
\exists
\]

estabelece a exigência de que exista ao menos um caso favorável.

A condição interna é:

\[
x+4=10.
\]

### f)

\[
P(5)
\]

afirma algo sobre o caso específico \(x=5\).

Já:

\[
\exists x\,P(x)
\]

não fixa previamente um caso: afirma que existe algum valor admissível que satisfaz \(P\).

Portanto, embora ambas sejam proposições determinadas, não fazem afirmações do mesmo tipo.

## Exercício 7

Considere os valores admissíveis:

\[
1,\quad2,\quad3,\quad4,\quad5,\quad6,\quad7.
\]

### a)

A Afirmação I é representada por:

\[
\boxed{\forall x\,(A(x)\to B(x))}.
\]

### b)

A fórmula:

\[
\forall x\,(A(x)\land B(x))
\]

é mais forte e representa outra afirmação.

Ela exige que **todo** valor admissível satisfaça simultaneamente \(A(x)\) e \(B(x)\). Isso exigiria, por exemplo, que números ímpares também fossem pares.

A frase original exige \(B(x)\) apenas nos casos em que \(A(x)\) é verdadeira.

No domínio considerado, os valores pares são:

\[
2,\quad4,\quad6,
\]

e todos são menores que \(7\).

### c)

A Afirmação II é representada por:

\[
\boxed{\exists x\,(A(x)\land B(x))}.
\]

### d)

Podemos utilizar:

\[
a=7.
\]

Temos:

\[
A(7)=F
\]

e:

\[
B(7)=F.
\]

Assim,

\[
A(7)\to B(7)=V,
\]

pois o antecedente é falso.

Por outro lado,

\[
A(7)\land B(7)=F.
\]

Isso mostra que um valor pode tornar o condicional verdadeiro sem ser simultaneamente \(A\) e \(B\). Por isso,

\[
\exists x\,(A(x)\to B(x))
\]

não representa corretamente:

> Existe pelo menos um \(A\) que é \(B\).

### e)

Em:

\[
\forall x\,(A(x)\to B(x)),
\]

o quantificador é:

\[
\forall,
\]

a estrutura interna é:

\[
A(x)\to B(x),
\]

e o conectivo interno é:

\[
\to.
\]

Em:

\[
\exists x\,(A(x)\land B(x)),
\]

o quantificador é:

\[
\exists,
\]

a estrutura interna é:

\[
A(x)\land B(x),
\]

e o conectivo interno é:

\[
\land.
\]

### f)

\[
\forall x\,(A(x)\to B(x))
\]

estabelece uma exigência condicional para todos os valores admissíveis: sempre que \(A(x)\) ocorrer, \(B(x)\) também deve ocorrer.

Já:

\[
\exists x\,(A(x)\land B(x))
\]

procura pelo menos um mesmo valor que satisfaça simultaneamente as duas propriedades.

## Exercício 8

### a)

Na expressão:

\[
\forall x\,(P(x)\to Q(x)),
\]

o quantificador é:

\[
\forall.
\]

A expressão sob seu alcance é:

\[
P(x)\to Q(x),
\]

organizada pelo conectivo:

\[
\to.
\]

Na expressão:

\[
\exists x\,(P(x)\land Q(x)),
\]

o quantificador é:

\[
\exists.
\]

A expressão sob seu alcance é:

\[
P(x)\land Q(x),
\]

organizada pelo conectivo:

\[
\land.
\]

### b)

Em:

\[
P(x)\to Q(x),
\]

\(x\) permanece livre.

Em:

\[
\forall x\,(P(x)\to Q(x)),
\]

\(x\) está quantificada. A expressão passa a afirmar que a relação condicional deve valer para todos os valores admissíveis.

### c)

A mesma diferença ocorre entre:

\[
P(x)\land Q(x)
\]

e:

\[
\exists x\,(P(x)\land Q(x)).
\]

Na primeira estrutura, \(x\) permanece livre.

Na segunda, o quantificador estabelece que existe pelo menos um valor admissível que satisfaz simultaneamente \(P\) e \(Q\).

### d)

Os parênteses tornam visível que o quantificador atua sobre a estrutura interna completa:

\[
P(x)\to Q(x)
\]

ou:

\[
P(x)\land Q(x).
\]

### e)

A fórmula procurada é:

\[
\boxed{\exists x\,(P(x)\land Q(x))}.
\]

### f)

A fórmula é:

\[
\boxed{\forall x\,(P(x)\to Q(x))}.
\]

A estrutura sob o alcance do quantificador é:

\[
P(x)\to Q(x).
\]

## Exercício 9

### a)

Temos:

\[
P(0):\quad2\cdot0<7,
\]

isto é,

\[
0<7,
\]

portanto:

\[
P(0)=V.
\]

\[
P(1):\quad2<7,
\]

logo:

\[
P(1)=V.
\]

\[
P(2):\quad4<7,
\]

logo:

\[
P(2)=V.
\]

\[
P(4):\quad8<7,
\]

portanto:

\[
P(4)=F.
\]

### b)

Como existe um valor admissível que não satisfaz \(P\),

\[
\boxed{\forall x\,P(x)=F}.
\]

### c)

Uma formulação verbal adequada é:

> Existe pelo menos um valor admissível que não satisfaz \(P\).

### d)

Simbolicamente:

\[
\boxed{
\neg(\forall x\,P(x))
\equiv
\exists x\,\neg P(x)
}.
\]

### e)

O valor:

\[
\boxed{4}
\]

é testemunho de:

\[
\exists x\,\neg P(x),
\]

pois:

\[
P(4)=F
\]

e, portanto,

\[
\neg P(4)=V.
\]

### f)

A universal exige que **todos** os valores admissíveis satisfaçam \(P\). Assim, basta um único caso em que \(P\) seja falsa para que essa exigência deixe de ser satisfeita.

### g)

O valor \(4\) exerce duas descrições compatíveis do mesmo papel lógico:

- é uma **exceção** à afirmação universal;
- é um **testemunho** de
  \[
  \exists x\,\neg P(x).
  \]

Ele mostra concretamente o caso cuja existência torna falsa a universal.

## Exercício 10

### a)

\[
P(1)=F,
\]

pois \(1\) não é múltiplo de \(3\).

\[
P(2)=F.
\]

\[
P(3)=V.
\]

\[
P(4)=F.
\]

### b)

Como:

\[
P(3)=V,
\]

temos:

\[
\boxed{\exists x\,P(x)=V}.
\]

O valor \(3\) funciona como testemunho.

### c)

O erro está em concluir, a partir de um único caso desfavorável, que nenhum caso favorável existe.

O fato de:

\[
P(2)=F
\]

não impede que outro valor satisfaça \(P\). De fato:

\[
P(3)=V.
\]

### d)

Para que:

\[
\exists x\,P(x)
\]

fosse falsa, **todos** os valores admissíveis precisariam deixar de satisfazer \(P\).

### e)

A negação correta é:

\[
\boxed{
\neg(\exists x\,P(x))
\equiv
\forall x\,\neg P(x)
}.
\]

### f)

\[
\exists x\,\neg P(x)
\]

é verdadeira.

Por exemplo,

\[
P(1)=F,
\]

portanto:

\[
\neg P(1)=V.
\]

Os valores \(2\) e \(4\) também poderiam funcionar como testemunhos.

### g)

\[
\exists x\,\neg P(x)
\]

afirma apenas que existe **algum** caso que não satisfaz \(P\).

Já:

\[
\neg(\exists x\,P(x))
\]

afirma que não existe qualquer caso favorável, o que equivale a:

\[
\forall x\,\neg P(x).
\]

Neste domínio, a primeira é verdadeira e a segunda é falsa porque \(3\) satisfaz \(P\).

## Exercício 11

### Parte I

### a)

A negação correta de:

\[
\forall x\,P(x)
\]

é a **Proposta III**:

\[
\boxed{\exists x\,\neg P(x)}.
\]

### b)

Na Proposta I:

\[
\exists x\,P(x),
\]

foi alterado apenas o quantificador. A condição \(P(x)\) permaneceu sem negação.

Na Proposta II:

\[
\forall x\,\neg P(x),
\]

foi negada apenas a condição interna. O quantificador universal permaneceu.

Na Proposta III:

\[
\exists x\,\neg P(x),
\]

as duas partes relevantes foram alteradas conjuntamente.

### c)

**Proposta I**

\[
\exists x\,P(x):
\]

> Existe pelo menos um valor admissível que satisfaz \(P\).

**Proposta II**

\[
\forall x\,\neg P(x):
\]

> Todos os valores admissíveis deixam de satisfazer \(P\).

**Proposta III**

\[
\exists x\,\neg P(x):
\]

> Existe pelo menos um valor admissível que não satisfaz \(P\).

---

### Parte II

### d)

A negação correta de:

\[
\exists x\,Q(x)
\]

é a **Proposta II**:

\[
\boxed{\forall x\,\neg Q(x)}.
\]

### e)

Na Proposta I:

\[
\exists x\,\neg Q(x),
\]

somente a condição interna foi negada.

Na Proposta III:

\[
\forall x\,Q(x),
\]

somente o quantificador foi alterado.

Na Proposta II:

\[
\forall x\,\neg Q(x),
\]

o quantificador e a condição interna foram alterados conjuntamente.

### f)

**Proposta I**

> Existe pelo menos um valor admissível que não satisfaz \(Q\).

**Proposta II**

> Todos os valores admissíveis deixam de satisfazer \(Q\).

**Proposta III**

> Todos os valores admissíveis satisfazem \(Q\).

### g)

Uma resposta possível é:

> Para negar uma afirmação quantificada desse tipo, não basta alterar apenas uma parte da expressão. É necessário observar conjuntamente o **quantificador** e a **condição interna**.

Outras formulações são aceitáveis se preservarem essa relação.

## Exercício 12

### a)

Temos:

\[
P(2):\quad2<10,
\]

portanto:

\[
P(2)=V.
\]

Da mesma forma:

\[
P(4)=V,
\qquad
P(6)=V,
\qquad
P(8)=V.
\]

Assim:

\[
\boxed{\forall x\,P(x)=V}.
\]

### b)

Não.

Entre:

\[
2,\quad4,\quad6,\quad8,
\]

todos os valores satisfazem \(x<10\).

### c)

O procedimento de Ana é correto porque a proposição quantificada está sendo interpretada relativamente aos valores admissíveis informados.

São esses quatro casos que precisam ser investigados.

### d)

É verdade que:

\[
12<10
\]

é falsa.

Entretanto, \(12\) não é um valor admissível neste domínio. Portanto, ele não pode funcionar como exceção à universal considerada.

### e)

Uma negação verbal correta é:

> Existe pelo menos um valor entre \(2\), \(4\), \(6\) e \(8\) que não satisfaz \(x<10\).

### f)

Precisaria existir, entre os próprios valores admissíveis, pelo menos um valor para o qual:

\[
x<10
\]

fosse falsa.

Não existe tal valor neste domínio.

### g)

Ao mudar os valores admissíveis, mudamos os casos sobre os quais a afirmação está sendo feita.

Assim, utilizar \(12\) não nega a proposição original: passa a introduzir outro contexto de investigação.

## Exercício 13

### a)

| Valor admissível \(a\) | \(A(a)\) | \(B(a)\) | \(A(a)\to B(a)\) | \(A(a)\land\neg B(a)\) |
|---:|:---:|:---:|:---:|:---:|
| \(2\) | \(F\) | \(F\) | \(V\) | \(F\) |
| \(3\) | \(V\) | \(F\) | \(F\) | \(V\) |
| \(5\) | \(F\) | \(V\) | \(V\) | \(F\) |
| \(6\) | \(V\) | \(V\) | \(V\) | \(F\) |

### Visual para HTML

**Função conceitual:** permitir a conferência simultânea das condições \(A(a)\), \(B(a)\), do condicional e da estrutura que caracteriza sua falha.

**Tipo:** reutilização da tabela estrutural do enunciado, agora preenchida.

**Conteúdo exato:** utilizar exatamente a tabela acima.

**Construção:** preservar as cinco colunas e a ordem dos valores \(2,3,5,6\). Não alterar rótulos nem criar nova representação.

**Ênfase:** favorecer a comparação entre:

\[
A(a)\to B(a)
\]

e:

\[
A(a)\land\neg B(a).
\]

**Implementação preferencial:** reutilizar a mesma estrutura HTML/CSS do enunciado.

### b)

A afirmação:

\[
\forall x\,(A(x)\to B(x))
\]

é falsa porque existe um caso em que o condicional interno é falso.

Logo:

\[
\boxed{\forall x\,(A(x)\to B(x))=F}.
\]

### c)

O contraexemplo é:

\[
\boxed{3}.
\]

### d)

Para \(a=3\):

\[
A(3)=V,
\]

pois \(3\) é múltiplo de \(3\).

Já:

\[
B(3)=F,
\]

pois \(3\) não é maior que \(4\).

Temos, portanto, a combinação:

\[
V,\quad F.
\]

### e)

O valor:

\[
2
\]

possui:

\[
B(2)=F,
\]

mas também:

\[
A(2)=F.
\]

Logo:

\[
A(2)\to B(2)=V.
\]

Por isso, a simples falsidade de \(B(a)\) não basta. O mesmo valor precisa satisfazer \(A(a)\).

### f)

Temos:

\[
\boxed{
\neg\left(\forall x\,(A(x)\to B(x))\right)
\equiv
\exists x\,\neg(A(x)\to B(x))
\equiv
\exists x\,(A(x)\land\neg B(x))
}.
\]

Na primeira equivalência, a negação da universal afirma a existência de um caso em que a condição interna falha.

Na segunda, utilizamos:

\[
\neg(A(x)\to B(x))
\equiv
A(x)\land\neg B(x).
\]

### g)

A forma final significa:

> Existe pelo menos um valor admissível que satisfaz \(A\) e não satisfaz \(B\).

As duas condições devem ocorrer no mesmo valor.

### h)

O valor \(3\) satisfaz:

\[
A(3)\land\neg B(3).
\]

Por isso, ele é simultaneamente:

- contraexemplo de
  \[
  \forall x\,(A(x)\to B(x));
  \]
- testemunho de
  \[
  \exists x\,(A(x)\land\neg B(x)).
  \]

São duas maneiras de descrever o mesmo caso a partir da proposição original e de sua negação.

### i)

Uma resposta possível é:

\[
\boxed{a=2}.
\]

Outra resposta válida seria \(a=6\).

### j)

Para \(a=2\):

\[
C(2)=V,
\]

pois \(2\) é par.

Mas:

\[
D(2)=F,
\]

pois \(2\) não é múltiplo de \(4\).

Assim,

\[
C(2)\land\neg D(2)
\]

é verdadeira, e \(2\) constitui um contraexemplo.

Da mesma forma, \(6\) também é válido, pois é par e não é múltiplo de \(4\).

## Exercício 14

### a)

| \(a\) | \(P(a)\) | \(Q(a)\) |
|---:|:---:|:---:|
| \(-2\) | \(F\) | \(F\) |
| \(-1\) | \(V\) | \(F\) |
| \(0\) | \(V\) | \(F\) |
| \(1\) | \(V\) | \(V\) |
| \(2\) | \(F\) | \(V\) |

### b)

**I.**

\[
\exists x\,P(x)
\]

é verdadeira.

Por exemplo:

\[
P(-1)=V.
\]

Assim, \(-1\) é um testemunho. Os valores \(0\) e \(1\) também seriam válidos.

---

**II.**

\[
\forall x\,P(x)
\]

é falsa.

Por exemplo:

\[
P(-2)=F.
\]

Logo, \(-2\) é uma exceção à universal. O valor \(2\) também poderia ser utilizado.

---

**III.**

\[
\exists x\,Q(x)
\]

é verdadeira.

Por exemplo:

\[
Q(1)=V.
\]

O valor \(2\) também é um testemunho possível.

---

**IV.**

\[
\forall x\,(P(x)\to Q(x))
\]

é falsa.

Para \(a=-1\):

\[
P(-1)=V
\]

e:

\[
Q(-1)=F.
\]

Portanto,

\[
P(-1)\to Q(-1)=F.
\]

O valor \(0\) também apresenta o mesmo padrão e constitui outro contraexemplo válido.

A informação relevante depende da estrutura examinada: nas existenciais procuramos um testemunho; numa universal simples, uma exceção pode revelar a falha; na universal com condicional, é necessário encontrar um caso com antecedente verdadeiro e consequente falso.

### c)

A negação é:

\[
\boxed{
\neg(\exists x\,Q(x))
\equiv
\forall x\,\neg Q(x)
}.
\]

Verbalmente:

> Todos os valores admissíveis deixam de satisfazer \(Q\).

Essa proposição é falsa, pois existem valores que satisfazem \(Q\), como:

\[
1
\]

e:

\[
2.
\]

### d)

Uma resposta possível é:

\[
a=-1.
\]

Nesse caso:

\[
P(-1)=V
\]

e:

\[
Q(-1)=F.
\]

Logo, o condicional:

\[
P(-1)\to Q(-1)
\]

é falso e \(-1\) funciona como contraexemplo da universal.

Também seria válida a escolha:

\[
a=0.
\]

### e)

Uma universal exige que a condição interna seja respeitada em **todos** os valores admissíveis.

Quando encontramos um caso em que:

\[
P(a)=V
\]

e:

\[
Q(a)=F,
\]

o condicional interno falha. Um único caso desse tipo já rompe a exigência universal.

### f)

**Ana**

A conclusão não é sustentada.

É verdade que:

\[
P(1)=V,
\]

mas um único caso favorável não permite concluir:

\[
\forall x\,P(x)=V.
\]

Os valores:

\[
-2
\]

e:

\[
2
\]

produzem:

\[
P(-2)=F
\]

e:

\[
P(2)=F.
\]

Uma correção adequada seria:

> \(P(1)\) mostra que existe um caso favorável, mas a afirmação universal é falsa porque nem todos os valores admissíveis satisfazem \(P\).

---

**Bruno**

A conclusão também não é sustentada.

De fato:

\[
Q(-2)=F,
\]

mas isso não elimina a possibilidade de outro valor satisfazer \(Q\).

Temos:

\[
Q(1)=V
\]

e:

\[
Q(2)=V.
\]

Logo:

\[
\exists x\,Q(x)=V.
\]

---

**Carla**

A conclusão é correta.

Como:

\[
Q(1)=V
\]

e \(1\) é admissível, temos um testemunho concreto de:

\[
\exists x\,Q(x).
\]

---

**Diego**

A conclusão é correta.

Para:

\[
a=-1,
\]

temos:

\[
P(-1)=V
\]

e:

\[
Q(-1)=F.
\]

Essa é exatamente a combinação que torna falso:

\[
P(-1)\to Q(-1).
\]

Assim, \(-1\) é um contraexemplo de:

\[
\forall x\,(P(x)\to Q(x)).
\]

### g)

Ana utiliza um único caso **favorável** para tentar estabelecer uma universal.

Isso não basta, pois a universal exige que todos os casos sejam favoráveis.

Bruno utiliza um único caso **desfavorável** para tentar eliminar uma existencial.

Isso também não basta, pois a existencial continua verdadeira enquanto houver ao menos um caso favorável.

Portanto, o problema é diferente nos dois raciocínios:

- um caso verdadeiro não estabelece uma exigência sobre todos;
- um caso falso não elimina a possibilidade de existir outro caso verdadeiro.

### h)

Carla utiliza \(1\) como **testemunho** de uma afirmação existencial:

\[
\exists x\,Q(x).
\]

Ela precisa apenas apresentar um valor admissível para o qual \(Q\) seja verdadeira.

Diego utiliza \(-1\) como **contraexemplo** de uma afirmação universal:

\[
\forall x\,(P(x)\to Q(x)).
\]

Nesse caso, o valor precisa realizar precisamente a falha do condicional:

\[
P(-1)=V
\]

e:

\[
Q(-1)=F.
\]

### i)

Uma resposta possível é escolher:

\[
\forall x\,(P(x)\to Q(x)).
\]

Essa proposição é universal e exige que, para cada valor admissível, sempre que \(P(a)\) for verdadeira, \(Q(a)\) também seja verdadeira.

Escolhendo:

\[
a=0,
\]

temos:

\[
P(0)=V
\]

e:

\[
Q(0)=F.
\]

Assim:

\[
P(0)\to Q(0)=F.
\]

Esse único valor é suficiente para revelar a falsidade da universal, pois realiza exatamente o caso que viola sua condição interna.

Também seria possível responder utilizando \(-1\) como contraexemplo, ou escolher a proposição:

\[
\forall x\,P(x)
\]

e utilizar \(-2\) ou \(2\) como exceção.
