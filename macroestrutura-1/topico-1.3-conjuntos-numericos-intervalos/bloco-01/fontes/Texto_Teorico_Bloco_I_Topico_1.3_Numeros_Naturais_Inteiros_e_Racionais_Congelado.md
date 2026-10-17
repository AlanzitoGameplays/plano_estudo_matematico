# PARTE I — NÚMEROS NATURAIS E INTEIROS

## O conjunto dos números naturais

Os números utilizados para contar objetos são familiares: um objeto, dois objetos, três objetos, e assim sucessivamente. Quando não existe nenhum objeto a ser contado, a quantidade correspondente é zero.

Esses números constituem o **conjunto dos números naturais**, representado pelo símbolo \(\mathbb N\):

\[
\boxed{\mathbb N=\{0,1,2,3,4,5,\ldots\}.}
\]

A notação entre chaves indica os elementos do conjunto. As reticências mostram que a sequência prossegue indefinidamente, seguindo o mesmo padrão. Assim, \(\mathbb N\) não contém apenas os números escritos na expressão: também contém \(6\), \(7\), \(8\) e todos os demais números naturais.

Neste Plano, adotaremos a convenção de que o zero pertence aos naturais:

\[
0\in\mathbb N.
\]

Algumas obras matemáticas utilizam uma convenção que começa os naturais em \(1\). Ambas são encontradas na literatura; o importante é reconhecer qual delas está sendo utilizada. Aqui, o zero será considerado um número natural.

Os naturais incluem, portanto, o zero e os números de contagem positivos. Todos os seus elementos são números inteiros não negativos: não possuem parte fracionária e não são negativos.

Por exemplo, \(4\in\mathbb N\), mas \(-4\notin\mathbb N\). O primeiro é um número natural; o segundo não pertence ao conjunto definido acima.

## A ampliação aos números inteiros

Os naturais não são suficientes para representar todos os resultados e situações que envolvem números inteiros.

Considere, por exemplo, a subtração \(2-5\). Não existe um número natural que represente seu resultado. Entretanto, podemos expressá-lo pelo número negativo \(-3\):

\[
2-5=-3.
\]

O número \(-3\) não pertence a \(\mathbb N\), mas pode ser utilizado matematicamente da mesma maneira que outros valores inteiros, como em uma temperatura de três graus abaixo de zero.

Para incluir os números negativos sem perder os naturais já conhecidos, consideramos um conjunto mais abrangente: o **conjunto dos números inteiros**, representado por \(\mathbb Z\).

\[
\boxed{
\mathbb Z=\{\ldots,-4,-3,-2,-1,0,1,2,3,4,\ldots\}.
}
\]

Nesse conjunto, distinguimos os inteiros negativos, o zero e os inteiros positivos.

Os inteiros negativos são

\[
\ldots,-4,-3,-2,-1,
\]

enquanto os inteiros positivos são

\[
1,2,3,4,\ldots
\]

O zero não é positivo nem negativo. Ele também é um número inteiro e, pela convenção adotada, pertence aos naturais.

Observe que a ampliação não altera os números anteriores. O número \(3\), por exemplo, continua sendo o mesmo objeto matemático; a diferença é que agora também o reconhecemos como elemento de um conjunto maior.

Assim,

\[
3\in\mathbb N
\qquad\text{e}\qquad
3\in\mathbb Z.
\]

Já o número \(-3\) pertence apenas ao segundo desses conjuntos:

\[
-3\notin\mathbb N,
\qquad
-3\in\mathbb Z.
\]

## A inclusão dos naturais nos inteiros

Comparando as definições, verificamos que todos os números naturais aparecem também no conjunto dos inteiros.

De fato, \(\mathbb N\) contém o zero e os inteiros positivos, e todos esses números pertencem a \(\mathbb Z\). Portanto, qualquer número escolhido em \(\mathbb N\) necessariamente pertencerá a \(\mathbb Z\).

