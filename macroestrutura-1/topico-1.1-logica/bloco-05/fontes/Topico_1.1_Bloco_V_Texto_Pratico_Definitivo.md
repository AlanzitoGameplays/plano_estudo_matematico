# TÓPICO 1.1 — LÓGICA MATEMÁTICA

# BLOCO V — ARGUMENTOS, VALIDADE E DEMONSTRAÇÃO ELEMENTAR

## Texto Prático

# Exemplos Resolvidos

## Exemplo 1 — A conclusão parece aceitável, mas ela é garantida?

Considere o seguinte argumento:

> Se um relatório passou pela revisão de Ana, então foi liberado.  
> Se um relatório passou pela revisão de Bruno, então foi liberado.  
> O relatório foi liberado.  
> Portanto, o relatório passou pela revisão de Ana ou pela revisão de Bruno.

O argumento pode parecer razoável: as duas primeiras premissas apresentam maneiras pelas quais o relatório poderia ter sido liberado, e a terceira informa que a liberação ocorreu.

A questão, porém, é outra:

> As premissas realmente **garantem** que o relatório passou pela revisão de Ana ou pela revisão de Bruno?

### Resolução

### 1. Identificando os papéis

As premissas são:

1. Se o relatório passou pela revisão de Ana, então foi liberado.
2. Se o relatório passou pela revisão de Bruno, então foi liberado.
3. O relatório foi liberado.

A conclusão é:

> O relatório passou pela revisão de Ana ou pela revisão de Bruno.

Para analisar a validade, precisamos investigar a relação entre essas premissas e a conclusão.

### 2. Abstraindo o conteúdo

Defina:

\[
A:\quad \text{o relatório passou pela revisão de Ana;}
\]

\[
B:\quad \text{o relatório foi liberado;}
\]

\[
C:\quad \text{o relatório passou pela revisão de Bruno.}
\]

A forma do argumento é:

\[
A\to B
\]

\[
C\to B
\]

\[
B
\]

\[
\therefore A\lor C.
\]

Agora podemos deixar o conteúdo particular em segundo plano e perguntar se essa forma garante a conclusão.

### 3. Procurando a situação decisiva

Para mostrar que o argumento é inválido, precisamos encontrar uma **contra-avaliação**:

- todas as premissas devem ser verdadeiras;
- a conclusão deve ser falsa.

A conclusão é:

\[
A\lor C.
\]

Para que ela seja falsa, precisamos de:

\[
A=F
\qquad\text{e}\qquad
C=F.
\]

Resta verificar se ainda é possível manter as três premissas verdadeiras.

Escolha:

\[
B=V.
\]

Temos então:

\[
A=F,\qquad B=V,\qquad C=F.
\]

### 4. Verificando a avaliação

| Expressão | Valor lógico |
|---|:---:|
| \(A\to B\) | \(V\) |
| \(C\to B\) | \(V\) |
| \(B\) | \(V\) |
| \(A\lor C\) | \(F\) |

As duas condicionais são verdadeiras porque seus antecedentes são falsos:

\[
A=F
\]

e:

\[
C=F.
\]

A terceira premissa também é verdadeira:

\[
B=V.
\]

Entretanto:

\[
A\lor C=F,
\]

pois tanto \(A\) quanto \(C\) são falsas.

Portanto, conseguimos exatamente a configuração procurada:

\[
\text{todas as premissas verdadeiras}
\]

e:

\[
\text{conclusão falsa}.
\]

### 5. Conclusão

O argumento é:

\[
\boxed{\text{inválido}}.
\]

A liberação do relatório pode ter ocorrido por alguma possibilidade não representada por \(A\) nem por \(C\). As premissas dizem que essas duas situações são suficientes para produzir \(B\), mas não dizem que são as únicas maneiras pelas quais \(B\) pode ocorrer.

Por isso, mesmo que a conclusão fosse verdadeira em algum caso concreto, sua verdade não seria suficiente para tornar o argumento válido.

A contra-avaliação:

\[
A=F,\qquad B=V,\qquad C=F
\]

mostra que as premissas não garantem a conclusão.

---

## Exemplo 2 — Uma tese verdadeira não salva uma demonstração defeituosa

Considere a afirmação:

> Se \(n\) é um número inteiro par, então \(5n\) é par.

Um estudante apresenta a seguinte tentativa de demonstração:

> Para \(n=2\),
>
> \[
> 5n=10,
> \]
>
> que é par.
>
> Para \(n=4\),
>
> \[
> 5n=20,
> \]
>
> que também é par.
>
> Para \(n=6\),
>
> \[
> 5n=30,
> \]
>
> novamente par.
>
> Portanto, se \(n\) é par, \(5n\) é par.

A conclusão está correta. Mas a argumentação apresentada realmente demonstra a afirmação?

### Resolução

### 1. O que precisa ser demonstrado?

A afirmação possui a forma condicional.

A hipótese é:

> \(n\) é um número inteiro par.

A tese é:

> \(5n\) é par.

Não precisamos mostrar apenas que a propriedade funciona para alguns números pares. Precisamos estabelecer que ela funciona para **qualquer inteiro que satisfaça a hipótese**.

### 2. O que a tentativa realmente mostrou?

O estudante verificou corretamente três casos:

\[
n=2,\qquad n=4,\qquad n=6.
\]

Neles:

\[
5\cdot2=10,
\]

\[
5\cdot4=20,
\]

\[
5\cdot6=30,
\]

e os três resultados são pares.

Essas verificações não são inúteis. Elas mostram que a afirmação funciona nesses casos e podem ajudar a perceber um padrão.

Mas elas estabelecem apenas:

> a propriedade vale para \(2\), \(4\) e \(6\).

A tese exige muito mais:

> a propriedade vale para qualquer número inteiro par.

### 3. Onde está a lacuna?

A passagem problemática está entre:

> “A propriedade funcionou para alguns números pares.”


e:

> “Portanto, ela funciona para todo número inteiro par.”

Os três exemplos favoráveis não justificam essa generalização.

Mesmo uma quantidade muito maior de casos testados continuaria sendo uma coleção de casos particulares. Ainda faltaria explicar por que **qualquer** inteiro par deve produzir o mesmo comportamento.

A tese pode ser verdadeira e, ainda assim, a tentativa apresentada não constituir sua demonstração.

### 4. Que informação geral a hipótese fornece?

Se \(n\) é par, então, pela definição de número par, existe um número inteiro \(k\) tal que:

\[
n=2k.
\]

Essa expressão não representa um par específico. Ela descreve a forma de qualquer inteiro par.

É essa informação geral que podemos utilizar para estabelecer a tese.

### 5. Reconstruindo a demonstração

Suponha que \(n\) seja um número inteiro par.

Então existe um inteiro \(k\) tal que:

\[
n=2k.
\]

Multiplicando \(n\) por \(5\), temos:

\[
5n=5(2k)=10k=2(5k).
\]

Como \(k\) é inteiro, \(5k\) também é inteiro.

Portanto, \(5n\) possui a forma:

\[
2\cdot\text{(um número inteiro)}.
\]

Pela definição de número par,

\[
\boxed{5n\text{ é par}.}
\]

Assim, foi estabelecido que:

> Se \(n\) é um número inteiro par, então \(5n\) é par.

### 6. Por que essa demonstração é geral?

Na demonstração reconstruída, não escolhemos:

\[
n=2,\quad n=4,\quad n=6
\]

nem qualquer outro valor particular.

Partimos apenas daquilo que caracteriza um inteiro par:

\[
n=2k,
\]

com \(k\) inteiro.

A partir dessa forma geral, obtivemos:

\[
5n=2(5k),
\]

que novamente possui a forma de um número par.

Os exemplos particulares mostravam que a afirmação funcionava em alguns casos. A demonstração reconstruída explica **por que ela precisa funcionar em todos os casos abrangidos pela hipótese**.

# Quiz

## Questão 1

Considere o argumento:

\[
p\lor q
\]

\[
\neg p
\]

\[
\therefore q.
\]

Qual alternativa descreve corretamente sua organização?

**A)** \(p\lor q\) e \(\neg p\) são premissas, \(q\) é a conclusão e \(\therefore\) apenas marca a afirmação apresentada como conclusão.

**B)** \(\therefore\) conecta \(\neg p\) e \(q\), formando uma nova proposição composta.

**C)** Apenas \(p\lor q\) é premissa; \(\neg p\) e \(q\) são duas conclusões sucessivas.

**D)** As três expressões são premissas, pois todas participam da mesma estrutura argumentativa.

---

## Questão 2

Qual afirmação distingue corretamente verdade, validade e solidez?

**A)** Um argumento é válido sempre que sua conclusão é verdadeira.

