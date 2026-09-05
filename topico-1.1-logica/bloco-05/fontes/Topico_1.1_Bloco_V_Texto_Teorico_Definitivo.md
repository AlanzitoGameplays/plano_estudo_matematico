# TÓPICO 1.1 — LÓGICA MATEMÁTICA

# BLOCO V — ARGUMENTOS, VALIDADE E DEMONSTRAÇÃO ELEMENTAR

## Texto Teórico

# Parte I — Argumentos, Inferência e Validade

## 1. Da proposição ao argumento

Considere a seguinte organização:

\[
p\to q
\]

\[
p
\]

\[
\therefore q
\]

As três linhas representam proposições, mas elas não desempenham o mesmo papel. As duas primeiras são tomadas como pontos de partida; a terceira é apresentada como aquilo que deve decorrer delas.

Isso é diferente de simplesmente escrever:

\[
p,\qquad q,\qquad r.
\]

Nessa segunda situação, temos apenas três proposições colocadas lado a lado. Nada foi dito sobre a relação que pretendemos estabelecer entre elas. Na primeira estrutura, ao contrário, existe uma direção no raciocínio: algumas afirmações fornecem a base a partir da qual outra é apresentada como consequência.

As proposições utilizadas como ponto de partida recebem o nome de **premissas**. A proposição que se pretende obter a partir delas é a **conclusão**.

Um **argumento** é, portanto, uma estrutura em que uma ou mais proposições são apresentadas como premissas para sustentar uma conclusão.

Isso não significa que as premissas sejam necessariamente verdadeiras. “Premissa” designa o papel que uma proposição ocupa no argumento, e não seu valor lógico. Uma afirmação falsa também pode ser tomada como premissa; a questão de sua verdade deve ser analisada separadamente.

A passagem das premissas para a conclusão recebe o nome de **inferência**. Inferir significa apresentar uma conclusão como decorrência de certas proposições assumidas como ponto de partida.

Na escrita simbólica, o sinal

\[
\therefore
\]

é utilizado para marcar a conclusão. Pode ser lido como “portanto” ou “logo”.

Assim, uma forma geral de argumento pode ser apresentada como:

\[
P_1
\]

\[
P_2
\]

\[
\vdots
\]

\[
P_n
\]

\[
\therefore C.
\]

As expressões \(P_1,P_2,\ldots,P_n\) representam as premissas, enquanto \(C\) representa a conclusão.

O símbolo \(\therefore\) não funciona como \(\land\), \(\lor\) ou \(\to\). Ele não conecta proposições para formar uma nova proposição. Sua função é apenas indicar, na apresentação do argumento, onde termina o conjunto de premissas e qual afirmação está sendo apresentada como conclusão.

Na linguagem verbal, essa organização pode aparecer sem qualquer notação especial. Palavras como “portanto”, “logo” e “assim” frequentemente introduzem conclusões; expressões como “pois”, “porque” e “dado que” podem introduzir razões ou premissas. O essencial, porém, não está nessas palavras, mas na relação que elas sinalizam.

Também é possível separar o **conteúdo particular** de um argumento de sua **forma**.

Por exemplo, diferentes argumentos concretos podem possuir a mesma organização:

\[
p\to q
\]

\[
p
\]

\[
\therefore q.
\]

Nesse caso, \(p\) e \(q\) podem representar proposições muito diferentes em cada aplicação. O que permanece é a maneira como elas estão relacionadas.

Essa estrutura abstrata é uma **forma de argumento**. Ao estudar sua forma, deixamos em segundo plano o conteúdo particular das proposições e passamos a investigar se a organização inferencial realmente garante a conclusão.

## 2. Verdade, validade e solidez

Uma proposição pode ser verdadeira ou falsa. Mas essa classificação não resolve, por si só, a questão central de um argumento.

Considere a forma:

\[
p\lor q
\]

\[
\therefore p.
\]

Suponha, em determinada avaliação, que:

\[
p=V
\qquad\text{e}\qquad
q=V.
\]

Nesse caso, a premissa \(p\lor q\) é verdadeira e a conclusão \(p\) também é verdadeira.

Ainda assim, isso não mostra que a conclusão seja garantida pela premissa.

Basta considerar outra avaliação:

\[
p=F
\qquad\text{e}\qquad
q=V.
\]

Agora,

\[
p\lor q=V,
\]

mas:

\[
p=F.
\]

A premissa continua verdadeira enquanto a conclusão se torna falsa.

Portanto, o fato de uma conclusão ser verdadeira em determinado caso não basta para estabelecer a qualidade da inferência que levou até ela.

É possível chegar a uma conclusão verdadeira por uma estrutura que não a garante.

Essa diferença separa dois níveis:

- **verdade e falsidade** são atribuídas às proposições;
- **validade e invalidade** são atribuídas aos argumentos.

Um argumento é **válido** quando não existe uma situação em que todas as suas premissas sejam verdadeiras e sua conclusão seja falsa.

Equivalentemente, podemos dizer que, num argumento válido, a verdade simultânea das premissas garante a verdade da conclusão.

A palavra “garante” é decisiva.

Validade não significa apenas que premissas e conclusão podem ser verdadeiras ao mesmo tempo. Significa que, sempre que todas as premissas forem verdadeiras, a conclusão não poderá ser falsa.

Por isso, uma conclusão verdadeira não implica, por si só, que o argumento seja válido.

Uma conclusão pode ser verdadeira independentemente da qualidade do raciocínio usado para alcançá-la.

Também ocorre a situação inversa: uma premissa falsa não torna automaticamente um argumento inválido.

Considere novamente:

\[
p\to q
\]

\[
p
\]

\[
\therefore q.
\]

Suponha uma avaliação em que:

\[
p=F
\qquad\text{e}\qquad
q=F.
\]

Nesse caso, a segunda premissa \(p\) é falsa, e a conclusão \(q\) também é falsa. Isso, por si só, não constitui uma falha da forma argumentativa.

A pergunta relevante não é:

> Existe alguma situação em que uma premissa é falsa?

Nem:

> Existe alguma situação em que a conclusão é falsa?

A pergunta é:

> Existe alguma situação em que **todas as premissas são verdadeiras e a conclusão é falsa**?