Essa condição estabelece a inclusão:

\[
\boxed{\mathbb N\subseteq\mathbb Z.}
\]

A afirmação não significa que os dois conjuntos sejam iguais. Existem inteiros que não são naturais, como \(-1\), \(-2\) e \(-3\). Significa que **nenhum número natural fica fora do conjunto dos inteiros**.

A passagem de \(\mathbb N\) para \(\mathbb Z\) é, portanto, uma ampliação do domínio numérico: os naturais são preservados, enquanto os inteiros negativos acrescentam novos elementos.

Ainda assim, nem todos os números familiares pertencem a \(\mathbb Z\). O número que representa metade de uma unidade, por exemplo, não é inteiro. Para compreender números dessa natureza, precisamos considerar outro conjunto numérico.

---

# PARTE II — NÚMEROS RACIONAIS E SUAS REPRESENTAÇÕES

## A ampliação aos números racionais

Os números inteiros permitem representar quantidades positivas, negativas e nulas, mas não incluem todos os números que podem surgir de uma divisão.

Considere uma unidade dividida em duas partes iguais. Cada parte corresponde à metade da unidade, representada pela expressão

\[
\frac12.
\]

Esse número não é inteiro. Nenhum elemento de \(\mathbb Z\) representa exatamente a metade de uma unidade. Entretanto, a quantidade está matematicamente determinada: conhecemos a unidade considerada, o número de partes iguais em que foi dividida e a quantidade correspondente a cada parte.

A expressão \(\frac12\) também pode ser interpretada como o quociente de \(1\) por \(2\), isto é, o resultado da divisão de um inteiro por outro.

O mesmo ocorre com números como

\[
\frac34,\qquad \frac53,\qquad -\frac72.
\]

Essas expressões representam números que podem ser obtidos como quocientes de inteiros, embora nem todos os resultados sejam números inteiros.

Para abranger esses números, consideramos o **conjunto dos números racionais**, representado por \(\mathbb Q\).

Um número é chamado de **racional** quando pode ser representado como quociente de dois números inteiros, desde que o segundo seja diferente de zero.

Essa definição é expressa por:

\[
\boxed{
\mathbb Q=
\left\{
\frac pq\;\middle|\;
p,q\in\mathbb Z,\ q\neq0
\right\}.
}
\]

Na expressão, \(p\) representa o numerador e \(q\) representa o denominador. Ambos devem ser números inteiros, mas o denominador não pode ser zero.

A condição \(p,q\in\mathbb Z\) permite que o numerador e o denominador sejam positivos ou negativos. O numerador também pode ser zero. A restrição essencial é:

\[
q\neq0.
\]

Assim, \(\frac23\) e \(-\frac32\) são representações de números racionais. Da mesma forma,

\[
\frac07=0
\]

é uma representação racional válida, pois o denominador é diferente de zero.

O fato de um número racional poder ser escrito como fração não significa que ele precise aparecer dessa maneira em todas as situações. A definição exige a **possibilidade de uma representação como quociente de inteiros**, não uma forma obrigatória de escrita.

### Por que o denominador não pode ser zero?

A restrição \(q\neq0\) decorre do próprio significado da divisão.

Quando escrevemos \(\frac pq\), estamos procurando um número que, multiplicado por \(q\), produza \(p\). Por exemplo,

\[
\frac62=3
\]

porque \(3\cdot2=6\).

Se o denominador fosse zero, essa interpretação deixaria de determinar um quociente.

Considere a expressão \(\frac30\). Para que ela representasse algum número \(x\), precisaríamos ter

\[
0\cdot x=3.
\]

Isso é impossível, pois o produto de zero por qualquer número é zero.

O caso \(\frac00\) também não define um quociente. Como \(0\cdot x=0\) para qualquer número \(x\), não existe um resultado único determinado por essa expressão.