**B)** Se uma das premissas é falsa, o argumento é necessariamente inválido.

**C)** Proposições podem ser verdadeiras ou falsas; argumentos podem ser válidos ou inválidos; um argumento sólido é válido e possui premissas verdadeiras.

**D)** Todo argumento válido é automaticamente sólido, independentemente do valor lógico de suas premissas.

---

## Questão 3

Qual situação constitui uma contra-avaliação para um argumento?

**A)** Todas as premissas são verdadeiras e a conclusão também é verdadeira.

**B)** Alguma premissa é falsa e a conclusão é falsa.

**C)** Todas as premissas são falsas e a conclusão é verdadeira.

**D)** Todas as premissas são verdadeiras e a conclusão é falsa.

---

## Questão 4

Compare:

### I

\[
A\to B
\]

\[
\neg B
\]

\[
\therefore\neg A
\]

### II

\[
A\to B
\]

\[
\neg A
\]

\[
\therefore\neg B.
\]

Qual alternativa é correta?

**A)** As duas formas são válidas porque ambas utilizam o mesmo condicional.

**B)** I é válida por modus tollens; II é inválida por negação do antecedente.

**C)** I é inválida por afirmar o consequente; II é válida por modus ponens.

**D)** As duas formas são inválidas porque nenhuma utiliza diretamente \(A\) como segunda premissa.

---

## Questão 5

Considere:

\[
A\lor B
\]

\[
\neg A.
\]

Qual conclusão pode ser obtida legitimamente em um único passo?

**A)**

\[
\neg B
\]

**B)**

\[
A
\]

**C)**

\[
B
\]

**D)**

\[
A\land B
\]

# Exercícios

## Exercício 1 — Onde está o argumento?

Analise as quatro estruturas.

### I

> Se um número é múltiplo de \(4\), então ele é par.  
> \(20\) é múltiplo de \(4\).  
> Logo, \(20\) é par.

### II

> \(7-3\) é positivo, pois \(7-3=4\) e \(4>0\).

### III

> \(12\) é par.  
> \(15\) é ímpar.  
> \(20>7\).

### IV

\[
p\lor q
\]

\[
\neg q
\]

\[
\therefore p.
\]

### a)

Identifique quais das quatro estruturas apresentam um argumento.

### b)

Nas estruturas que constituem argumentos, identifique:

- a premissa ou as premissas;
- a conclusão.

### c)

Explique por que a estrutura III, embora contenha várias proposições, não apresenta por si só uma inferência.

### d)

Na estrutura II, a conclusão aparece antes das razões apresentadas para sustentá-la.

Reorganize-a na forma:

\[
\text{premissas}
\]

\[
\therefore\text{ conclusão}.
\]

### e)

Compare as estruturas I e IV.

Uma utiliza linguagem verbal e a outra linguagem simbólica. Explique o que precisa existir em ambas para que sejam reconhecidas como argumentos, independentemente da forma de escrita.

---

## Exercício 2 — Verdade não é validade; validade não é solidez

Em cada cenário, considere que os valores lógicos indicados são os valores assumidos pelas proposições naquela situação.

### Cenário I

\[
A\to B
\]

\[
A
\]

\[
\therefore B
\]

com:

\[
A=F,
\qquad
B=V.
\]

### Cenário II

\[
A\lor B
\]

\[
\therefore A
\]

com:

\[
A=V,
\qquad
B=V.
\]

### Cenário III

\[
A\land B
\]

\[
\therefore A
\]

com:

\[
A=V,
\qquad
B=V.
\]

### a)

Em cada cenário, determine o valor lógico de todas as premissas e da conclusão.

### b)

Classifique cada **forma de argumento** como válida ou inválida.

Não decida a validade apenas pela avaliação particular fornecida.

### c)

Em quais cenários estão satisfeitas simultaneamente as duas condições necessárias para a solidez?

Justifique levando em conta:

- a validade da forma;
- a verdade das premissas na situação apresentada.

### d)

Um estudante observa o Cenário II e afirma:

> “A premissa é verdadeira e a conclusão também é verdadeira. Portanto, o argumento é válido.”

Analise a justificativa.

Que informação ainda precisa ser considerada para decidir validade?

### e)

Outro estudante observa o Cenário I e afirma:

> “Como \(A\) é falsa, o argumento é inválido.”

Corrija esse raciocínio distinguindo o valor lógico de uma premissa da validade da forma argumentativa.

---

## Exercício 3 — Construindo uma contra-avaliação

Considere o argumento:

\[
A\lor B
\]

\[
A\to C
\]

\[
\therefore C.
\]

### a)

Antes de escolher qualquer valor lógico, descreva qual configuração uma avaliação precisa produzir para funcionar como contra-avaliação desse argumento.

### b)

Construa uma atribuição de valores para:

\[
A,\qquad B,\qquad C
\]

que torne simultaneamente verdadeiras as duas premissas e falsa a conclusão.

### c)

Verifique separadamente, usando a atribuição escolhida:

\[
A\lor B,
\]

\[
A\to C,
\]

e:

\[
C.
\]

Organize a conferência em uma pequena tabela ou em linhas separadas.

### d)

Explique por que a avaliação construída é suficiente para decidir a validade do argumento.

### e)

Considere agora a avaliação:

\[
A=V,
\qquad
B=F,
\qquad
C=V.
\]

Verifique as premissas e a conclusão.

Essa avaliação também é uma contra-avaliação?

Explique o que ela informa — e o que não informa — sobre a validade.

---

## Exercício 4 — Onde devemos procurar a falha?

Considere:

\[
A\lor B
\]

\[
A\to C
\]

\[
B\to C
\]

\[
\therefore C.
\]

Em vez de testar atribuições aleatoriamente, investigue diretamente a possibilidade de construir uma contra-avaliação.

### a)

Para que uma contra-avaliação exista, qual deve ser o valor lógico da conclusão \(C\)?

### b)

Suponha esse valor para \(C\).

Que valor \(A\) precisaria possuir para que:

\[
A\to C
\]

continuasse verdadeira?

### c)

Na mesma situação, que valor \(B\) precisaria possuir para que:

\[
B\to C
\]

continuasse verdadeira?

### d)

Os valores encontrados para \(A\) e \(B\) são compatíveis com a exigência de que:

\[
A\lor B
\]

seja verdadeira?

A partir dessa análise, determine se é possível construir uma contra-avaliação.

### e)

Conclua se o argumento é válido ou inválido e justifique pela existência ou inexistência da configuração:

> todas as premissas verdadeiras e conclusão falsa.

### f)

Reúna as três premissas numa única conjunção e escreva o condicional que possui essa conjunção como antecedente e \(C\) como consequente.

Utilize a forma:

\[
[(\text{premissas})]\to C.
\]

### g)

Explique como a tentativa de falsificar esse condicional está relacionada à procura por uma contra-avaliação do argumento original.

---

## Exercício 5 — Reconhecendo formas fundamentais

Em cada argumento, identifique a regra de inferência utilizada:

- modus ponens;
- modus tollens;
- silogismo hipotético;
- silogismo disjuntivo.

Além do nome, indique quais expressões ocupam os papéis estruturais relevantes.

### I

\[
(p\land q)\to r
\]

\[
p\land q
\]

\[
\therefore r.
\]

### II

\[
p\to(q\lor r)
\]

\[
\neg(q\lor r)
\]

\[
\therefore\neg p.
\]

### III

\[
(p\lor q)\to r
\]

\[
r\to s
\]

\[
\therefore(p\lor q)\to s.
\]

### IV

\[
(p\land q)\lor r
\]

\[
\neg r
\]

\[
\therefore p\land q.
\]

### V

\[
p\lor(q\land r)
\]

\[
\neg p
\]

\[
\therefore q\land r.
\]

### a)

Nomeie a regra correspondente em cada caso.

### b)

Nos argumentos I e II, identifique o que desempenha o papel de \(A\) e de \(B\) nas formas abstratas:

\[
A\to B,\quad A\quad\therefore B
\]

e:

\[
A\to B,\quad\neg B\quad\therefore\neg A.
\]

### c)

No argumento III, identifique as três expressões que desempenham os papéis de \(A\), \(B\) e \(C\) em:

\[
A\to B,
\qquad
B\to C,
\qquad
\therefore A\to C.
\]

### d)

Nos argumentos IV e V, explique por que uma fórmula composta inteira pode ocupar o lugar de uma das alternativas de uma disjunção.

### e)

Uma regra de inferência utilizada acima afirma que duas fórmulas são logicamente equivalentes?

Explique brevemente a diferença entre usar uma forma para **obter uma conclusão** e escrever uma equivalência como:

\[
A\equiv B.
\]

---

## Exercício 6 — Aplicando a regra à estrutura inteira