Para a forma acima, não.

Se \(p\) for verdadeira e \(p\to q\) também for verdadeira, então \(q\) não poderá ser falsa. A própria condição de verdade do condicional impede essa combinação.

Assim, a validade não afirma que as premissas são verdadeiras. Ela estabelece o que necessariamente ocorreria com a conclusão **caso todas as premissas fossem verdadeiras**.

Essa distinção permite introduzir uma exigência adicional.

Um argumento é chamado de **sólido** quando:

- é válido;
- e suas premissas são verdadeiras.

Assim,

\[
\text{solidez}
=
\text{validade}
+
\text{premissas verdadeiras}.
\]

A validade fornece a garantia inferencial. A verdade das premissas garante que estamos efetivamente na situação em que essa garantia pode ser aplicada.

Se todas as premissas de um argumento sólido são verdadeiras e sua estrutura não permite premissas verdadeiras com conclusão falsa, então sua conclusão também deve ser verdadeira.

Portanto, verdade, validade e solidez não são três palavras para a mesma coisa.

A verdade diz respeito ao que uma proposição afirma. A validade diz respeito à relação entre premissas e conclusão. A solidez reúne uma relação inferencial válida com pontos de partida verdadeiros.

## 3. Contra-avaliação e critério de validade

A definição de validade identifica uma configuração especialmente importante:

\[
\text{todas as premissas verdadeiras}
\]

e:

\[
\text{conclusão falsa}.
\]

Se conseguirmos produzir uma situação desse tipo, teremos mostrado que as premissas não garantem a conclusão.

Uma atribuição de valores lógicos que torna todas as premissas verdadeiras e a conclusão falsa recebe o nome de **contra-avaliação**.

Retome:

\[
p\lor q
\]

\[
\therefore p.
\]

Escolha:

\[
p=F
\qquad\text{e}\qquad
q=V.
\]

Temos:

\[
p\lor q=V,
\]

enquanto:

\[
p=F.
\]

Logo, essa avaliação produz exatamente a configuração:

\[
\text{premissa verdadeira}
+
\text{conclusão falsa}.
\]

Ela é uma contra-avaliação.

Portanto, o argumento é inválido.

Uma única contra-avaliação é suficiente.

Isso ocorre porque a validade expressa uma garantia geral: **não deve existir** uma situação em que todas as premissas sejam verdadeiras e a conclusão falsa. Encontrar uma única situação desse tipo basta para quebrar essa garantia.

O raciocínio é semelhante ao papel desempenhado por um contraexemplo diante de uma afirmação universal: quando se alega que determinado caso proibido nunca ocorre, uma ocorrência concreta é suficiente para refutar a alegação.

O contrário, porém, não funciona da mesma forma.

Considere novamente o mesmo argumento, mas escolha:

\[
p=V
\qquad\text{e}\qquad
q=F.
\]

Temos:

\[
p\lor q=V
\]

e:

\[
p=V.
\]

Nessa avaliação, a premissa é verdadeira e a conclusão também.

Isso é perfeitamente compatível com a possibilidade de o argumento ser válido, mas essa única avaliação não estabelece sua validade. Já encontramos outra avaliação em que a premissa é verdadeira e a conclusão falsa.

Casos favoráveis isolados não demonstram uma garantia geral.

Também não devemos usar avaliações com premissas falsas para refutar validade.

Se alguma premissa é falsa, então a condição específica investigada pela definição de validade — **todas as premissas verdadeiras** — nem sequer foi satisfeita.

### Visual de HTML

**Função conceitual:** organizar as situações relevantes na análise de validade e destacar a única configuração que constitui uma contra-avaliação.

**Tipo:** tabela comparativa em HTML/CSS.

**Conteúdo exato:**

| Situação das premissas | Conclusão | O que isso informa? |
|---|---|---|
| todas verdadeiras | verdadeira | compatível com validade, mas não a estabelece isoladamente |
| alguma premissa falsa | verdadeira ou falsa | não decide a validade |
| todas verdadeiras | falsa | contra-avaliação: o argumento é inválido |

**Construção:** três colunas. A leitura deve conduzir da situação das premissas ao valor da conclusão e, por fim, ao significado lógico daquela configuração. A última linha deve possuir maior destaque estrutural.

**Ênfase:** destacar a combinação **todas as premissas verdadeiras + conclusão falsa** como o único caso que refuta validade. O destaque deve utilizar hierarquia, peso tipográfico e tratamento discreto de fundo, sem depender apenas de cor.

**Restrições de fidelidade:** não sugerir que uma avaliação com premissas verdadeiras e conclusão verdadeira prova validade. Não sugerir que uma premissa falsa torna um argumento inválido. Não transformar a comparação em tabela-verdade completa. Não antecipar formas nomeadas de inferência. Não utilizar SVG.

**Implementação preferencial:** HTML/CSS.

Uma forma válida pode ser contrastada com o exemplo anterior por meio de uma estrutura simples:

\[
p\land q
\]

\[
\therefore p.
\]

Para que a premissa \(p\land q\) seja verdadeira, tanto \(p\) quanto \(q\) precisam ser verdadeiras.

Assim, sempre que a premissa for verdadeira,

\[
p=V.
\]

Não existe avaliação em que:

\[
p\land q=V
\]

e, ao mesmo tempo,

\[
p=F.
\]

A contra-avaliação necessária para mostrar invalidade é impossível. Portanto, o argumento é válido.

Uma tabela-verdade pode ser utilizada para realizar esse tipo de análise de maneira sistemática. Nesse caso, não precisamos tratar todas as linhas como igualmente importantes. Para investigar validade, dirigimos a atenção especialmente às linhas em que **todas as premissas são verdadeiras**.

Se alguma dessas linhas apresentar conclusão falsa, encontramos uma contra-avaliação e o argumento é inválido.

Se nenhuma linha com todas as premissas verdadeiras apresentar conclusão falsa, a forma é válida.

Há ainda uma maneira de relacionar esse critério à estrutura do condicional.

Considere um argumento geral:

\[
P_1
\]

\[
P_2
\]

\[
\vdots
\]

\[
P_n
\]