Portanto, **a divisão por zero não está definida**, seja o numerador diferente de zero ou igual a zero.

Essa restrição faz parte da definição dos números racionais e deve ser preservada sempre que uma expressão da forma \(\frac pq\) for utilizada.

## Um número pode possuir diferentes representações

A representação de um número não deve ser confundida com o próprio número.

Considere novamente a metade de uma unidade. Podemos representá-la por

\[
\frac12.
\]

Se a mesma unidade for dividida em quatro partes iguais, duas dessas partes também corresponderão à metade. Logo,

\[
\frac12=\frac24.
\]

As duas expressões são diferentes: possuem numeradores e denominadores distintos. Entretanto, representam exatamente a mesma quantidade e, portanto, o mesmo número racional.

Podemos ainda utilizar a escrita decimal:

\[
\boxed{\frac12=\frac24=0{,}5.}
\]

A expressão \(0{,}5\) indica cinco décimos de uma unidade, quantidade equivalente à sua metade.

Temos, assim, três representações de um único número. A escolha de uma escrita não altera sua identidade matemática.

Isso é especialmente importante na Teoria dos Conjuntos. Considere

\[
A=\left\{\frac12,\frac24,0{,}5\right\}.
\]

Embora existam três expressões entre as chaves, todas indicam o mesmo objeto. Como um conjunto não distingue repetições de um mesmo elemento, temos

\[
A=\left\{\frac12\right\}.
\]

Portanto, \(A\) é um conjunto unitário.

O que determina seus elementos são os números representados, não a quantidade de escritas utilizadas para apresentá-los.

Essa distinção também esclarece por que um número escrito como fração não precisa ser diferente de um número inteiro.

Considere

\[
\frac62=3.
\]

A expressão \(\frac62\) está na forma de um quociente, mas o número que ela representa é o inteiro \(3\).

Consequentemente,

\[
\frac62\in\mathbb Z.
\]

A forma da escrita, isoladamente, não determina o menor conjunto numérico ao qual o número pertence. É necessário considerar o número efetivamente representado.

## Os inteiros também são racionais

A definição de número racional permite estabelecer uma relação importante entre \(\mathbb Z\) e \(\mathbb Q\).

Considere um inteiro qualquer, como \(5\). Podemos escrevê-lo como

\[
5=\frac51.
\]

O numerador \(5\) é inteiro, o denominador \(1\) também é inteiro e não é zero. Portanto, \(5\) satisfaz a definição de número racional.

O mesmo vale para um inteiro negativo:

\[
-4=\frac{-4}{1},
\]

e para o zero:

\[
0=\frac01.
\]

Esses exemplos não representam casos isolados. Para qualquer número inteiro \(n\), temos

\[
n=\frac n1.
\]

Como \(n\in\mathbb Z\), \(1\in\mathbb Z\) e \(1\neq0\), essa representação satisfaz as condições da definição de \(\mathbb Q\).

Logo, todo número inteiro é também um número racional:

\[
\boxed{\mathbb Z\subseteq\mathbb Q.}
\]

Essa inclusão não depende de verificar individualmente todos os inteiros. A justificativa vale para um inteiro arbitrário e, por isso, estabelece uma propriedade geral.

Entretanto, a inclusão inversa não é verdadeira. O número \(\frac12\), por exemplo, é racional, mas não é inteiro. Portanto, existem elementos de \(\mathbb Q\) que não pertencem a \(\mathbb Z\).

O conjunto dos racionais amplia o domínio dos inteiros porque conserva todos eles e incorpora números que não podem ser representados por elementos de \(\mathbb Z\).

## As representações decimais dos racionais

Além da representação como quociente de inteiros, os números racionais podem ser escritos na forma decimal.

A escrita decimal utiliza a vírgula para distinguir a parte inteira das posições correspondentes a décimos, centésimos, milésimos e assim sucessivamente.

Por exemplo,

\[
\frac12=0{,}5
\]