Em cada item, analise as premissas e determine o que pode ser obtido legitimamente em **um único passo** com as regras de inferência disponíveis.

Quando uma conclusão puder ser obtida:

- escreva-a;
- identifique a regra utilizada;
- indique a correspondência entre as fórmulas concretas e sua forma abstrata.

### a)

\[
\neg p\to(q\lor r)
\]

\[
\neg p.
\]

### b)

\[
(p\land q)\lor r
\]

\[
\neg r.
\]

### c)

\[
(p\lor q)\to r
\]

\[
r\to\neg s.
\]

### d)

\[
(p\land q)\to r
\]

\[
\neg r.
\]

### e)

Considere:

\[
(p\land q)\to r
\]

\[
p.
\]

Um estudante propõe concluir:

\[
r.
\]

É possível obter \(r\) legitimamente em um único passo com as regras disponíveis?

Sua justificativa deve observar a estrutura **inteira** da primeira premissa, e não apenas parte dela.

### f)

Escolha um dos itens em que uma conclusão pode ser legitimamente obtida e explique por que a passagem realizada é uma **inferência**, e não uma afirmação de que alguma premissa seja logicamente equivalente à conclusão.

---

## Exercício 7 — Formas válidas e imitações próximas

### Parte I — Antecedente e consequente

Compare:

### Forma I

\[
A\to B
\]

\[
A
\]

\[
\therefore B
\]

### Forma II

\[
A\to B
\]

\[
B
\]

\[
\therefore A.
\]

### a)

Identifique qual forma é válida e nomeie a regra correspondente.

### b)

Identifique a forma inválida pelo nome construído no Texto Teórico.

### c)

Construa uma atribuição de valores para \(A\) e \(B\) que torne verdadeiras as premissas da forma inválida e falsa sua conclusão.

### d)

Explique, em linguagem verbal, por que a direção estabelecida por:

\[
A\to B
\]

não autoriza a passagem realizada pela forma inválida.

---

### Parte II — Negando uma das posições

Compare:

### Forma III

\[
A\to B
\]

\[
\neg B
\]

\[
\therefore\neg A
\]

### Forma IV

\[
A\to B
\]

\[
\neg A
\]

\[
\therefore\neg B.
\]

### e)

Identifique qual forma é válida e nomeie-a.

### f)

Identifique a forma inválida.

### g)

Construa uma contra-avaliação para a forma inválida e verifique:

- a primeira premissa;
- a segunda premissa;
- a conclusão.

### h)

Explique por que negar o antecedente não autoriza, em geral, negar o consequente.

---

### Parte III — Transferência para um argumento verbal

Considere:

> Se a senha foi digitada corretamente, então o sistema libera o acesso.  
> O sistema liberou o acesso.  
> Portanto, a senha foi digitada corretamente.

### i)

Defina proposições adequadas para formalizar o argumento.

### j)

Escreva sua forma simbólica.

### k)

Classifique-a como válida ou inválida e identifique sua estrutura.

### l)

Explique por que a liberação do acesso, por si só, não garante a conclusão apresentada.

Sua análise deve tratar da direção lógica do condicional, não de possíveis detalhes técnicos do sistema.

---

## Exercício 8 — Qual regra realmente serve?

Em cada item, determine se as premissas permitem obter alguma conclusão indicada pela estrutura em **um único passo**.

Quando permitirem:

- escreva a conclusão;
- identifique a regra;
- justifique brevemente por que ela se aplica.

### I

\[
A\to B
\]

\[
B\to C.
\]

Que relação condicional entre \(A\) e \(C\) pode ser obtida?

### II

\[
A\lor B
\]

\[
\neg B.
\]

Qual das alternativas da primeira premissa pode ser concluída?

### III

\[
(p\land q)\to r
\]

\[
p\land q.
\]

Qual conclusão pode ser obtida?

### IV

\[
p\to(q\lor r)
\]

\[
\neg(q\lor r).
\]

Que conclusão sobre \(p\) pode ser obtida?

### V

Considere:

\[
A\to B
\]

\[
\neg A
\]

e a conclusão proposta:

\[
\neg B.
\]

Alguma das quatro regras válidas disponíveis autoriza essa conclusão em um único passo?

Se não, identifique o problema estrutural da tentativa.

---

## Exercício 9 — Encadeamento de inferências

Considere como premissas iniciais:

\[
p\lor q
\]

\[
\neg p
\]

\[
q\to r
\]

\[
r\to s.
\]

Pretende-se estabelecer:

\[
s.
\]

### a)

Identifique uma afirmação que possa ser legitimamente obtida a partir das premissas já disponíveis.

Indique exatamente quais informações utiliza e qual regra justifica a passagem.

### b)

Utilize a nova informação obtida, quando ela estiver legitimamente disponível, para continuar o raciocínio.

Prossiga até alcançar:

\[
s.
\]

### c)

Registre cada passo indicando:

- a afirmação obtida;
- as informações utilizadas;
- a justificativa da inferência.

### Visual para HTML

**Função conceitual:** tornar perceptível que uma cadeia de inferências não é apenas uma sequência de fórmulas: cada nova linha precisa possuir uma origem legítima e só pode ser reutilizada depois de estabelecida.

**Tipo:** tabela de encadeamento e justificação.

**Conteúdo exato:**

| Passo | Afirmação disponível ou obtida | Informações utilizadas | Justificativa |
|---:|---|---|---|
| Premissas | \(p\lor q\); \(\neg p\); \(q\to r\); \(r\to s\) | — | dadas |
| 1 | ____________________ | ____________________ | ____________________ |
| 2 | ____________________ | ____________________ | ____________________ |
| 3 | ____________________ | ____________________ | ____________________ |

**Construção:** a primeira coluna deve marcar a ordem lógica dos passos. A segunda registra a afirmação disponível ou obtida. A terceira registra as informações das quais ela depende. A quarta registra a regra ou justificativa utilizada. As premissas iniciais devem aparecer como informações já disponíveis; as conclusões intermediárias e suas justificativas devem permanecer vazias.

**Ênfase:** destacar estruturalmente a relação entre **afirmação**, **origem** e **justificação**. A tabela deve permitir perceber quando uma conclusão intermediária passa a poder ser utilizada numa etapa posterior.

**Restrições de fidelidade:** não preencher a cadeia. Não antecipar os nomes das regras nas células vazias. Não utilizar \(\to\) como seta gráfica. Não depender apenas de cor. Não criar fluxograma decorativo. Não introduzir novas regras de inferência. Não acrescentar premissas.

**Implementação preferencial:** HTML/CSS. Não utilizar SVG.

### d)

Explique em que momento cada conclusão intermediária passa a estar legitimamente disponível para ser utilizada como premissa de um passo posterior.

### e)

Examine a dependência entre os passos que você construiu.

É possível obter a conclusão final sem antes estabelecer determinadas conclusões intermediárias?

Justifique com base nas premissas disponíveis, sem apenas reorganizar visualmente as linhas.

---

Considere agora a seguinte tentativa de resolução construída com as mesmas premissas:

### Passo 1

\[
r
\]

Justificativa apresentada:

> De \(q\to r\) e \(q\), por modus ponens.

### Passo 2

\[
q
\]

Justificativa apresentada:

> De \(p\lor q\) e \(\neg p\), por silogismo disjuntivo.

### Passo 3

\[
s
\]

Justificativa apresentada:

> De \(r\to s\) e \(r\), por modus ponens.

### f)

Localize a primeira linha que não está legitimamente justificada **no momento em que aparece**.

### g)

A justificativa escrita nessa linha corresponde a uma forma de inferência válida em si mesma?

Explique por que isso ainda não basta para tornar o passo legítimo naquela posição da cadeia.

### h)

Reorganize a resolução de modo que cada afirmação utilizada como premissa já tenha sido previamente fornecida ou legitimamente obtida.

### i)

Explique por que uma conclusão intermediária não pode ser utilizada apenas porque sabemos que ela aparecerá mais adiante no raciocínio.

---

## Exercício 10 — Testar, demonstrar ou refutar?

### Parte I — Duas abordagens para uma afirmação geral

Considere a afirmação:

> Se \(n\) é um número inteiro par, então \(n+6\) é par.

Dois estudantes investigam essa afirmação de maneiras diferentes.

### Abordagem A

O primeiro estudante escolhe alguns números pares:

Para:

\[
n=2,
\]

temos:

\[
n+6=8.
\]

Para:

\[
n=8,
\]

temos:

\[
n+6=14.
\]

Para:

\[
n=20,
\]

temos:

\[
n+6=26.
\]

Nos três casos, \(n+6\) é par.

### Abordagem B

O segundo estudante começa escrevendo:

\[
n=2k,
\]

com \(k\) inteiro, e procura utilizar essa informação para analisar \(n+6\) sem escolher um valor particular para \(n\).

### a)

O que a Abordagem A realmente estabelece sobre os valores:

\[
2,\quad 8,\quad 20?
\]

### b)

Explique por que os três casos favoráveis, mesmo estando corretos, não são suficientes para demonstrar a afirmação geral.

### c)

Complete a Abordagem B.

Parta de:

\[
n=2k
\]

e transforme \(n+6\) até obter uma expressão da forma:

\[
2\cdot\text{(um número inteiro)}.
\]

### d)

Justifique por que a expressão obtida permite concluir que \(n+6\) é par.

### e)

Compare as duas abordagens. Por que a Abordagem B consegue tratar qualquer inteiro par abrangido pela hipótese, enquanto a Abordagem A examina apenas casos particulares?

---

### Parte II — Quando um único caso é suficiente

Considere agora a afirmação:

> Para todo número real \(x\),
>
> \[
> x^2\geq x.
> \]

### f)

Procure um número real para o qual:

\[
x^2<x.
\]

### g)

Substitua o valor escolhido e verifique numericamente a desigualdade.

### h)

Explique por que um único valor desse tipo é suficiente para refutar a afirmação universal.

### i)

Compare as duas situações deste exercício:

- vários casos favoráveis na Parte I;
- um único caso desfavorável na Parte II.

Por que essas evidências não possuem a mesma força lógica?

---

## Exercício 11 — Construindo uma demonstração direta

Considere a afirmação:

> Se \(n\) é um número inteiro par, então \(3n+4\) é par.

Construa uma demonstração direta.

### a)

Identifique a **hipótese**.

### b)

Identifique a **tese**.

### c)

Utilize a definição de número par para escrever \(n\) na forma:

\[
n=2k,
\]

indicando que tipo de número \(k\) deve ser.

### d)

Substitua essa expressão em:

\[
3n+4
\]

e desenvolva as igualdades necessárias até obter uma expressão da forma:

\[
2\cdot\text{(uma expressão)}.
\]

### e)

Explique por que a expressão que aparece multiplicando \(2\) representa um número inteiro.

### f)

Conclua explicitamente por que:

\[
3n+4
\]

é par.

### g)

Na demonstração construída, foi necessário escolher algum valor particular como:

\[
n=2,\qquad n=4,\qquad n=10?
\]

Explique por que a ausência dessa escolha é importante para a generalidade da demonstração.

### h)

Reescreva sua demonstração de forma contínua e concisa, mantendo visíveis a hipótese, os passos centrais e a conclusão.

---

## Exercício 12 — Demonstrando pela contrapositiva

Considere \(x\) um número real e a afirmação:

> Se
>
> \[
> 5x+2>17,
> \]
>
> então
>
> \[
> x>3.
> \]

Pretende-se demonstrar essa afirmação por **contraposição**.

### a)

Considere:

\[
A:\quad 5x+2>17
\]

e:

\[
B:\quad x>3.
\]

Escreva simbolicamente a forma da afirmação original.

### b)

Escreva a forma simbólica de sua contrapositiva utilizando:

\[
\neg B\to\neg A.
\]

### c)

Traduza:

\[
\neg B
\]

para uma desigualdade envolvendo \(x\).

### d)

Traduza:

\[
\neg A
\]

para uma desigualdade envolvendo \(5x+2\).

### e)

Parta da desigualdade correspondente a \(\neg B\) e desenvolva uma demonstração que chegue à desigualdade correspondente a \(\neg A\).

Justifique as operações relevantes realizadas com a desigualdade.

### f)

Depois de estabelecer a contrapositiva, explique por que a afirmação original também fica demonstrada.

### g)

Compare agora esta demonstração com o **modus tollens**.

No modus tollens, qual proposição já está disponível como premissa?

Na demonstração por contraposição, qual proposição é justamente aquilo que ainda precisa ser estabelecido?

### h)

Explique por que demonstrar:

\[
\neg B\to\neg A
\]

não significa utilizar:

\[
A\to B
\]

como premissa durante a própria demonstração.

---

## Exercício 13 — Onde está a contradição?

Considere a afirmação:

> Não existem dois números inteiros consecutivos que sejam ambos pares.

Pretende-se demonstrá-la por contradição.

### a)

Identifique a tese que precisa ser estabelecida.

### b)

Escreva, em linguagem verbal, a **negação** dessa tese.

### c)

Assuma temporariamente a negação.

Considere, portanto, dois inteiros consecutivos:

\[
n
\]

e:

\[
n+1,
\]

e suponha que ambos sejam pares.

### d)

Como \(n\) foi assumido par, represente-o utilizando a definição de número par e um inteiro adequado.

### e)

Faça o mesmo para:

\[
n+1.
\]

Utilize uma letra diferente para o inteiro que aparece nessa segunda representação.

### f)

Compare as duas igualdades obtidas e desenvolva-as até chegar a uma relação que envolva:

\[
1
\]

e o dobro de um número inteiro.

### g)

Identifique precisamente a incompatibilidade matemática produzida.

Não responda apenas que “a conta deu errado”. Explique quais duas condições não podem ser satisfeitas simultaneamente.

### h)

Por que essa incompatibilidade obriga a rejeitar a suposição temporária feita no item c?

### i)

Conclua a tese original.

### j)

Considere agora a seguinte descrição de uma tentativa de prova:

> “Assumi a negação da tese, fiz algumas contas e não consegui continuar. Portanto, encontrei uma contradição.”

Essa justificativa é suficiente?

Explique a diferença entre:

- encontrar uma dificuldade no raciocínio;
- obter uma incompatibilidade lógica ou matemática real.

---

## Exercício 14 — Demonstrando por casos

Sabe-se que um número real \(x\) é necessariamente um dos três valores:

\[
-2,\qquad 0,\qquad 2.
\]

Demonstre que:

\[
x^2\leq4.
\]

### a)

Liste todas as possibilidades fornecidas pela hipótese.

### b)

Organize a demonstração em três casos.

Em cada caso:

1. fixe uma das possibilidades para \(x\);
2. calcule \(x^2\);
3. verifique a tese
   \[
   x^2\leq4.
   \]

### c)

Depois de analisar os três casos, explique por que a tese fica estabelecida para qualquer \(x\) abrangido pela hipótese.

### d)

Por que essa demonstração por casos não é equivalente a escolher arbitrariamente três exemplos favoráveis de um conjunto maior de possibilidades?

Sua resposta deve considerar a **cobertura** fornecida pelos casos.

---

Considere agora a seguinte tentativa:

> **Caso 1:** \(x=-2\). Verifica-se que \(x^2\leq4\).
>
> **Caso 2:** \(x=0\). Verifica-se que \(x^2\leq4\).
>
> Portanto,
>
> \[
> x^2\leq4.
> \]

### e)

Os dois casos efetivamente analisados estão corretos?

### f)

Mesmo que estejam corretos, a demonstração completa está terminada?

### g)

Identifique exatamente qual possibilidade fornecida pela hipótese não foi analisada.

### h)

Explique por que duas ramificações corretas não compensam a ausência de uma possibilidade admissível.

### i)

Complete a tentativa de modo que os casos cubram integralmente a hipótese e conduzam à mesma tese.

---

## Exercício 15 — Duas direções para uma equivalência

Considere \(x\) um número real e a afirmação:

\[
x>4
\leftrightarrow
3x-2>10.
\]

### a)

Separe a bicondicional nas duas afirmações condicionais que precisam ser estabelecidas.

Escreva-as simbolicamente.

### b)

Demonstre a primeira direção:

\[
x>4\to3x-2>10.
\]

Parta da hipótese dessa direção e desenvolva as desigualdades até alcançar sua tese.

### c)

Demonstre agora a direção recíproca:

\[
3x-2>10\to x>4.
\]

### d)

Ao manipular as desigualdades, justifique por que as multiplicações ou divisões efetuadas não invertem o sentido da desigualdade.

### e)

Depois de estabelecer as duas direções, conclua a bicondicional:

\[
x>4
\leftrightarrow
3x-2>10.
\]

### f)

Explique por que demonstrar apenas:

\[
x>4\to3x-2>10
\]

não seria suficiente para estabelecer toda a bicondicional.

---

Um estudante apresenta a seguinte tentativa:

> Suponha:
>
> \[
> x>4.
> \]
>
> Multiplicando por \(3\),
>
> \[
> 3x>12.
> \]
>
> Subtraindo \(2\),
>
> \[
> 3x-2>10.
> \]
>
> Portanto,
>
> \[
> x>4
> \leftrightarrow
> 3x-2>10.
> \]