\[
\therefore C.
\]

As premissas podem ser reunidas por conjunção:

\[
P_1\land P_2\land\cdots\land P_n.
\]

Podemos então formar:

\[
(P_1\land P_2\land\cdots\land P_n)\to C.
\]

O antecedente desse condicional é verdadeiro exatamente quando **todas as premissas são verdadeiras ao mesmo tempo**.

O consequente é a conclusão \(C\).

Para que esse condicional seja falso, precisamos precisamente da situação:

\[
P_1\land P_2\land\cdots\land P_n=V
\]

e:

\[
C=F.
\]

Mas isso significa:

\[
\text{todas as premissas verdadeiras}
+
\text{conclusão falsa}.
\]

É exatamente a configuração que torna um argumento inválido.

Assim, dizer que

\[
P_1,P_2,\ldots,P_n\therefore C
\]

é válido equivale, neste nível de análise, a dizer que não existe avaliação capaz de falsificar:

\[
(P_1\land P_2\land\cdots\land P_n)\to C.
\]

A validade não acrescenta uma nova espécie de verdade às proposições. Ela expressa uma garantia sobre a passagem das premissas para a conclusão: sempre que os pontos de partida forem simultaneamente verdadeiros, a conclusão não poderá falhar.

# Parte II — Formas Fundamentais de Inferência

## 1. Da validade à forma inferencial

Uma forma de argumento não depende do assunto particular das proposições que a preenchem. Quando escrevemos, por exemplo,

\[
A\to B,
\]

as letras \(A\) e \(B\) podem representar proposições simples ou fórmulas inteiras. O que permanece constante é a maneira como essas expressões estão organizadas.

Isso permite aproveitar uma consequência importante da validade. Se determinada forma não admite nenhuma contra-avaliação — isto é, se sua própria estrutura impede que todas as premissas sejam verdadeiras e a conclusão falsa —, essa garantia não precisa ser reconstruída desde o início toda vez que a mesma organização reaparece com outro conteúdo.

Uma forma válida utilizada dessa maneira recebe o nome de **regra de inferência**.

Uma regra de inferência é, portanto, uma forma válida de argumento que pode servir como padrão para obter uma conclusão a partir de determinadas premissas.

A palavra “regra” não indica uma convenção arbitrária. Não estamos simplesmente autorizando, por escolha, determinada passagem simbólica. A conclusão pode ser inferida porque a forma já possui a garantia exigida pela validade.

Se uma regra possui a estrutura:

\[
A,\qquad B
\]

\[
\therefore C,
\]

a possibilidade de substituir \(A\), \(B\) e \(C\) por proposições concretas não altera essa relação, desde que a estrutura seja preservada. É por isso que uma mesma forma pode participar de raciocínios sobre objetos matemáticos muito diferentes.

Essa função também distingue uma regra de inferência de uma equivalência lógica.

Quando escrevemos:

\[
A\equiv B,
\]

afirmamos que \(A\) e \(B\) possuem os mesmos valores lógicos em todas as avaliações.

Uma inferência realiza outro trabalho. Se determinadas premissas estão disponíveis, uma conclusão fica autorizada por sua relação com elas.

Assim, de:

\[
A\to B
\]

e:

\[
A,
\]

podemos obter \(B\). Isso não significa, porém, que

\[
(A\to B)\land A
\]

seja logicamente equivalente a \(B\). Equivalência compara fórmulas; inferência estabelece uma passagem legítima das premissas para a conclusão.

Para compreender por que uma regra é válida, continua valendo a mesma pergunta:

> Se todas as premissas forem verdadeiras, a conclusão poderia ser falsa?

Nas formas fundamentais a seguir, a própria estrutura dos conectivos torna a resposta perceptível sem que seja necessário reconstruir uma tabela-verdade completa para cada caso.

## 2. Modus ponens e modus tollens

Considere:

\[
A\to B
\]

\[
A
\]

\[
\therefore B.
\]

A primeira premissa estabelece uma direção: quando \(A\) ocorre, \(B\) deve ocorrer. A segunda informa que justamente \(A\) ocorre. A condição suficiente estabelecida pelo condicional foi satisfeita; portanto, \(B\) é garantida.

Essa forma recebe tradicionalmente o nome de **modus ponens**:

\[
A\to B
\]

\[
A
\]

\[
\therefore B.
\]

Sua validade pode ser percebida diretamente pela tentativa de construir uma contra-avaliação.

Suponha que as duas premissas sejam verdadeiras. Teríamos:

\[
A\to B=V
\]

e:

\[
A=V.
\]

Para que a conclusão fosse falsa, precisaríamos ainda de:

\[
B=F.
\]

Mas isso produziria:

\[
A=V
\qquad\text{e}\qquad
B=F,
\]

exatamente a combinação que torna \(A\to B\) falso. A primeira premissa deixaria de ser verdadeira.

Portanto, não existe avaliação em que as duas premissas do modus ponens sejam verdadeiras e sua conclusão falsa.

O modus ponens não cria uma nova direção para o condicional. Ele apenas utiliza a direção que já foi estabelecida:

\[
A\to B.
\]

Se \(A\) é suficiente para \(B\) e \(A\) efetivamente ocorre, então \(B\) deve ocorrer.

Há, porém, outra maneira legítima de utilizar a mesma relação condicional.

Considere:

\[
A\to B
\]

\[
\neg B
\]

\[
\therefore \neg A.
\]

Se \(A\) fosse verdadeira, a primeira premissa exigiria \(B\). Mas a segunda premissa afirma que \(B\) é falsa. Logo, \(A\) não pode ser verdadeira.

Essa forma recebe o nome de **modus tollens**:

\[
A\to B
\]

\[
\neg B
\]

\[
\therefore\neg A.
\]

Sua estrutura coincide com a direção já expressa pela contrapositiva:

\[
A\to B
\equiv
\neg B\to\neg A.
\]

A segunda premissa fornece precisamente:

\[
\neg B,
\]

e a contrapositiva permite concluir:

\[
\neg A.
\]

A mesma relação pode ser compreendida em termos de necessidade. Se:

\[
A\to B,
\]