e

\[
\frac34=0{,}75.
\]

Nesses dois casos, a representação decimal possui uma quantidade limitada de algarismos após a vírgula. Dizemos que se trata de uma **representação decimal finita**.

Toda representação decimal finita corresponde a um número racional. Isso pode ser observado, por exemplo, em

\[
0{,}25=\frac{25}{100}.
\]

O número decimal \(0{,}25\) representa vinte e cinco centésimos. Como pode ser escrito como quociente de dois inteiros, satisfaz a definição de racionalidade.

Entretanto, nem todos os números racionais possuem uma representação decimal finita.

Considere o número

\[
\frac13.
\]

Sua representação decimal é

\[
\frac13=0{,}3333\ldots
\]

O algarismo \(3\) continua aparecendo indefinidamente. Não existe uma última casa decimal nessa representação.

Apesar disso, \(\frac13\) continua sendo racional: sua própria escrita como quociente de dois inteiros já satisfaz a definição.

A característica importante dessa expansão decimal não é apenas sua extensão infinita, mas a **repetição regular de seus algarismos**.

O bloco que se repete indefinidamente recebe o nome de *período*. No número \(0{,}3333\ldots\), o período é o algarismo \(3\).

Em outros casos, o período pode conter mais de um algarismo. Por exemplo, na escrita

\[
0{,}12121212\ldots,
\]

o período é formado pelos algarismos \(12\).

Uma representação decimal infinita que repete indefinidamente um mesmo bloco de algarismos, a partir de determinada posição, é chamada de **dízima periódica**.

### Quando o período não começa imediatamente

A repetição não precisa começar na primeira casa decimal.

Considere:

\[
\frac16=0{,}16666\ldots
\]

O primeiro algarismo após a vírgula é \(1\). Depois dele, o algarismo \(6\) se repete indefinidamente.

A representação não é periódica desde sua primeira casa decimal, mas torna-se periódica após esse algarismo inicial. Por isso, dizemos que ela é **eventualmente periódica**.

Uma expansão eventualmente periódica possui uma quantidade finita de algarismos iniciais, após os quais um bloco fixo passa a se repetir indefinidamente. A parte inicial pode inclusive estar ausente, como ocorre em \(0{,}3333\ldots\).

Desse modo, tanto

\[
0{,}3333\ldots
\]

quanto

\[
0{,}16666\ldots
\]

são representações decimais eventualmente periódicas, embora a repetição comece em posições diferentes.

A periodicidade exige mais do que a simples ocorrência repetida de alguns algarismos. É necessário que, a partir de determinada posição, **um mesmo bloco continue se repetindo sem interrupção**.

### A caracterização decimal dos números racionais

Existe uma propriedade matemática que relaciona precisamente a definição dos números racionais às suas representações decimais:

**Os números racionais são exatamente os números que admitem uma representação decimal finita ou infinita eventualmente periódica.**

Isso significa que a relação funciona nas duas direções.

Todo número racional admite uma representação decimal finita ou eventualmente periódica. Reciprocamente, qualquer representação decimal dessas formas determina um número racional.

Podemos resumir essa caracterização:

\[
\boxed{
\begin{gathered}
\text{Representação decimal finita}\\
\text{ou eventualmente periódica}\\
\Updownarrow\\
\text{Número racional}
\end{gathered}
}
\]

A expressão é uma **caracterização matemática dos racionais**, não uma segunda definição arbitrária do conjunto \(\mathbb Q\).

A definição de racionalidade continua sendo a possibilidade de representar um número como quociente de dois inteiros, com denominador não nulo. A caracterização decimal estabelece que essa condição corresponde precisamente às duas formas de representação descritas.

Os exemplos anteriores permitem compreender o significado do resultado, mas não constituem, por si sós, uma demonstração de sua validade para todos os números. A demonstração geral exige propriedades da representação decimal e procedimentos aritméticos que serão desenvolvidos posteriormente.