### g)

Qual direção o estudante efetivamente demonstrou?

### h)

Qual direção ainda não foi estabelecida?

### i)

Complete a tentativa acrescentando a parte necessária para justificar legitimamente a bicondicional.

---

## Exercício 16 — Auditoria e integração

Considere \(n\) um número inteiro e a tese:

> Se \(n+4\) é par, então \(n\) é par.

Quatro estudantes apresentam tentativas diferentes de demonstração.

---

### Tentativa I

> Suponha que \(n+4\) seja par.
>
> Então existe um inteiro \(k\) tal que:
>
> \[
> n+4=2k.
> \]
>
> Logo:
>
> \[
> n=2k-4=2(k-2).
> \]
>
> Como \(k-2\) é inteiro, \(n\) é par.

---

### Tentativa II

> Suponha que \(n\) seja par.
>
> Então existe um inteiro \(k\) tal que:
>
> \[
> n=2k.
> \]
>
> Assim:
>
> \[
> n+4=2k+4=2(k+2).
> \]
>
> Como \(k+2\) é inteiro, \(n+4\) é par.
>
> Portanto, se \(n+4\) é par, então \(n\) é par.

---

### Tentativa III

> Suponha que \(n+4\) seja par.
>
> Então:
>
> \[
> n+4=2k
> \]
>
> para algum inteiro \(k\).
>
> Como \(n\) é par, podemos escrever:
>
> \[
> n=2m
> \]
>
> para algum inteiro \(m\).
>
> Desse modo:
>
> \[
> n+4=2m+4=2(m+2),
> \]
>
> o que é compatível com a hipótese.
>
> Logo, \(n\) é par.

---

### Tentativa IV

> Para \(n=0\),
>
> \[
> n+4=4
> \]
>
> é par, e \(n\) também é par.
>
> Para \(n=4\),
>
> \[
> n+4=8
> \]
>
> é par, e \(n\) também é par.
>
> Para \(n=10\),
>
> \[
> n+4=14
> \]
>
> é par, e \(n\) também é par.
>
> Portanto, sempre que \(n+4\) é par, \(n\) é par.

### a)

Identifique qual das quatro tentativas estabelece legitimamente a tese.

### b)

Para cada tentativa, registre:

- qual condição foi efetivamente tomada como ponto de partida;
- qual conclusão foi efetivamente obtida;
- qual foi o passo ou estratégia central utilizado.

### c)

Nas Tentativas II, III e IV, localize o **primeiro defeito lógico relevante**.

Não se limite a dizer que a tentativa está incorreta; identifique onde a legitimidade do raciocínio é perdida.

### d)

Na Tentativa II, todas as manipulações algébricas podem estar corretas e, ainda assim, a tese original não ter sido demonstrada.

Explique por quê, comparando a direção demonstrada com a direção exigida pela tese.

### e)

Na Tentativa III, identifique a afirmação que foi utilizada antes de ser legitimamente estabelecida.

Explique por que esse uso torna o raciocínio circular.

### f)

Na Tentativa IV, explique separadamente:

1. o que os três casos testados realmente mostram;
2. o que eles não são suficientes para mostrar.

### g)

Escolha **uma** das Tentativas II, III ou IV e reconstrua-a de modo que passe a constituir uma demonstração legítima da tese original.

Sua reconstrução não precisa conservar os mesmos passos da tentativa defeituosa.

### h)

Depois de reconstruir o raciocínio, redija uma versão final concisa da demonstração.

A apresentação deve permitir ao leitor recuperar:

- a hipótese;
- a informação obtida da hipótese;
- os passos centrais;
- a razão da conclusão.

Não é necessário narrar tentativas abandonadas durante a descoberta da solução.

### i)

Compare a versão final redigida no item h com o processo utilizado para encontrá-la.

Por que uma demonstração pode ser apresentada numa ordem mais limpa do que a sequência de tentativas que levou à sua descoberta?

### j)

Um estudante analisa a Tentativa II e afirma:

> “Como essa tentativa não demonstra a tese, então a tese é falsa.”

Analise essa conclusão.

Sua resposta deve distinguir cuidadosamente as afirmações:

> “Este argumento não demonstra a tese.”


e:

> “A tese é falsa.”

# Gabarito Comentado

## Quiz

### Questão 1

**Alternativa A.**

\[
p\lor q
\]

e

\[
\neg p
\]

são as premissas, enquanto \(q\) é a conclusão. O símbolo \(\therefore\) apenas marca a afirmação apresentada como conclusão; ele não funciona como conectivo proposicional.

### Questão 2

**Alternativa C.**

Verdade e falsidade são propriedades de proposições; validade e invalidade dizem respeito aos argumentos. Um argumento é sólido quando é válido e, além disso, possui premissas verdadeiras.

### Questão 3

**Alternativa D.**

Uma contra-avaliação precisa produzir exatamente:

\[
\text{todas as premissas verdadeiras}
\]

e

\[
\text{conclusão falsa}.
\]

Uma única avaliação desse tipo é suficiente para mostrar que o argumento é inválido.

### Questão 4

**Alternativa B.**

A forma I é um **modus tollens**, portanto válida:

\[
A\to B,\qquad \neg B\qquad \therefore\neg A.
\]

A forma II é uma **negação do antecedente**, portanto inválida:

\[
A\to B,\qquad \neg A\qquad \therefore\neg B.
\]

### Questão 5

**Alternativa C.**

De:

\[
A\lor B
\]

e

\[
\neg A,
\]

obtemos:

\[
B
\]

por **silogismo disjuntivo**.

## Exercício 1

### a)

As estruturas que apresentam argumentos são:

\[
\boxed{I,\ II\ \text{e}\ IV.}
\]

A estrutura III contém apenas proposições colocadas lado a lado, sem que alguma delas seja apresentada como conclusão sustentada pelas demais.

### b)

Na estrutura I, as premissas são:

> Se um número é múltiplo de \(4\), então ele é par.

e:

> \(20\) é múltiplo de \(4\).

A conclusão é:

> \(20\) é par.

Na estrutura II, a conclusão é:

> \(7-3\) é positivo.

As razões apresentadas para sustentá-la são:

\[
7-3=4
\]

e:

\[
4>0.
\]

Na estrutura IV, as premissas são:

\[
p\lor q
\]

e:

\[
\neg q.
\]

A conclusão é:

\[
p.
\]

### c)

Na estrutura III, temos três proposições, mas nenhuma é apresentada como decorrência das outras. Uma coleção de proposições não se torna um argumento apenas por conter várias afirmações.

### d)

Uma reorganização possível é:

\[
7-3=4
\]

\[
4>0
\]

\[
\therefore 7-3\text{ é positivo}.
\]

A ordem verbal original não altera os papéis lógicos: a conclusão pode aparecer antes das razões que a sustentam.

### e)

Tanto em linguagem verbal quanto simbólica, deve existir uma organização inferencial: algumas proposições funcionam como **premissas**, e outra é apresentada como **conclusão** sustentada por elas.

A presença de palavras como “logo” ou do símbolo \(\therefore\) pode sinalizar essa organização, mas não é, sozinha, aquilo que constitui o argumento.

## Exercício 2

### a)–c)

#### Cenário I

Temos:

\[
A=F,\qquad B=V.
\]

Logo:

\[
A\to B=V.
\]

Assim:

- primeira premissa: \(V\);
- segunda premissa \(A\): \(F\);
- conclusão \(B\): \(V\).

A forma:

\[
A\to B
\]

\[
A
\]

\[
\therefore B
\]

é válida: trata-se de **modus ponens**.

Entretanto, na avaliação apresentada, o argumento não é sólido, pois uma de suas premissas é falsa.

Isso mostra que:

\[
\boxed{\text{premissa falsa não implica argumento inválido}.}
\]

#### Cenário II

Com:

\[
A=V,\qquad B=V,
\]

temos:

\[
A\lor B=V
\]

e a conclusão:

\[
A=V.
\]

Apesar de premissa e conclusão serem verdadeiras nessa avaliação, a forma:

\[
A\lor B
\]

\[
\therefore A
\]

é inválida.

Por exemplo, tome:

\[
A=F,\qquad B=V.
\]

Então:

\[
A\lor B=V
\]

e:

\[
A=F.
\]

Temos uma contra-avaliação. Portanto, a forma é inválida e não pode ser sólida.

#### Cenário III

Com:

\[
A=V,\qquad B=V,
\]

temos:

\[
A\land B=V
\]

e:

\[
A=V.
\]

A forma:

\[
A\land B
\]

\[
\therefore A
\]

é válida. Como a premissa também é verdadeira na situação apresentada, o argumento é sólido.

### d)

A justificativa do estudante é incorreta.