então \(B\) é condição necessária para \(A\). Se \(B\) não ocorre, também não pode ocorrer aquilo que dependia necessariamente dela.

Podemos ainda testar semanticamente a forma. Se \(A\to B\) fosse verdadeira e \(\neg B\) também fosse verdadeira, então \(B=F\). Caso \(A\) fosse verdadeira, teríamos novamente:

\[
A=V,\qquad B=F,
\]

o que falsificaria o condicional.

Por isso, com as duas premissas verdadeiras, \(\neg A\) não pode ser falsa.

Modus ponens e modus tollens exploram, assim, duas direções legitimamente disponíveis a partir de um condicional. A primeira utiliza a presença do antecedente para obter o consequente; a segunda utiliza a negação do consequente para obter a negação do antecedente, de acordo com a contrapositiva.

## 3. Silogismo hipotético e silogismo disjuntivo

Uma relação condicional também pode participar de um encadeamento.

Considere:

\[
A\to B
\]

e:

\[
B\to C.
\]

A primeira premissa estabelece que \(A\) conduz a \(B\). A segunda estabelece que \(B\) conduz a \(C\).

Se \(A\) ocorrer, então \(B\) deverá ocorrer; e, ocorrendo \(B\), \(C\) também deverá ocorrer. Portanto, a direção inicial pode ser prolongada:

\[
A\to C.
\]

Temos então:

\[
A\to B
\]

\[
B\to C
\]

\[
\therefore A\to C.
\]

Essa forma recebe o nome de **silogismo hipotético**.

Sua validade pode ser compreendida procurando a situação que tornaria sua conclusão falsa. Para que:

\[
A\to C
\]

fosse falsa, precisaríamos de:

\[
A=V
\]

e:

\[
C=F.
\]

Mas, com \(A=V\) e \(A\to B=V\), somos obrigados a ter:

\[
B=V.
\]

Com \(B=V\) e \(B\to C=V\), somos então obrigados a ter:

\[
C=V.
\]

Isso contradiz a tentativa de manter \(C=F\). Logo, não é possível tornar simultaneamente verdadeiras as duas premissas e falsa a conclusão.

A importância da forma está na passagem intermediária. A proposição \(B\) ocupa o ponto em que uma consequência de \(A\) se torna, por sua vez, condição suficiente para \(C\). Assim, duas direções compatíveis podem formar uma direção mais longa.

Uma estrutura diferente aparece quando a premissa principal é uma disjunção:

\[
A\lor B.
\]

Essa proposição exige que pelo menos uma das alternativas seja verdadeira.

Suponha agora que também saibamos:

\[
\neg A.
\]

A possibilidade representada por \(A\) foi eliminada. Como \(A\lor B\) continua verdadeira, \(B\) não pode ser falsa também. Portanto:

\[
B.
\]

A forma completa é:

\[
A\lor B
\]

\[
\neg A
\]

\[
\therefore B.
\]

Ela recebe o nome de **silogismo disjuntivo**.

Sua validade decorre diretamente da exigência imposta pela disjunção. Se \(A\lor B\) é verdadeira e \(A\) é falsa, então admitir também \(B=F\) tornaria ambas as alternativas falsas e, consequentemente, falsificaria a primeira premissa.

Logo, \(B\) precisa ser verdadeira.

A mesma estrutura pode atuar sobre a outra alternativa:

\[
A\lor B
\]

\[
\neg B
\]

\[
\therefore A.
\]

Não se trata de outra regra. O princípio é o mesmo: uma disjunção verdadeira permanece com apenas uma alternativa disponível depois que a outra é excluída.

## 4. Formas inválidas próximas

A semelhança entre formas simbólicas não garante que elas possuam a mesma validade.

Considere novamente o condicional:

\[
A\to B.
\]

Sabemos que \(A\) é suficiente para \(B\). Isso autoriza concluir \(B\) quando \(A\) é dada como premissa. Mas não autoriza percorrer essa relação no sentido contrário apenas porque \(B\) ocorreu.

Considere:

\[
A\to B
\]

\[
B
\]

\[
\therefore A.
\]

Essa forma recebe o nome de **afirmação do consequente**.

O problema está na direção da inferência. De \(A\to B\), não sabemos que \(B\) só pode ocorrer quando \(A\) ocorre. O condicional estabelece \(A\) como condição suficiente para \(B\), mas não estabelece \(A\) como condição necessária.

Concluir \(A\) a partir de \(B\) exigiria, em geral, uma direção como:

\[
B\to A,
\]

isto é, a recíproca do condicional original.

A invalidade pode ser confirmada por uma contra-avaliação simples.

Tome:

\[
A=F
\]

e:

\[
B=V.
\]

Nesse caso:

\[
A\to B=V,
\]

pois um antecedente falso e um consequente verdadeiro não falsificam o condicional.

A segunda premissa também é verdadeira:

\[
B=V.
\]

Mas a conclusão é falsa:

\[
A=F.
\]

Portanto:

\[
A\to B=V,
\qquad
B=V,
\qquad
A=F.
\]

Todas as premissas são verdadeiras e a conclusão é falsa. A forma é inválida.

Uma distorção semelhante ocorre quando partimos da falsidade do antecedente:

\[
A\to B
\]

\[
\neg A
\]

\[
\therefore\neg B.
\]

Essa forma recebe o nome de **negação do antecedente**.

Se \(A\) é suficiente para \(B\), a ausência de \(A\) não estabelece que \(B\) seja impossível. \(B\) pode ocorrer sem que \(A\) tenha ocorrido.

O condicional original não fornece a direção:

\[
\neg A\to\neg B.
\]

A mesma avaliação anterior revela a falha:

\[
A=F,
\qquad
B=V.
\]

Temos:

\[
A\to B=V,
\]

e, como \(A=F\),

\[
\neg A=V.
\]

Mas, como \(B=V\),

\[
\neg B=F.
\]

Portanto:

\[
A\to B=V,
\qquad
\neg A=V,
\qquad
\neg B=F.
\]

Novamente, as premissas são verdadeiras e a conclusão falsa.

A mesma contra-avaliação expõe, portanto, o defeito das duas formas:

\[
A=F,\qquad B=V.
\]