Por enquanto, a caracterização permite reconhecer uma consequência essencial: **uma representação decimal infinita não é necessariamente irracional**.

As dízimas periódicas também representam números racionais. Portanto, para compreender a racionalidade de um número, não basta observar se sua escrita decimal termina ou prossegue indefinidamente; é necessário considerar se existe uma repetição periódica.

---

# PARTE III — RELAÇÕES ENTRE OS DOMÍNIOS NUMÉRICOS

## A estrutura de inclusão dos conjuntos numéricos

As definições dos números naturais, inteiros e racionais estabelecem uma organização em que cada conjunto está contido no seguinte.

Já sabemos que todo natural é inteiro:

\[
\mathbb N\subseteq\mathbb Z.
\]

Também sabemos que todo inteiro é racional, pois qualquer inteiro \(n\) pode ser escrito como \(\frac n1\):

\[
\mathbb Z\subseteq\mathbb Q.
\]

Reunindo essas relações, obtemos

\[
\mathbb N\subseteq\mathbb Z\subseteq\mathbb Q.
\]

Entretanto, podemos afirmar algo mais preciso. Nenhuma dessas inclusões representa uma igualdade entre os conjuntos envolvidos.

Considere primeiro \(\mathbb N\) e \(\mathbb Z\). O número \(-1\) pertence aos inteiros, mas não pertence aos naturais:

\[
-1\in\mathbb Z,
\qquad
-1\notin\mathbb N.
\]

Portanto, \(\mathbb Z\) possui pelo menos um elemento que não pertence a \(\mathbb N\).

Como todos os naturais pertencem aos inteiros, mas nem todos os inteiros pertencem aos naturais, temos uma **inclusão própria**:

\[
\mathbb N\subsetneq\mathbb Z.
\]

A mesma justificativa pode ser aplicada aos inteiros e aos racionais.

Sabemos que \(\mathbb Z\subseteq\mathbb Q\). Contudo,

\[
\frac12\in\mathbb Q
\]

e

\[
\frac12\notin\mathbb Z.
\]

Logo, \(\mathbb Q\) possui elementos que não pertencem a \(\mathbb Z\), e a inclusão também é própria:

\[
\mathbb Z\subsetneq\mathbb Q.
\]

Combinando as duas relações, estabelecemos a organização fundamental desses conjuntos:

\[
\boxed{
\mathbb N\subsetneq\mathbb Z\subsetneq\mathbb Q.
}
\]

A primeira inclusão mostra que os naturais constituem parte dos inteiros. A segunda mostra que os inteiros constituem parte dos racionais.

Consequentemente, todos os números naturais são também racionais:

\[
\mathbb N\subsetneq\mathbb Q.
\]

Essa organização pode ser representada por três regiões encaixadas: a região dos naturais inteiramente contida na dos inteiros, e esta inteiramente contida na dos racionais. As regiões restantes correspondem aos números acrescentados em cada ampliação, como \(-1\) entre os inteiros não naturais e \(\frac12\) entre os racionais não inteiros.

As inclusões descrevem relações entre os elementos dos conjuntos, não proporções entre suas quantidades.

## Pertencimento simultâneo e classificação numérica

A organização anterior possui uma consequência importante: **um número pode pertencer simultaneamente a vários conjuntos numéricos**.

Considere o número \(2\).

Ele pertence aos naturais, pois aparece entre seus elementos:

\[
2\in\mathbb N.
\]

Como todo natural é inteiro, também temos

\[
2\in\mathbb Z.
\]

E, como todo inteiro é racional,

\[
2\in\mathbb Q.
\]

Portanto, as três afirmações são verdadeiras:

\[
\boxed{
2\in\mathbb N,\qquad
2\in\mathbb Z,\qquad
2\in\mathbb Q.
}
\]

Não existe contradição nessa classificação. As categorias não são mutuamente exclusivas, pois os conjuntos estão relacionados por inclusão.