Encontrar uma avaliação em que premissa e conclusão são verdadeiras mostra apenas que essa avaliação é **compatível** com validade. Para decidir validade, precisamos saber se existe alguma situação em que todas as premissas sejam verdadeiras e a conclusão falsa.

No Cenário II, tal situação existe.

### e)

A falsidade de \(A\) na avaliação apresentada não torna a forma inválida.

Validade diz respeito à relação geral entre premissas e conclusão. A forma continua sendo modus ponens e, portanto, válida.

O que a falsidade de \(A\) impede, nessa situação particular, é que o argumento seja sólido.

## Exercício 3

### a)

Uma contra-avaliação precisa satisfazer simultaneamente:

\[
A\lor B=V,
\]

\[
A\to C=V,
\]

e:

\[
C=F.
\]

### b)–c)

Uma resposta possível é:

\[
A=F,\qquad B=V,\qquad C=F.
\]

Verificando:

| Expressão | Valor |
|---|:---:|
| \(A\lor B\) | \(V\) |
| \(A\to C\) | \(V\) |
| \(C\) | \(F\) |

Logo, todas as premissas são verdadeiras e a conclusão é falsa.

### d)

Essa única avaliação já é suficiente para mostrar que o argumento é:

\[
\boxed{\text{inválido}}.
\]

A validade exige que nenhuma contra-avaliação exista.

### e)

Para:

\[
A=V,\qquad B=F,\qquad C=V,
\]

temos:

\[
A\lor B=V,
\]

\[
A\to C=V,
\]

e:

\[
C=V.
\]

Portanto, essa avaliação **não** é uma contra-avaliação.

Ela mostra apenas uma situação em que premissas verdadeiras convivem com conclusão verdadeira. Isso não basta para estabelecer validade.

## Exercício 4

### a)

Para procurar uma contra-avaliação, começamos impondo:

\[
C=F.
\]

### b)

Para que:

\[
A\to C
\]

permaneça verdadeira com \(C=F\), é necessário:

\[
A=F.
\]

### c)

Pelo mesmo motivo, para:

\[
B\to C
\]

permaneça verdadeira com \(C=F\), precisamos de:

\[
B=F.
\]

### d)

Mas, se:

\[
A=F
\qquad\text{e}\qquad
B=F,
\]

então:

\[
A\lor B=F.
\]

A primeira premissa deixaria de ser verdadeira.

Logo, é impossível manter simultaneamente todas as premissas verdadeiras e \(C\) falsa.

### e)

Não existe contra-avaliação. Portanto:

\[
\boxed{\text{o argumento é válido}.}
\]

### f)

O condicional associado é:

\[
[(A\lor B)\land(A\to C)\land(B\to C)]\to C.
\]

### g)

O antecedente desse condicional é verdadeiro exatamente quando as três premissas do argumento são verdadeiras ao mesmo tempo.

Para falsificá-lo, seria necessário:

\[
(A\lor B)\land(A\to C)\land(B\to C)=V
\]

e:

\[
C=F.
\]

Essa é precisamente a configuração de uma contra-avaliação do argumento original.

## Exercício 5

### a)

**I — Modus ponens**

\[
(p\land q)\to r
\]

\[
p\land q
\]

\[
\therefore r.
\]

**II — Modus tollens**

\[
p\to(q\lor r)
\]

\[
\neg(q\lor r)
\]

\[
\therefore\neg p.
\]

**III — Silogismo hipotético**

\[
(p\lor q)\to r
\]

\[
r\to s
\]

\[
\therefore(p\lor q)\to s.
\]

**IV — Silogismo disjuntivo**

\[
(p\land q)\lor r
\]

\[
\neg r
\]

\[
\therefore p\land q.
\]

**V — Silogismo disjuntivo**

\[
p\lor(q\land r)
\]

\[
\neg p
\]

\[
\therefore q\land r.
\]

### b)

No argumento I:

\[
A=p\land q,
\qquad
B=r.
\]

No argumento II:

\[
A=p,
\qquad
B=q\lor r.
\]

### c)

No argumento III:

\[
A=p\lor q,
\]

\[
B=r,
\]

\[
C=s.
\]

Isso produz exatamente:

\[
A\to B,
\qquad
B\to C,
\qquad
\therefore A\to C.
\]

### d)

As letras \(A\), \(B\) e \(C\) das formas abstratas não precisam representar proposições simples. Elas podem representar fórmulas inteiras.

Por isso, em IV, a alternativa da disjunção pode ser:

\[
p\land q,
\]

e, em V:

\[
q\land r.
\]

### e)

Não.

Uma regra de inferência autoriza obter uma conclusão a partir de premissas.

Já:

\[
A\equiv B
\]

afirma que \(A\) e \(B\) possuem os mesmos valores lógicos em todas as avaliações.

Inferência e equivalência realizam funções diferentes.

## Exercício 6

### a)

De:

\[
\neg p\to(q\lor r)
\]

e:

\[
\neg p,
\]

obtemos:

\[
\boxed{q\lor r}
\]

por **modus ponens**.

A correspondência é:

\[
A=\neg p,
\qquad
B=q\lor r.
\]

### b)

De:

\[
(p\land q)\lor r
\]

e:

\[
\neg r,
\]

obtemos:

\[
\boxed{p\land q}
\]

por **silogismo disjuntivo**.

### c)

De:

\[
(p\lor q)\to r
\]

e:

\[
r\to\neg s,
\]

obtemos:

\[
\boxed{(p\lor q)\to\neg s}
\]

por **silogismo hipotético**.

Correspondência:

\[
A=p\lor q,\qquad B=r,\qquad C=\neg s.
\]

### d)

De:

\[
(p\land q)\to r
\]

e:

\[
\neg r,
\]

obtemos:

\[
\boxed{\neg(p\land q)}
\]

por **modus tollens**.

Aqui:

\[
A=p\land q,
\qquad
B=r.
\]

### e)

Não é possível concluir \(r\) legitimamente em um único passo.

A primeira premissa possui antecedente:

\[
p\land q.
\]

Entretanto, temos apenas:

\[
p.
\]

A disponibilidade de uma parte da conjunção não equivale à disponibilidade da conjunção inteira. Portanto, não podemos aplicar modus ponens.

### f)

Uma resposta possível, utilizando o item a:

De:

\[
\neg p\to(q\lor r)
\]

e:

\[
\neg p,
\]

inferimos:

\[
q\lor r.
\]

Isso significa que a conclusão é legitimamente obtida das premissas por uma regra válida. Não significa que:

\[
\neg p
\]

ou:

\[
\neg p\to(q\lor r)
\]

sejam logicamente equivalentes a:

\[
q\lor r.
\]

Outras explicações corretas utilizando os itens b, c ou d também são aceitáveis.

## Exercício 7

### Parte I

### a)

A Forma I é válida:

\[
A\to B
\]

\[
A
\]

\[
\therefore B.
\]

Trata-se de **modus ponens**.

### b)

A Forma II:

\[
A\to B
\]

\[
B
\]

\[
\therefore A
\]

é a **afirmação do consequente** e é inválida.

### c)

Uma contra-avaliação possível é:

\[
A=F,\qquad B=V.
\]

Então:

\[
A\to B=V,
\]

\[
B=V,
\]

mas:

\[
A=F.
\]

### d)

O condicional:

\[
A\to B
\]

estabelece que \(A\) é suficiente para \(B\). Ele não afirma que \(B\) só pode ocorrer quando \(A\) ocorre.

Por isso, partir da verdade de \(B\) e retornar a \(A\) não é autorizado.

### Parte II

### e)

A Forma III é válida:

\[
A\to B
\]

\[
\neg B
\]

\[
\therefore\neg A.
\]

É um **modus tollens**.

### f)

A Forma IV:

\[
A\to B
\]

\[
\neg A
\]

\[
\therefore\neg B
\]

é uma **negação do antecedente** e é inválida.

### g)

Uma contra-avaliação possível é:

\[
A=F,\qquad B=V.
\]

Logo:

\[
A\to B=V,
\]

\[
\neg A=V,
\]

e:

\[
\neg B=F.
\]

Todas as premissas são verdadeiras, mas a conclusão é falsa.

### h)

A falsidade de \(A\) não impede, em geral, que \(B\) seja verdadeira. O condicional original apenas declara que, quando \(A\) ocorre, \(B\) deve ocorrer.

### Parte III

### i)

Uma formalização adequada é:

\[
A:\quad \text{a senha foi digitada corretamente;}
\]

\[
B:\quad \text{o sistema libera o acesso.}
\]

### j)

A forma é:

\[
A\to B
\]

\[
B
\]

\[
\therefore A.
\]

### k)

É uma **afirmação do consequente**, portanto inválida.