Ela mostra simultaneamente que \(B\) pode ser verdadeira sem \(A\) ser verdadeira e que \(B\) pode permanecer verdadeira mesmo quando \(A\) é falsa.

### Visual de HTML

**Função conceitual:** tornar visíveis as pequenas diferenças estruturais que separam inferências válidas de formas inválidas próximas, destacando a direção realmente autorizada pelo condicional.

**Tipo:** duas comparações paralelas em HTML/CSS.

**Conteúdo exato:**

**Par 1**

| Forma válida | Forma inválida |
|---|---|
| **Modus ponens** | **Afirmação do consequente** |
| \(A\to B\) | \(A\to B\) |
| \(A\) | \(B\) |
| \(\therefore B\) | \(\therefore A\) |

**Par 2**

| Forma válida | Forma inválida |
|---|---|
| **Modus tollens** | **Negação do antecedente** |
| \(A\to B\) | \(A\to B\) |
| \(\neg B\) | \(\neg A\) |
| \(\therefore\neg A\) | \(\therefore\neg B\) |

**Construção:** apresentar os dois pares em blocos comparativos separados verticalmente. Dentro de cada par, forma válida e forma inválida devem aparecer lado a lado, com as três linhas simbólicas alinhadas para que a diferença entre a segunda premissa e a conclusão seja imediatamente perceptível.

**Ênfase:** o contraste deve ser estrutural, não apenas cromático. No primeiro par, evidenciar que afirmar o antecedente permite seguir para o consequente, enquanto afirmar o consequente não autoriza retornar ao antecedente. No segundo, evidenciar que negar o consequente permite chegar à negação do antecedente, enquanto negar o antecedente não autoriza negar o consequente.

**Restrições de fidelidade:** não transformar o visual em catálogo geral de falácias. Não utilizar vermelho e verde como único código de validade. Não acrescentar outras regras, tabelas-verdade ou métodos de demonstração. Não utilizar SVG.

**Implementação preferencial:** HTML/CSS.

A diferença entre as quatro formas pode ser condensada pela direção já estabelecida em:

\[
A\to B.
\]

A partir dela, quando \(A\) é verdadeira, podemos concluir \(B\); e, pela contrapositiva, quando \(B\) é falsa, podemos concluir \(\neg A\). Em geral, porém, a verdade de \(B\) não autoriza concluir \(A\), assim como a falsidade de \(A\) não autoriza concluir \(\neg B\).

A validade depende da direção efetivamente estabelecida, não da simples presença dos mesmos símbolos em posições semelhantes.

## 5. Encadeamento de inferências

Uma inferência válida não precisa encerrar um raciocínio. Sua conclusão pode fornecer informação para uma nova etapa.

Considere:

\[
p\to q
\]

\[
q\to r
\]

\[
p.
\]

Das premissas:

\[
p\to q
\]

e:

\[
p,
\]

obtemos:

\[
q.
\]

Esse \(q\) não foi acrescentado ao raciocínio por suposição. Ele foi legitimamente obtido das informações já disponíveis.

Agora podemos utilizá-lo juntamente com:

\[
q\to r.
\]

Temos então:

\[
q\to r
\]

\[
q
\]

\[
\therefore r.
\]

Assim, a cadeia pode ser organizada como:

\[
p\to q,
\qquad
q\to r,
\qquad
p
\]

\[
\therefore q
\]

\[
\therefore r.
\]

A conclusão intermediária \(q\) ocupa dois papéis em momentos diferentes. Primeiro, é aquilo que obtemos a partir de \(p\to q\) e \(p\). Depois de legitimamente estabelecida, passa a funcionar como premissa para a inferência seguinte.

O mesmo raciocínio pode ser organizado por outra sequência de passos. Das duas primeiras condicionais,

\[
p\to q
\]

e:

\[
q\to r,
\]

podemos obter:

\[
p\to r.
\]

Combinando esse resultado com:

\[
p,
\]

chegamos novamente a:

\[
r.
\]

As duas organizações utilizam formas válidas e chegam à mesma conclusão, embora distribuam os passos de maneira diferente.

O ponto decisivo de um encadeamento não está em fazer a conclusão final parecer plausível. Cada passagem precisa conservar a garantia inferencial.

Se uma expressão intermediária é usada como premissa de uma etapa posterior, deve haver uma razão legítima para que ela esteja disponível. Caso um passo seja inserido sem decorrer das informações anteriores, o restante da cadeia pode até terminar numa proposição verdadeira, mas isso não corrige a falha ocorrida no caminho.

Uma inferência válida preserva a verdade neste sentido: quando suas premissas são todas verdadeiras, sua conclusão também precisa ser verdadeira. Ao encadear inferências válidas, essa garantia pode passar de uma etapa à seguinte, desde que cada nova conclusão seja realmente obtida antes de ser utilizada como ponto de partida para o próximo passo.

# Parte III — Demonstração Matemática Elementar

## 1. Da inferência à demonstração

Uma conclusão obtida legitimamente pode tornar-se ponto de partida para uma nova inferência. Quando esse processo se prolonga, já não temos apenas uma passagem isolada entre premissas e conclusão, mas uma cadeia na qual cada afirmação obtida depende das anteriores.

Essa cadeia, porém, pode ser organizada em torno de uma finalidade mais precisa. Em Matemática, muitas vezes existe uma afirmação determinada que queremos estabelecer. Essa afirmação desempenha o papel de **tese**.

As informações das quais partimos podem ter origens diferentes. Algumas são assumidas especificamente no problema; outras decorrem de definições, propriedades já estabelecidas ou resultados anteriormente demonstrados. O que importa é que estejam legitimamente disponíveis antes de serem utilizadas.

Considere uma afirmação com estrutura condicional:

\[
A\to B.
\]

Quando queremos estabelecê-la, \(A\) pode desempenhar o papel de **hipótese** e \(B\), o de **tese**. A hipótese fornece a condição sob a qual precisamos justificar a conclusão expressa pela tese.

Essa linguagem é especialmente transparente em afirmações condicionais, mas a ideia de tese é mais ampla: é aquilo que o raciocínio pretende estabelecer.

Uma **demonstração matemática** é um argumento que estabelece uma tese por meio de uma sequência de passos logicamente justificados a partir de informações legitimamente admitidas.