O número \(-2\), por outro lado, não é natural. Ele pertence aos inteiros e, consequentemente, aos racionais:

\[
-2\notin\mathbb N,
\qquad
-2\in\mathbb Z,
\qquad
-2\in\mathbb Q.
\]

Já o número \(\frac12\) pertence aos racionais, mas não aos inteiros nem aos naturais:

\[
\frac12\notin\mathbb N,
\qquad
\frac12\notin\mathbb Z,
\qquad
\frac12\in\mathbb Q.
\]

Esses três casos permitem visualizar a organização:

| Número | \(\mathbb N\) | \(\mathbb Z\) | \(\mathbb Q\) |
|---|:---:|:---:|:---:|
| \(2\) | Sim | Sim | Sim |
| \(-2\) | Não | Sim | Sim |
| \(\frac12\) | Não | Não | Sim |

A tabela evidencia que pertencer a um conjunto menor garante o pertencimento aos conjuntos maiores que o contêm. A recíproca, entretanto, não é necessariamente verdadeira.

### O menor conjunto que contém um número

A organização também permite diferenciar duas perguntas matemáticas.

A primeira é: **a quais conjuntos numéricos um número pertence?**

A segunda é: **qual é o menor desses conjuntos que contém o número?**

No caso de \(2\), a primeira pergunta possui três respostas: \(\mathbb N\), \(\mathbb Z\) e \(\mathbb Q\).

Para a segunda, a resposta é \(\mathbb N\), pois os naturais constituem o menor dos três conjuntos que contém \(2\).

Para \(-2\), o menor conjunto estudado que o contém é \(\mathbb Z\). Já para \(\frac12\), é \(\mathbb Q\).

Observe que a classificação continua dependendo do número, não de sua aparência.

Considere

\[
\frac42=2.
\]

Embora esteja escrito como fração, esse número pertence a \(\mathbb N\). Portanto, entre os três conjuntos estudados, o menor que o contém é \(\mathbb N\), e não \(\mathbb Q\).

Isso não significa que \(\frac42\) deixe de ser racional. Significa que o número representado por essa expressão também satisfaz a condição de pertencimento a um conjunto menor.

A distinção entre número e representação, construída anteriormente, continua necessária para interpretar corretamente as relações entre os conjuntos numéricos.

## O significado das ampliações numéricas

A estrutura

\[
\mathbb N\subsetneq\mathbb Z\subsetneq\mathbb Q
\]

mostra que os conjuntos estudados não são coleções independentes de números.

Cada conjunto mais abrangente conserva os elementos dos anteriores e acrescenta outros que não pertenciam ao domínio menor.

Nos naturais, encontramos o zero e os números de contagem positivos. Nos inteiros, conservamos esses números e acrescentamos os inteiros negativos. Nos racionais, conservamos todos os inteiros e incorporamos os números que podem ser expressos como quocientes de inteiros, mesmo quando não são inteiros.

As inclusões permitem passar de uma afirmação sobre um conjunto menor para outra sobre o conjunto que o contém. Se sabemos que um número é natural, podemos concluir imediatamente que ele também é inteiro e racional. Entretanto, saber que um número é racional não permite concluir que seja inteiro: seria necessário verificar uma condição adicional.

A classificação numérica depende, assim, das definições dos conjuntos e das relações que existem entre eles. Não depende apenas do símbolo ou da forma utilizada para escrever cada número.

Os racionais constituem um domínio suficientemente amplo para incluir todos os inteiros e muitas quantidades não inteiras. Sua definição, contudo, estabelece uma condição específica: cada elemento deve admitir uma representação como quociente de dois inteiros, com denominador não nulo.

Resta investigar se essa condição abrange todos os números que podem ser representados na reta numérica ou se existem números que não a satisfazem. Essa questão conduzirá à ampliação seguinte dos domínios numéricos.