### l)

A premissa:

\[
A\to B
\]

não estabelece que \(A\) seja a única condição capaz de produzir \(B\). Assim, a ocorrência de \(B\) não garante \(A\).

Não é necessário supor concretamente outras formas de acesso; basta reconhecer que o condicional fornecido não exclui outras possibilidades.

## Exercício 8

### I

De:

\[
A\to B
\]

e:

\[
B\to C,
\]

obtemos:

\[
\boxed{A\to C}
\]

por **silogismo hipotético**.

### II

De:

\[
A\lor B
\]

e:

\[
\neg B,
\]

obtemos:

\[
\boxed{A}
\]

por **silogismo disjuntivo**.

### III

De:

\[
(p\land q)\to r
\]

e:

\[
p\land q,
\]

obtemos:

\[
\boxed{r}
\]

por **modus ponens**.

### IV

De:

\[
p\to(q\lor r)
\]

e:

\[
\neg(q\lor r),
\]

obtemos:

\[
\boxed{\neg p}
\]

por **modus tollens**.

### V

Não é possível obter:

\[
\neg B
\]

a partir de:

\[
A\to B
\]

e:

\[
\neg A.
\]

A tentativa realiza uma **negação do antecedente**, forma inválida.

Nenhuma das quatro regras válidas disponíveis autoriza essa conclusão em um único passo.

## Exercício 9

### a)–c)

A cadeia correta é:

**Passo 1**

De:

\[
p\lor q
\]

e:

\[
\neg p,
\]

obtemos:

\[
q
\]

por silogismo disjuntivo.

**Passo 2**

De:

\[
q
\]

e:

\[
q\to r,
\]

obtemos:

\[
r
\]

por modus ponens.

**Passo 3**

De:

\[
r
\]

e:

\[
r\to s,
\]

obtemos:

\[
s
\]

por modus ponens.

| Passo | Afirmação disponível ou obtida | Informações utilizadas | Justificativa |
|---:|---|---|---|
| Premissas | \(p\lor q\); \(\neg p\); \(q\to r\); \(r\to s\) | — | dadas |
| 1 | \(q\) | \(p\lor q\), \(\neg p\) | silogismo disjuntivo |
| 2 | \(r\) | \(q\), \(q\to r\) | modus ponens |
| 3 | \(s\) | \(r\), \(r\to s\) | modus ponens |

### d)

A proposição \(q\) só passa a estar disponível depois de ser obtida no Passo 1.

Depois disso, pode ser utilizada juntamente com:

\[
q\to r
\]

para produzir \(r\).

Da mesma forma, \(r\) só passa a estar disponível depois do Passo 2 e, então, pode ser utilizada com:

\[
r\to s.
\]

### e)

Há uma dependência necessária entre as conclusões intermediárias.

Com as premissas fornecidas, não podemos aplicar modus ponens a:

\[
q\to r
\]

sem antes dispor de \(q\). E não podemos utilizar:

\[
r\to s
\]

para obter \(s\) sem antes dispor de \(r\).

### f)

A primeira linha ilegítima da tentativa é:

\[
r.
\]

### g)

A justificativa indicada corresponde, em abstrato, a um modus ponens válido:

\[
q\to r,
\qquad
q
\qquad
\therefore r.
\]

O problema é que, naquele momento da cadeia, \(q\) ainda não havia sido fornecida nem obtida.

Uma regra válida só pode ser aplicada quando suas premissas estão efetivamente disponíveis.

### h)

A ordem correta é:

1. obter \(q\) de \(p\lor q\) e \(\neg p\);
2. obter \(r\) de \(q\) e \(q\to r\);
3. obter \(s\) de \(r\) e \(r\to s\).

### i)

Saber que uma proposição será obtida posteriormente não a torna disponível antecipadamente. Cada etapa precisa utilizar apenas premissas iniciais ou resultados que já tenham sido legitimamente estabelecidos.

## Exercício 10

### Parte I

### a)

A Abordagem A estabelece que a propriedade funciona nos três valores testados:

\[
n=2,\qquad n=8,\qquad n=20.
\]

### b)

Esses três casos são particulares. Mesmo estando corretos, não mostram por que a propriedade deve valer para **qualquer** inteiro par.

### c)–d)

Uma demonstração possível para a Abordagem B é:

Suponha que \(n\) seja par. Então existe um inteiro \(k\) tal que:

\[
n=2k.
\]

Assim:

\[
n+6
=
2k+6
=
2(k+3).
\]

Como \(k\) é inteiro, \(k+3\) também é inteiro. Logo:

\[
n+6
\]

é par.

### e)

A Abordagem A trabalha com valores escolhidos individualmente.

A Abordagem B utiliza:

\[
n=2k,
\]

que descreve um inteiro par arbitrário. Por isso, o raciocínio não depende de um caso particular.

### Parte II

### f)–g)

Uma resposta possível é:

\[
x=\frac12.
\]

Temos:

\[
x^2
=
\left(\frac12\right)^2
=
\frac14.
\]

Como:

\[
\frac14<\frac12,
\]

a desigualdade:

\[
x^2\geq x
\]

falha nesse caso.

Outros valores corretos são aceitáveis. O critério é escolher um real que satisfaça:

\[
x^2<x.
\]

### h)

A afirmação diz que a propriedade vale para **todo** real. Um único real admissível no qual ela falhe basta para refutá-la.

### i)

Casos favoráveis isolados não garantem uma afirmação universal, porque ainda podem existir casos não testados em que ela falha.

Já um único contraexemplo é suficiente para mostrar que a universal não vale para todos os casos.

## Exercício 11

### a)

Hipótese:

\[
n\text{ é par}.
\]

### b)

Tese:

\[
3n+4\text{ é par}.
\]

### c)–f)

Uma demonstração possível é:

Como \(n\) é par, existe um inteiro \(k\) tal que:

\[
n=2k.
\]

Então:

\[
3n+4
=
3(2k)+4
=
6k+4
=
2(3k+2).
\]

Como \(k\) é inteiro:

\[
3k+2
\]

também é inteiro.

Portanto:

\[
3n+4
\]

é par.

### g)

Nenhum valor particular de \(n\) foi escolhido. O argumento utilizou apenas a forma geral:

\[
n=2k,
\]

válida para qualquer inteiro par.

### h)

Uma redação possível é:

> Suponha que \(n\) seja par. Então existe um inteiro \(k\) tal que \(n=2k\). Assim,
> \[
> 3n+4=3(2k)+4=6k+4=2(3k+2).
> \]
> Como \(3k+2\) é inteiro, \(3n+4\) é par.

Outras redações são aceitáveis desde que partam da hipótese correta, obtenham uma expressão igual a \(2\) vezes um inteiro e concluam explicitamente a tese.

## Exercício 12

### a)

Temos:

\[
A:\quad 5x+2>17
\]

e:

\[
B:\quad x>3.
\]

A afirmação original é:

\[
A\to B.
\]

### b)

A contrapositiva é:

\[
\neg B\to\neg A.
\]

### c)

A negação de:

\[
x>3
\]

é:

\[
x\leq3.
\]

### d)

A negação de:

\[
5x+2>17
\]

é:

\[
5x+2\leq17.
\]

Logo, a contrapositiva é:

\[
x\leq3
\to
5x+2\leq17.
\]

### e)

Uma demonstração possível:

Suponha:

\[
x\leq3.
\]

Multiplicando por \(5\), que é positivo:

\[
5x\leq15.
\]

Somando \(2\) aos dois lados:

\[
5x+2\leq17.
\]

Portanto, a contrapositiva foi demonstrada.

### f)

Como:

\[
A\to B
\equiv
\neg B\to\neg A,
\]

demonstrar a contrapositiva estabelece também o condicional original.

### g)

No **modus tollens**, o condicional:

\[
A\to B
\]

já está disponível como premissa. Com:

\[
\neg B,
\]

inferimos:

\[
\neg A.
\]

Na demonstração por contraposição, ao contrário:

\[
A\to B
\]

é justamente aquilo que ainda queremos estabelecer. Demonstramos então a proposição equivalente:

\[
\neg B\to\neg A.
\]

### h)

Não estamos usando \(A\to B\) para demonstrar a si próprio. A legitimidade do procedimento vem da equivalência lógica entre o condicional e sua contrapositiva.

## Exercício 13

### a)

A tese é:

> Não existem dois números inteiros consecutivos que sejam ambos pares.

### b)

Sua negação é:

> Existem dois números inteiros consecutivos que são ambos pares.

### c)–f)

Assuma, para obter uma contradição, que \(n\) e \(n+1\) sejam ambos pares.

Então existem inteiros \(a\) e \(b\) tais que:

\[
n=2a
\]