A demonstração não se reduz, portanto, a chegar a uma afirmação verdadeira. O caminho que liga os pontos de partida à tese faz parte do que precisa ser estabelecido.

Por essa razão, uma sucessão de fórmulas não constitui automaticamente uma demonstração. Considere, de maneira esquemática:

\[
A
\]

\[
D
\]

\[
E
\]

\[
B.
\]

Mesmo que \(A\) seja uma hipótese legítima e \(B\) seja exatamente a tese desejada, ainda falta saber por que \(D\) decorre de \(A\), por que \(E\) decorre do que já foi obtido e por que \(B\) pode finalmente ser concluída.

Uma passagem pode ser sustentada por uma definição, por uma propriedade conhecida, por uma equivalência, por uma inferência válida ou por outro resultado já estabelecido. Não é necessário reconstruir toda a Matemática utilizada a cada demonstração, mas deve ser possível recuperar a razão dos passos relevantes.

Esse aspecto também separa **testar uma afirmação** de **demonstrá-la**.

Suponha que determinada proposição afirme que uma propriedade vale para todos os valores admissíveis. Podemos experimentar um primeiro caso e obter sucesso. Depois um segundo, um terceiro, um centésimo. Esses resultados podem aumentar nossa confiança, revelar um padrão ou ajudar a descobrir uma demonstração, mas continuam sendo casos particulares.

A exigência universal não é:

> a propriedade funcionou muitas vezes.

Ela é:

> a propriedade vale para todos os casos abrangidos pela afirmação.

Por isso, exemplos favoráveis podem orientar uma investigação sem substituir a razão geral necessária para estabelecer a tese.

Há uma assimetria importante. Para refutar uma afirmação universal, um único contraexemplo pode ser suficiente. Para demonstrá-la, porém, acumular exemplos favoráveis não produz o mesmo efeito. Demonstrar e refutar são tarefas logicamente diferentes.

Essa distinção revela por que toda demonstração possui uma estrutura argumentativa, mas nem todo argumento apresentado constitui uma demonstração matemática. Uma demonstração precisa efetivamente estabelecer sua tese a partir de fundamentos legítimos, preservando a justificação ao longo do raciocínio.

## 2. Demonstração direta

Considere que a tese a estabelecer seja:

\[
A\to B.
\]

O condicional não exige que \(A\) seja verdadeira em todas as situações. Ele estabelece uma relação: nos casos em que \(A\) for verdadeira, \(B\) também deverá ser.

Isso indica uma maneira natural de organizar a demonstração.

Podemos começar supondo:

\[
A.
\]

A partir dessa hipótese, procuramos obter:

\[
B.
\]

A estrutura conceitual é:

\[
A
\]

\[
\text{passos justificados}
\]

\[
B.
\]

Quando conseguimos construir essa passagem para um caso arbitrário que satisfaz a hipótese, estabelecemos que a presença de \(A\) obriga a presença de \(B\). É isso que a proposição \(A\to B\) afirma.

A expressão “suponha \(A\)” merece atenção. Ela não significa que estamos declarando \(A\) verdadeira universalmente, nem que estamos concedendo gratuitamente aquilo que deveríamos demonstrar.

Estamos examinando justamente a situação relevante para o condicional: **um caso no qual o antecedente é verdadeiro**.

Se conseguimos mostrar que, sob essa condição, \(B\) necessariamente segue, então estabelecemos a direção pretendida.

Essa maneira de proceder recebe o nome de **demonstração direta**. Ela começa da hipótese na forma em que foi apresentada e procura alcançar a tese por uma sequência justificável.

Um exemplo elementar permite observar essa estrutura sem acrescentar muita teoria externa.

Dizemos que um número inteiro \(n\) é **par** quando existe um número inteiro \(k\) tal que:

\[
n=2k.
\]

Considere a afirmação:

> Se \(n\) é par, então \(n+2\) é par.

A hipótese é:

\[
n\text{ é par}.
\]

Pela própria definição, isso significa que existe um inteiro \(k\) para o qual:

\[
n=2k.
\]

Somando \(2\) aos dois lados, obtemos:

\[
n+2=2k+2.
\]

Colocando \(2\) em evidência:

\[
n+2=2(k+1).
\]

Como \(k\) é inteiro, \(k+1\) também é inteiro. Portanto, \(n+2\) possui a forma \(2\) vezes um inteiro.

Logo,

\[
n+2
\]

é par.

A demonstração não depende de testar \(n=2\), depois \(n=4\), depois \(n=6\). Ela parte daquilo que caracteriza **qualquer** inteiro par:

\[
n=2k,
\]

e preserva essa estrutura até obter a forma necessária para a tese.

É isso que produz generalidade.

A demonstração é chamada de direta não porque seja necessariamente curta nem porque seu caminho seja sempre óbvio. O nome descreve principalmente sua orientação: começamos da hipótese e avançamos até aquilo que desejamos estabelecer.

## 3. Demonstração por contraposição

Nem sempre a informação fornecida pela hipótese é a forma mais conveniente de iniciar o raciocínio.

Considere novamente uma tese condicional:

\[
A\to B.
\]

Temos a equivalência:

\[
A\to B
\equiv
\neg B\to\neg A.
\]

Isso significa que estabelecer a contrapositiva também estabelece o condicional original.

Em vez de começar supondo \(A\), podemos então trabalhar com:

\[
\neg B
\]

e procurar obter:

\[
\neg A.
\]

A estrutura torna-se:

\[
\neg B
\]

\[
\text{passos justificados}
\]

\[
\neg A.
\]

Essa organização recebe o nome de **demonstração por contraposição**.

Não estamos substituindo a tese por outra afirmação apenas por conveniência. A legitimidade do método vem precisamente da equivalência lógica:

\[
A\to B
\equiv
\neg B\to\neg A.
\]

Portanto, demonstrar a segunda proposição é suficiente para estabelecer a primeira.

Essa mudança de direção pode ser útil quando negar a tese produz uma informação matematicamente mais manejável que a hipótese original. Não existe superioridade geral da contraposição sobre a demonstração direta; trata-se de escolher uma forma equivalente na qual a estrutura do problema se deixe trabalhar com maior clareza.

A diferença entre esse método e o modus tollens é importante.

No modus tollens, já possuímos:

\[
A\to B
\]

como premissa. Também possuímos:

\[
\neg B.
\]

Então inferimos:

\[
\neg A.
\]

Na demonstração por contraposição, \(A\to B\) ainda é justamente aquilo que pretendemos estabelecer. Em vez de utilizá-lo como premissa, demonstramos a proposição equivalente:

\[
\neg B\to\neg A.
\]

O modus tollens **usa** um condicional já disponível; a contraposição **estabelece** um condicional demonstrando sua forma equivalente.

Podemos visualizar essa diferença por meio de uma situação matemática simples.

Considere números reais \(x\) e a afirmação:

> Se \(x>3\), então \(2x+1>7\).

É possível demonstrá-la diretamente. Mas podemos também demonstrar sua contrapositiva:

> Se \(2x+1\leq 7\), então \(x\leq3\).

Suponha:

\[
2x+1\leq7.
\]

Subtraindo \(1\):

\[
2x\leq6.
\]

Dividindo por \(2\):

\[
x\leq3.
\]

Obtivemos exatamente a negação da hipótese original.

Assim, foi estabelecido:

\[
2x+1\leq7\to x\leq3,
\]

e, pela equivalência com a contrapositiva, fica estabelecido:

\[
x>3\to2x+1>7.
\]

Nesse exemplo, a direção direta também seria simples. O interesse está em tornar visível o mecanismo: uma equivalência lógica permite reorganizar a tarefa sem modificar aquilo que, ao final, foi demonstrado.

## 4. Demonstração por contradição

Há situações em que a tese não se oferece naturalmente como uma direção a ser percorrida. Outra possibilidade é investigar o que aconteceria se aquilo que queremos estabelecer fosse falso.

Considere uma tese:

\[
T.
\]

Na **demonstração por contradição**, assumimos temporariamente:

\[
\neg T.
\]

A partir dessa suposição, juntamente com as demais informações legitimamente disponíveis, desenvolvemos o raciocínio.

Se a suposição força uma incompatibilidade, ela não pode ser mantida.

Por exemplo, podemos chegar simultaneamente a:

\[
R
\]

e:

\[
\neg R.
\]

As duas proposições não podem ser verdadeiras na mesma situação. Se essa incompatibilidade foi consequência inevitável da suposição \(\neg T\) combinada com informações legítimas, então a suposição deve ser rejeitada.

Consequentemente, estabelecemos:

\[
T.
\]

O ponto decisivo não é simplesmente “supor o contrário e dar errado”. Uma tentativa que se torna difícil, um cálculo pouco elegante ou um resultado inesperado não constitui contradição.

A incompatibilidade precisa ser real.

Considere a afirmação:

> Não existe um maior número natural.

Suponha, para obter uma contradição, que essa afirmação seja falsa. Então existiria um maior número natural. Chame-o de \(m\).

Pela suposição, nenhum número natural poderia ser maior que \(m\).

Mas:

\[
m+1
\]

também é um número natural, e:

\[
m+1>m.
\]

Obtivemos simultaneamente duas exigências incompatíveis:

\(m\) seria o maior número natural;

e existiria um número natural \(m+1\) maior que \(m\).

A contradição não surgiu porque o cálculo se tornou inconveniente. Ela surgiu porque a suposição de existência de um maior natural obriga uma situação que viola a própria condição atribuída a esse número.

Portanto, a suposição precisa ser rejeitada.

Não existe um maior número natural.

A demonstração por contradição e a demonstração por contraposição podem, em algumas situações, parecer próximas, mas suas estruturas não são idênticas.

Na contraposição de:

\[
A\to B,
\]

a tarefa é reorganizada de forma precisa como:

\[
\neg B\to\neg A.
\]

Há uma nova direção condicional claramente determinada.

Na contradição, partimos da negação da tese e procuramos mostrar que ela não pode coexistir com as demais condições legítimas. Não precisamos necessariamente terminar em \(\neg A\); podemos chegar a qualquer incompatibilidade logicamente decisiva.

Por isso, a contradição não deve ser tratada como um procedimento automático a ser escolhido sempre que o caminho direto não aparece imediatamente. Se uma demonstração direta ou uma contraposição deixa a estrutura mais transparente, não há ganho em esconder o raciocínio dentro de uma contradição.

O método serve à organização da justificativa, e não o contrário.

## 5. Demonstração por casos

Algumas afirmações precisam abranger situações que se apresentam de maneiras diferentes.

Suponha que sabemos:

\[
A\lor B.
\]

Isso significa que toda situação relevante considerada satisfaz pelo menos uma dessas alternativas.

Queremos estabelecer uma tese \(C\).

Uma possibilidade é mostrar primeiro que, sob \(A\),

\[
C
\]

é verdadeira.

Depois, mostrar que, sob \(B\),

\[
C
\]

também é verdadeira.

Em termos lógicos, temos:

\[
A\lor B,
\]

\[
A\to C,
\]

\[
B\to C.
\]

Como todas as possibilidades abrangidas por \(A\lor B\) conduzem à mesma tese, podemos concluir:

\[
C.
\]

Essa organização recebe o nome de **demonstração por casos**.

Seu ponto mais importante não é a simples divisão do raciocínio. É a **cobertura das possibilidades**.

Imagine que uma afirmação possa ocorrer em três situações legítimas:

\[
A,\qquad B,\qquad D.
\]

Se demonstrarmos a tese apenas sob \(A\) e sob \(B\), nada foi estabelecido sobre \(D\). Mesmo que os dois primeiros casos estejam perfeitamente demonstrados, a prova geral permanece incompleta.

Por isso, os casos precisam cobrir todas as possibilidades relevantes.

Eles não precisam necessariamente ser mutuamente exclusivos. Pode existir uma situação que pertença a mais de um caso sem que isso prejudique a demonstração. O essencial é que não exista uma possibilidade admissível deixada de fora.

Em muitos exemplos elementares, casos separados sem sobreposição tornam a exposição mais simples, mas a validade do método depende da cobertura, não da exclusividade.