e:

\[
n+1=2b.
\]

Substituindo a primeira igualdade na segunda:

\[
2a+1=2b.
\]

Assim:

\[
1=2b-2a
\]

e:

\[
1=2(b-a).
\]

### g)

Como \(a\) e \(b\) são inteiros:

\[
b-a
\]

é inteiro.

A igualdade:

\[
1=2(b-a)
\]

afirmaria que \(1\) é duas vezes um número inteiro. Isso é impossível: não existe inteiro \(c\) tal que:

\[
2c=1.
\]

Essa é a contradição efetiva.

### h)

A incompatibilidade foi consequência da suposição de que os dois inteiros consecutivos eram pares. Como essa suposição conduz a uma impossibilidade, ela deve ser rejeitada.

### i)

Portanto, não existem dois números inteiros consecutivos que sejam ambos pares.

### j)

Não.

“Não consegui continuar” indica apenas que uma tentativa de raciocínio encontrou uma dificuldade. Uma demonstração por contradição exige que a suposição conduza efetivamente a uma incompatibilidade lógica ou matemática.

Outras demonstrações equivalentes são aceitáveis desde que a contradição seja real e decorra da suposição feita.

## Exercício 14

### a)

As possibilidades são exatamente:

\[
x=-2,\qquad x=0,\qquad x=2.
\]

### b)

**Caso 1**

Se:

\[
x=-2,
\]

então:

\[
x^2=4\leq4.
\]

**Caso 2**

Se:

\[
x=0,
\]

então:

\[
x^2=0\leq4.
\]

**Caso 3**

Se:

\[
x=2,
\]

então:

\[
x^2=4\leq4.
\]

### c)

Esses três valores constituem todas as possibilidades admitidas pela hipótese. Como a tese foi estabelecida em cada uma delas, vale para qualquer \(x\) abrangido pela situação.

### d)

Não estamos escolhendo três exemplos dentre muitas possibilidades possíveis. Estamos verificando **todos** os casos permitidos pela hipótese.

É essa cobertura completa que torna o argumento uma demonstração por casos.

### e)

Sim. Os dois casos analisados na tentativa estão corretos.

### f)

Não. A demonstração está incompleta.

### g)

Falta analisar:

\[
x=2.
\]

### h)

Mesmo que cada ramo apresentado esteja correto, uma demonstração por casos precisa cobrir todas as possibilidades admissíveis. Um caso omitido deixa aberta a possibilidade de a tese falhar justamente ali.

### i)

Basta acrescentar:

> **Caso 3:** se \(x=2\), então
> \[
> x^2=4\leq4.
> \]

Agora todas as possibilidades foram verificadas e a demonstração fica completa.

## Exercício 15

### a)

As duas direções são:

\[
x>4\to3x-2>10
\]

e:

\[
3x-2>10\to x>4.
\]

### b)

Uma demonstração possível da primeira direção:

Suponha:

\[
x>4.
\]

Multiplicando por \(3\), número positivo:

\[
3x>12.
\]

Subtraindo \(2\):

\[
3x-2>10.
\]

Logo:

\[
x>4\to3x-2>10.
\]

### c)

Para a segunda direção, suponha:

\[
3x-2>10.
\]

Somando \(2\):

\[
3x>12.
\]

Dividindo por \(3\):

\[
x>4.
\]

Portanto:

\[
3x-2>10\to x>4.
\]

### d)

Multiplicamos e dividimos apenas pelo número positivo \(3\). Por isso, o sentido das desigualdades é preservado.

### e)

Como as duas direções foram demonstradas:

\[
\boxed{x>4\leftrightarrow3x-2>10}.
\]

### f)

Uma bicondicional exige ambas as direções. Demonstrar somente:

\[
x>4\to3x-2>10
\]

não estabelece que:

\[
3x-2>10
\]

também seja suficiente para:

\[
x>4.
\]

### g)

A tentativa apresentada demonstra apenas:

\[
x>4\to3x-2>10.
\]

### h)

Falta demonstrar:

\[
3x-2>10\to x>4.
\]

### i)

Podemos completar:

> Suponha:
> \[
> 3x-2>10.
> \]
> Somando \(2\):
> \[
> 3x>12.
> \]
> Dividindo por \(3\):
> \[
> x>4.
> \]
> Como as duas direções foram estabelecidas,
> \[
> x>4\leftrightarrow3x-2>10.
> \]

Outras redações equivalentes são aceitáveis desde que ambas as direções sejam efetivamente demonstradas.

## Exercício 16

### a)

A tentativa que estabelece legitimamente a tese é:

\[
\boxed{\text{Tentativa I}.}
\]

Ela começa exatamente da hipótese:

\[
n+4\text{ é par}
\]

e conclui:

\[
n\text{ é par}.
\]

### b)

| Tentativa | Ponto de partida | O que efetivamente obtém | Estratégia ou diagnóstico |
|---|---|---|---|
| I | \(n+4\) é par | \(n\) é par | demonstração legítima |
| II | \(n\) é par | \(n+4\) é par | demonstra a direção recíproca |
| III | \(n+4\) é par | utiliza \(n\) par antes de estabelecê-lo | raciocínio circular |
| IV | casos particulares | validade da afirmação nesses casos | não estabelece a generalidade |

### c)

Na Tentativa II, o primeiro problema está já na escolha do ponto de partida: ela assume \(n\) par, quando a hipótese da tese é \(n+4\) par.

Na Tentativa III, o primeiro defeito ocorre em:

> “Como \(n\) é par...”

Nesse momento, \(n\) ser par ainda é precisamente aquilo que deveria ser demonstrado.

Na Tentativa IV, o problema aparece quando os casos particulares corretos são usados para anunciar uma conclusão universal.

### d)

A Tentativa II demonstra corretamente:

\[
n\text{ é par}
\to
n+4\text{ é par}.
\]

Mas a tese solicitada é:

\[
n+4\text{ é par}
\to
n\text{ é par}.
\]

As duas afirmações possuem direções diferentes. Provar a recíproca não substitui a demonstração da direção original.

### e)

Na Tentativa III, a afirmação:

\[
n\text{ é par}
\]

é utilizada antes de ser estabelecida.

A partir dela, escreve-se:

\[
n=2m.
\]

Mas esse passo depende justamente da tese que ainda está em demonstração. Assim, a conclusão é usada como fundamento para si mesma: o raciocínio é circular.

### f)

A Tentativa IV mostra corretamente que a tese funciona nos casos:

\[
n=0,\qquad n=4,\qquad n=10.
\]

Ela não mostra que a tese vale para qualquer inteiro \(n\) cuja soma \(n+4\) seja par.

Casos particulares favoráveis não fornecem, sozinhos, uma justificativa geral.

### g)

Uma reconstrução possível, tomando a Tentativa II como ponto de partida, é abandonar a direção recíproca e começar pela hipótese correta:

Suponha que:

\[
n+4
\]

seja par.

Então existe um inteiro \(k\) tal que:

\[
n+4=2k.
\]

Logo:

\[
n=2k-4
\]

e:

\[
n=2(k-2).
\]

Como \(k-2\) é inteiro, \(n\) é par.

Também seriam aceitáveis reconstruções corretas das Tentativas III ou IV, desde que a tese seja efetivamente estabelecida sem circularidade e sem depender apenas de exemplos particulares.

### h)

Uma versão final concisa possível é:

> Suponha que \(n+4\) seja par. Então existe um inteiro \(k\) tal que:
> \[
> n+4=2k.
> \]
> Assim:
> \[
> n=2k-4=2(k-2).
> \]
> Como \(k-2\) é inteiro, \(n\) é par.

Não é necessário reproduzir literalmente essa redação. Uma demonstração correta deve:

- partir da hipótese adequada;
- utilizar uma informação legitimamente obtida dela;
- chegar à forma de \(2\) vezes um inteiro;
- justificar que esse fator é inteiro;
- concluir que \(n\) é par.

### i)

Durante a descoberta de uma demonstração, é possível testar caminhos, começar pela tese, abandonar tentativas ou perceber posteriormente uma forma mais simples de organizar o raciocínio.

A redação final não precisa narrar essa história. Ela deve reorganizar o argumento numa ordem em que o leitor consiga reconstruir claramente por que cada passagem é legítima.

### j)

A afirmação do estudante é incorreta.

Mostrar que a Tentativa II falha estabelece apenas:

> A Tentativa II não demonstra a tese.

Isso é diferente de estabelecer:

> A tese é falsa.

Uma demonstração defeituosa pode falhar mesmo quando a tese é verdadeira. Para mostrar que uma tese é falsa, seria necessária uma refutação legítima.

Neste caso, a própria Tentativa I demonstra corretamente a tese.