Também é necessário que os diferentes ramos conduzam à mesma tese.

Se queremos estabelecer \(C\), não basta obter \(C\) em um caso e uma afirmação sem relação suficiente com \(C\) em outro. Cada possibilidade precisa levar à conclusão pretendida, direta ou legitimamente.

Uma ilustração simples pode ser dada sem introduzir uma nova teoria matemática.

Suponha que, para determinado objeto, saibamos que ocorre \(A\) ou \(B\), e que queremos estabelecer \(C\).

No primeiro caso, suponha \(A\). A partir das informações disponíveis, obtemos:

\[
D
\]

e de \(D\):

\[
C.
\]

No segundo caso, suponha \(B\). Por outro caminho, obtemos:

\[
E
\]

e de \(E\):

\[
C.
\]

Os ramos podem utilizar informações intermediárias diferentes. O que os reúne é o fato de que a divisão \(A\lor B\) cobre as possibilidades consideradas e ambos terminam estabelecendo a mesma tese \(C\).

A demonstração por casos não consiste, portanto, em testar alguns exemplos. Cada “caso” representa uma classe inteira de situações abrangidas por determinada condição, e todas as possibilidades relevantes precisam ser contempladas.

## 6. Demonstração de equivalência e escrita justificada

Considere agora uma tese com a forma:

\[
A\leftrightarrow B.
\]

Uma bicondicional reúne duas direções:

\[
A\to B
\]

e:

\[
B\to A.
\]

Por isso, demonstrar apenas:

\[
A\to B
\]

não estabelece toda a bicondicional.

É necessário demonstrar também:

\[
B\to A.
\]

Uma demonstração de equivalência pode, portanto, ser organizada em duas partes conceituais.

Primeiro, estabelecemos:

\[
A\to B.
\]

Depois:

\[
B\to A.
\]

Quando ambas as direções foram justificadas, temos:

\[
A\leftrightarrow B.
\]

As duas partes não precisam utilizar a mesma estratégia.

Pode acontecer de:

\[
A\to B
\]

admitir um caminho direto natural, enquanto:

\[
B\to A
\]

seja mais transparente por contraposição. A bicondicional exige simetria quanto ao que deve ser estabelecido — as duas direções —, mas não exige simetria na maneira de demonstrá-las.

Essa observação aponta para uma característica mais geral do trabalho com demonstrações: **encontrar uma prova e apresentá-la não são exatamente a mesma atividade**.

Durante a investigação, podemos testar exemplos, manipular expressões, tentar uma demonstração direta, abandonar esse caminho, examinar a contrapositiva ou começar pela própria tese perguntando o que seria suficiente para alcançá-la.

Podemos, por exemplo, olhar para a tese \(B\) e perceber que seria suficiente estabelecer \(D\). Em seguida, perguntar o que permitiria obter \(D\), chegando a uma condição \(E\). Talvez então descubramos que \(E\) decorre facilmente da hipótese \(A\).

A descoberta pode ter ocorrido mentalmente na ordem:

\[
B
\leftarrow
D
\leftarrow
E
\leftarrow
A.
\]

Mas, uma vez encontrado o caminho, a demonstração pode ser apresentada na ordem justificativa:

\[
A
\]

\[
E
\]

\[
D
\]

\[
B.
\]

Trabalhar retrospectivamente durante a descoberta não significa inverter arbitrariamente inferências na versão final. Significa utilizar a tese como orientação para descobrir quais passos intermediários poderiam ser suficientes para alcançá-la.

A demonstração redigida deve permitir ao leitor reconstruir por que cada passagem relevante é legítima.

Isso não exige registrar toda tentativa abandonada. Se cinco caminhos foram explorados antes de encontrar um sexto que funciona, a demonstração final não precisa narrar esse processo. Ela precisa apresentar o argumento que efetivamente estabelece a tese.

Também não é necessário explicitar cada microetapa concebível.

Uma demonstração pode ser concisa quando seus passos intermediários são recuperáveis pelo leitor no nível adequado. Mas a concisão deixa de ser qualidade quando elimina justamente a razão que sustenta a passagem principal.

Há uma diferença entre omitir uma operação elementar e omitir o argumento central.

Palavras como “logo”, “portanto” e “assim” não resolvem essa diferença. Elas indicam que uma conclusão está sendo apresentada, mas não criam a relação lógica que a justifica. Escrever:

> Portanto, \(B\).

não torna \(B\) consequência de \(A\) se nenhuma passagem legítima foi estabelecida entre as duas afirmações.

Uma demonstração pode apoiar-se em definições, hipóteses, equivalências, propriedades e resultados já legitimamente estabelecidos. Isso permite que a Matemática avance sem reconstruir cada fundamento a cada novo argumento. O que não pode ocorrer é utilizar como fundamento algo cuja legitimidade depende justamente da tese que ainda está sendo demonstrada.

Suponha que queremos estabelecer \(T\).

Se, em algum ponto essencial do raciocínio, assumimos \(T\) como informação disponível e depois utilizamos essa própria informação para concluir \(T\), a argumentação é **circular**.

A circularidade pode ser evidente:

\[
T
\]

\[
\therefore T,
\]

mas também pode estar escondida em várias etapas. O problema permanece o mesmo: a tese foi utilizada como fundamento antes de ter sido legitimamente estabelecida.

Por outro lado, descobrir uma falha numa tentativa de demonstração não produz automaticamente a negação da tese.

Se encontramos uma inferência inválida, uma lacuna ou uma etapa que não conseguimos justificar, estabelecemos apenas que **aquele argumento não demonstra a afirmação**.

A tese pode continuar verdadeira e exigir outro caminho.

Para mostrar que ela é falsa, é necessário apresentar uma refutação legítima — por exemplo, um contraexemplo quando sua estrutura permitir —, e não apenas constatar que uma tentativa de prova fracassou.

A força de uma demonstração não vem da quantidade de símbolos utilizados, do número de casos testados ou da autoridade de quem a apresenta. Ela está na possibilidade de reconstruir uma cadeia de razões pelas quais, a partir do que foi legitimamente admitido, a tese não é apenas anunciada, mas efetivamente estabelecida.
