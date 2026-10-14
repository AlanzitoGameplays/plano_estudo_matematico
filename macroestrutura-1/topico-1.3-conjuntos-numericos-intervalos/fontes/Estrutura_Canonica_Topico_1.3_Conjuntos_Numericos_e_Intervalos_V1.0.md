# ESTRUTURA CANÔNICA DO TÓPICO 1.3 — CONJUNTOS NUMÉRICOS E INTERVALOS

**Plano de Estudo Matemático 4.0 — Macroestrutura 1: Fundamentos**  
**Versão local:** 1.0 — 13/10/2026  
**Estado:** arquitetura geral consolidada para orientar a produção; tratada como referência estável, sujeita a reabertura apenas por problema real.  
**Abrangência:** Estrutura Única do Tópico; núcleo matemático comum dos Blocos; diretrizes gerais dos Textos Teóricos e Práticos; corpus, representações, fronteiras e critérios de auditoria.  
**Natureza:** documento local de arquitetura, **não** substitui as Estruturas Canônicas V1.1 nem as Regras Gerais especializadas.

> **Propósito.** Este arquivo registra o conjunto suficiente de decisões para que os Textos Teóricos e Práticos do Tópico 1.3 sejam desenvolvidos com identidade matemática, continuidade, rigor, controle de pré-requisitos e economia. Não é o Texto Teórico, não é o Texto Prático, não é um Prompt-Mestre e não estabelece quotas universais de exemplos, exercícios ou páginas.

---

# I. POSIÇÃO CURRICULAR E IDENTIDADE

## 1. Posição no Plano

- **Macroestrutura 1 — Fundamentos:**
  - 1.1 — Lógica Matemática;
  - 1.2 — Teoria dos Conjuntos;
  - **1.3 — Conjuntos Numéricos e Intervalos**;
  - 1.4 — Relações e Introdução à Ideia de Função.
- **Desenvolvimentos posteriores decisivos:** 2.1 — Sistemas de Numeração; 2.2 — Operações Fundamentais e Propriedades; 2.3 — Ordem, Valor Absoluto, Aproximação e Estimativa; 2.4 — Potenciação, Radiciação e Notação Científica; 2.5 — Divisibilidade, Números Primos, MDC e MMC; 3.1 — Frações e Números Decimais. Essas unidades não devem ser antecipadas integralmente.

## 2. Identidade matemática

O Tópico organiza **domínios numéricos**, estabelece relações entre eles, introduz o domínio dos números reais em sua apresentação escolar e estuda **subconjuntos de \(\mathbb R\) determinados por condições de ordem**, particularmente os intervalos.

Possui três dimensões coordenadas:

1. **Classificatória:** caracterizar números naturais, inteiros, racionais e irracionais e reconhecer pertinências.
2. **Estrutural:** compreender inclusões e a composição do conjunto dos reais, sem confundir número, sua representação e o conjunto a que pertence.
3. **Representacional e relacional:** relacionar números reais, pontos da reta, ordem, desigualdades, intervalos e operações conjuntistas.

A unidade do Tópico não nasce de uma lista de classes numéricas; nasce da pergunta sobre **qual domínio está em consideração e como selecionar, comparar e representar seus elementos**.

## 3. Pergunta central

**Como os números se organizam em diferentes conjuntos, que relações existem entre esses conjuntos e como a ordem real permite representar e operar com subconjuntos da reta?**

## 4. Insuficiência curricular e função

Os Tópicos 1.1 e 1.2 já fornecem linguagem lógica, pertinência, inclusão e operações conjuntistas. Ainda não especificam sistematicamente os domínios numéricos usados na Matemática posterior nem a notação de regiões da reta real. O Tópico 1.3 transforma esses instrumentos gerais em linguagem de classificação numérica, ordenação e intervalos, preparando a delimitação de domínios, condições e conjuntos-solução, em especial no Tópico 1.4, na Álgebra e em Funções.

## 5. Profundidade e princípio de calibração

**Profundidade conceitual alta; exigência operacional moderada; formalização proporcional.** O Tópico deve ensinar o significado, as condições e as relações entre os objetos, sem tentar desenvolver toda a aritmética desses objetos.

**Distinção orientadora:** conhecer o domínio numérico e suas representações **não equivale** a dominar sistematicamente as operações e técnicas próprias desse domínio.

---

# II. CONTRATOS GERAIS

## 6. Contrato de entrada — o que já pode ser utilizado

**De 1.1 — Lógica Matemática:** sentenças abertas e condições; conectivos, particularmente \(\land\), \(\lor\), negação e implicação; quantificadores e contraexemplos no nível já legitimado.

**De 1.2 — Teoria dos Conjuntos:** conjunto e elemento; \(\in\), \(\notin\); conjuntos por enumeração e por propriedade; \(\varnothing\); \(\subseteq\), igualdade, inclusão própria, diferença entre pertinência e inclusão; \(\cup\), \(\cap\), \(\setminus\); universo relativo quando pertinente; finitude e cardinalidade finita.

**Conhecimento numérico informal de apoio:** números de contagem e zero, negativos usuais, algumas frações e decimais familiares, localização aproximada e comparações elementares. Essa familiaridade **não** autoriza presumir algoritmos ou provas formais que o Plano só desenvolverá posteriormente.

## 7. Contrato negativo — o que ainda não pode ser exigido

Não pressupor que o estudante já domine:

- algoritmos gerais de operações, simplificação e equivalência de frações;
- conversões gerais entre frações, dízimas e números decimais;
- divisibilidade, paridade em nível demonstrativo, MDC e coprimalidade;
- potenciação e radiciação sistemáticas;
- transformações algébricas de inequações e estudo de expressões algébricas;
- propriedades axiomáticas completas da ordem, valor absoluto e técnicas de aproximação;
- teoria de cardinalidades infinitas, completude dos reais, cortes de Dedekind ou sequências de Cauchy.

Uma operação simples pode ser usada como **apoio local explicado**, se necessária ao significado; não pode tornar-se cobrança encoberta do conteúdo futuro.

## 8. Contrato de saída do Tópico

Ao final, o estudante deve poder:

1. caracterizar \(\mathbb N\), \(\mathbb Z\), \(\mathbb Q\), os irracionais e \(\mathbb R\) no nível escolar contratado;
2. classificar exemplos, reconhecer pertinências simultâneas e justificar não pertinências;
3. explicar por que \(\mathbb N\subsetneq\mathbb Z\subsetneq\mathbb Q\subsetneq\mathbb R\);
4. interpretar \(p/q\), com \(p,q\in\mathbb Z\), \(q\neq0\), distinguindo número de representação;
5. distinguir representações decimais finitas, eventualmente periódicas e não periódicas, reconhecendo o estatuto do resultado usado;
6. compreender a existência de irracionais sem depender de demonstrações posteriores;
7. compreender a apresentação escolar de \(\mathbb R\), a correspondência número–ponto e a reta real ordenada;
8. interpretar \(<\), \(>\), \(\leq\), \(\geq\) e condições simultâneas de ordem;
9. representar subconjuntos reais por desigualdades, notação de intervalos e reta;
10. distinguir extremos incluídos/excluídos, intervalos limitados/ilimitados e casos vazios ou unitários;
11. realizar união, interseção e diferença de intervalos simples e reconhecer resultados que **não** são intervalos únicos;
12. identificar e justificar erros de classificação, notação, pertença, inclusão, representação e extremos.

## 9. Fronteiras positivas do Tópico

| Estatuto | Conteúdo e função |
|---|---|
| **Ensina** | Domínios \(\mathbb N,\mathbb Z,\mathbb Q\); números irracionais e reais; representações decimais como caracterização introdutória; reta real; ordem necessária aos intervalos; conceito, notações e operações conjuntistas com intervalos. |
| **Utiliza** | Lógica e linguagem conjuntista anteriores; cálculos numéricos elementares estritamente auxiliares. |
| **Retoma pontualmente** | Pertinência versus inclusão; igualdade e diferença; universo; conjunto vazio; finitude quando houver novo trabalho matemático. |
| **Prepara** | Domínios, condições e conjuntos-solução; relações e funções; tratamento aritmético e algébrico da ordem. |
| **Adia** | Aritmética geral de frações, decimais, potências e raízes; técnicas de desigualdades; prova clássica da irracionalidade de \(\sqrt 2\) dependente de divisibilidade. |
| **Exclui do núcleo** | Construção axiomática ou analítica de \(\mathbb R\); teoria de cardinalidade infinita; números complexos; teoria geral de sequências e de limites. |

**Regra de fronteira:** proximidade temática, presença no corpus ou utilidade em um exemplo **não** bastam para ampliar o contrato de saída.

---

# III. MOVIMENTO GLOBAL E ORGANIZAÇÃO INTERNA

## 10. Movimento matemático

\[
\underbrace{\mathbb N\subsetneq\mathbb Z\subsetneq\mathbb Q}_{\text{domínios e inclusão}}
\quad\longrightarrow\quad
\underbrace{\text{irracionais},\ \mathbb R,\ \text{reta e ordem}}_{\text{ampliação e representação}}
\quad\longrightarrow\quad
\underbrace{\text{desigualdades e intervalos}}_{\text{subconjuntos e operações}}.
\]

O progresso não é meramente uma passagem do “fácil” ao “difícil”: muda a **ação intelectual predominante** — classificar e relacionar, depois ampliar e localizar, por fim selecionar e operar.

## 11. Divisão em Blocos — decisão justificada

**Três Blocos; nove Partes**, sem exigência de extensão semelhante.

| Bloco | Pergunta local | Movimento próprio | Partes |
|---|---|---|---|
| **I — Números Naturais, Inteiros e Racionais** | A que domínios pertencem os números e por que se incluem? | Reconhecer, caracterizar, representar e comparar. | I. Naturais e Inteiros; II. Racionais e suas Representações; III. Relações entre Domínios. |
| **II — Números Irracionais, Reais e Reta Numérica** | O que falta aos racionais e como representar e ordenar os reais? | Reconhecer insuficiência, ampliar o domínio e localizar. | I. Insuficiência dos Racionais e Irracionais; II. Reais; III. Reta Real e Ordem. |
| **III — Intervalos Reais** | Como representar e operar com conjuntos definidos pela ordem real? | Selecionar, representar e operar. | I. Intervalos Limitados; II. Ilimitados e Casos Especiais; III. Operações e Relações. |

Cada Bloco tem pergunta, identidade, movimento e saída próprios. Não criar Blocos adicionais para igualar tamanhos nem reunir as três funções em uma única exposição heterogênea. Em particular, **operações com intervalos pertencem ao Bloco III**, e não exigem um Bloco IV.

## 12. Regimes matemáticos em nível macro

| Regime | Bloco I | Bloco II | Bloco III |
|---|---|---|---|
| Conceitual | Muito alto | Muito alto | Alto |
| Simbólico-notacional | Alto | Moderado | Muito alto |
| Operacional | Baixo | Baixo | Alto |
| Demonstrativo | Moderado | Moderado | Moderado |
| Representacional | Moderado | Muito alto | Muito alto |

As intensidades são **orientações de função**, não percentuais, quotas ou moldes editoriais.

---

# IV. BLOCO I — NÚMEROS NATURAIS, INTEIROS E RACIONAIS

## 13. Identidade, pergunta e contrato

**Identidade:** caracterização dos primeiros domínios numéricos e justificação de suas inclusões.  
**Pergunta:** quais números pertencem a \(\mathbb N\), \(\mathbb Z\) e \(\mathbb Q\), e por que cada conjunto está contido no seguinte?  
**Entrada específica:** linguagem conjuntista, inteiros e frações em exemplos familiares; sem algoritmos gerais de cálculo fracionário.  
**Saída específica:** classificar, distinguir representação de número, reconhecer pertinências múltiplas e justificar \(\mathbb N\subsetneq\mathbb Z\subsetneq\mathbb Q\).

## 14. Parte I — Números Naturais e Inteiros

**Função:** estabelecer a convenção para os naturais e a passagem aos inteiros, incorporando os negativos.

**Núcleo:**

\[
\mathbb N=\{0,1,2,3,\ldots\},\qquad
\mathbb Z=\{\ldots,-2,-1,0,1,2,\ldots\}.
\]

- Adotar **\(0\in\mathbb N\)**, reconhecer brevemente que outra convenção existe, sem gerar notações concorrentes desnecessárias.
- Distinguir números naturais, inteiros negativos e zero; mostrar que \(\mathbb N\subsetneq\mathbb Z\).
- Explicar o significado de negativo sem converter o Bloco em aula de regras de sinais.
- Evitar estudar paridade, divisibilidade, algoritmo de subtração, inversos e axiomas aritméticos como novos núcleos.

**Gargalo:** natural/inteiro é relação de inclusão, não classificação exclusiva.  
**Teoria:** definições, exemplos e contraste; justificativa breve de inclusão.  
**Prática:** reconhecer pertenças, refutar pertinências erradas, explicar inclusão própria.

## 15. Parte II — Números Racionais e suas Representações

**Função:** construir a racionalidade por uma condição de representação, distinguindo objeto numérico e forma escrita.

**Definição nuclear:**

\[
\mathbb Q=\left\{\frac pq\;\middle|\;p,q\in\mathbb Z,\ q\neq0\right\}.
\]

**Condições essenciais:**

- Numerador e denominador pertencem a \(\mathbb Z\); o denominador não é zero.
- Todo inteiro é racional porque \(n=n/1\).
- Escritas diferentes podem representar o mesmo número, por exemplo \(1/2=2/4=0{,}5\), sem exigir algoritmos gerais de frações.
- Racionalidade não significa “ser escrito obrigatoriamente como uma fração não inteira”.

**Representação decimal — calibração obrigatória:** ensinar como **caracterização reconhecida, sem demonstração geral**, que um número real é racional se e somente se admite representação decimal **finita ou eventualmente periódica**. Diferenciar:

- decimal finito: \(1/2=0{,}5\);
- decimal periódico desde o início: \(1/3=0{,}333\ldots\);
- decimal eventualmente periódico: \(1/6=0{,}1666\ldots\).

Esse resultado é um **teorema caracterizador**, não definição arbitrária nem conclusão provada por três exemplos. Não introduzir os procedimentos gerais de converter dízimas em frações ou frações em decimais; cabem ao Tópico 3.1. Não discutir exceções de unicidade de expansões decimais sem necessidade curricular.

**Gargalos:** \(q\neq0\); diferença entre número e representação; racionalidade de inteiros; dízima não é qualquer decimal infinito.

**Teoria:** fundamentar definição, equivalência representacional simples e inclusão \(\mathbb Z\subseteq\mathbb Q\); interpretar a caracterização decimal, declarando sua condição de resultado não demonstrado integralmente aqui.

**Prática:** decidir racionalidade em exemplos autorizados e justificar com uma representação válida ou com a caracterização apresentada; não cobrar conversões ou técnicas inéditas.

## 16. Parte III — Relações entre os Domínios Numéricos

**Função:** integrar as três classes, consolidando a diferença entre \(x\in A\) e \(A\subseteq B\).

\[
\mathbb N\subsetneq\mathbb Z\subsetneq\mathbb Q.
\]

- Justificar as inclusões pelo significado dos conjuntos.
- Usar testemunhas simples para justificar que são **próprias**: por exemplo, \(-1\in\mathbb Z\setminus\mathbb N\) e \(1/2\in\mathbb Q\setminus\mathbb Z\).
- Trabalhar pertinências simultâneas: \(2\in\mathbb N\), \(2\in\mathbb Z\), \(2\in\mathbb Q\).
- Distinguir **menor conjunto estudado que contém o número** de **todos os conjuntos que o contêm**.
- Um esquema de inclusão pode sintetizar a relação; uma tabela de pertinência é condicional, não obrigatória.

**Saída do Bloco I:** classificação fundamentada e relações entre domínios estáveis, sem antecipação de aritmética sistemática.

---

# V. BLOCO II — NÚMEROS IRRACIONAIS, REAIS E RETA NUMÉRICA

## 17. Identidade, pergunta e contrato

**Identidade:** ampliação além dos racionais e compreensão escolar do domínio real como reta ordenada.  
**Pergunta:** por que os racionais não esgotam os números da reta, e como representar e ordenar os números reais?  
**Entrada específica:** racionalidade e representação decimal no regime calibrado, conjuntos e diferença, comparações numéricas elementares.  
**Saída específica:** reconhecer irracionalidade com fundamento apropriado, compreender \(\mathbb R\), localizar e comparar reais e interpretar condições de ordem.

## 18. Parte I — A Insuficiência dos Racionais e os Números Irracionais

**Função:** apresentar a existência de números não representáveis como quociente de inteiros, sem pressupor técnicas posteriores de divisibilidade e radiciação.

**Sequência conceitual (evitar circularidade):**

1. Retomar funcionalmente a propriedade decimal dos racionais.
2. Introduzir, **em linguagem pré-formal**, a ideia de um domínio numérico maior, associado à reta e a representações decimais que não precisam terminar nem repetir períodos.
3. Mostrar a existência de uma representação infinita não eventualmente periódica **com lei de formação clara**; por exemplo, \(0{,}101001000100001\ldots\), com blocos de zeros progressivamente maiores entre os dígitos 1.
4. Interpretar essa expansão, mediante a caracterização decimal já apresentada, como um exemplo de número não racional, chamado **irracional**.
5. Reservar a definição conjuntista formal \(\mathbb R\setminus\mathbb Q\) para a Parte II, depois de o domínio \(\mathbb R\) ter sido estabelecido.

**Exemplos reconhecíveis:** \(\sqrt2\), \(\sqrt3\) e \(\pi\) podem aparecer como irracionais **cuja irracionalidade é informada**, não demonstrada no estágio atual. Não afirmar que a mera inspeção de casas decimais finitas prove irracionalidade.

**Estatuto:** definição de irracionalidade relativa ao domínio real; teorema de caracterização decimal utilizado com escopo reconhecido; existência exemplificada por construção decimal acessível, sem construção formal de \(\mathbb R\).

**Não exigir:** prova por contradição de \(\sqrt2\), paridade e MDC, algoritmo de radiciação ou generalizações sobre todas as expressões com raízes.

**Gargalo:** “decimal infinito” **não** implica “irracional”; periodicidade eventual é a distinção pertinente.

## 19. Parte II — O Conjunto dos Números Reais

**Função:** estabilizar o domínio \(\mathbb R\) e a decomposição entre racionais e irracionais sem fingir uma construção axiomática dos reais.

**Tratamento escolar:** \(\mathbb R\) é apresentado como o domínio numérico associado aos pontos de uma reta idealizada orientada, considerado aqui com todas as suas posições; a correspondência número–ponto será desenvolvida na Parte III. Esta é **uma apresentação didática**, não prova da completude nem definição formal fundacional.

Após introduzir \(\mathbb R\), caracterizar o conjunto dos irracionais como \(\mathbb R\setminus\mathbb Q\), e então registrar:

\[
\mathbb Q\subsetneq\mathbb R,\qquad
\mathbb R=\mathbb Q\cup(\mathbb R\setminus\mathbb Q),
\qquad
\mathbb Q\cap(\mathbb R\setminus\mathbb Q)=\varnothing.
\]

- Explicar que todo real é racional ou irracional, nunca os dois ao mesmo tempo.
- Mostrar que essa decomposição **não é**, por si só, uma construção dos números reais: é uma relação conjuntista após o domínio ter recebido significado.
- Não introduzir sistemas \(\mathbb C\) nem aritmética complexa.
- Não utilizar indevidamente analogias visuais que coloquem racionais e irracionais em trechos geométricos separados da mesma reta.

**Gargalos:** composição versus construção; exclusividade entre racional e irracional (diferentemente das inclusões \(\mathbb N,\mathbb Z,\mathbb Q\)); diferença entre número e ponto representativo.

## 20. Parte III — Reta Real e Relações de Ordem

**Função:** construir o significado geométrico e simbólico da ordem estritamente necessário para os intervalos.

**Núcleo:**

- Origem \(0\), orientação positiva, unidade e correspondência escolar entre números reais e pontos da reta.
- Números menores à esquerda, maiores à direita; negativos, zero e positivos.
- Relações \(<\), \(>\), \(\leq\), \(\geq\) e desigualdades encadeadas.
- Comparabilidade e tricotomia: para \(a,b\in\mathbb R\), exatamente uma das relações \(a<b\), \(a=b\), \(a>b\) ocorre.
- Transitividade: \(a<b\land b<c\Rightarrow a<c\).
- Leitura lógica: \(a<x<b\) significa \(x>a\land x<b\).
- **Ausência de consecutivos reais:** entre dois reais distintos existe outro real; explicar por exemplos e justificativa proporcional, sem construir teoria analítica. Um intervalo com extremos diferentes contém infinitos reais.

**Contrastes essenciais:** ponto representativo versus número; posições representadas versus continuidade da reta; reta com marcações finitas versus conjunto real não reduzido às marcações.

**Fronteira da ordem:** interpretar e comparar, **não** estudar propriedades operatórias gerais (adição, multiplicação e inversão de desigualdades), resolver inequações algébricas ou desenvolver módulo, aproximação e estimativa sistematicamente. Esses estudos terão tratamento posterior, especialmente em 2.3 e na Álgebra.

**Representação essencial:** reta orientada, posições geometricamente corretas de exemplos usados para comparar números, possibilidade de explicitar a região selecionada por \(x<a\) ou \(x\geq b\).

**Saída do Bloco II:** domínio real e ordem interpretados com precisão suficiente para construir os intervalos.

---

# VI. BLOCO III — INTERVALOS REAIS

## 21. Identidade, pergunta e contrato

**Identidade:** subconjuntos de \(\mathbb R\) determinados por condições de ordem e suas relações conjuntistas.  
**Pergunta:** como representar e operar com conjuntos de reais delimitados por desigualdades?  
**Entrada específica:** \(\mathbb R\), reta ordenada, desigualdades elementares, conjuntos por propriedade, inclusão, união, interseção e diferença.  
**Saída específica:** interpretar e traduzir representações, decidir pertinência e inclusão, operar com intervalos sem perder a situação dos extremos.

**Significado nuclear, antes do catálogo de símbolos:** um intervalo real é um conjunto sem lacunas **na ordem**: se \(x,z\) pertencem ao intervalo e \(x<y<z\), então \(y\) também pertence ao intervalo. Essa caracterização pode ser explicada com prosa e reta; a escrita quantificada geral não é obrigatória na primeira exposição.

## 22. Parte I — Intervalos Limitados e seus Extremos

**Função:** construir intervalos como conjuntos e estabelecer as três representações coordenadas: desigualdade, notação de intervalo e região na reta.

Para \(a,b\in\mathbb R\) com \(a<b\):

| Tipo | Notação local | Conjunto por condição |
|---|---|---|
| Aberto | \((a;b)\) | \(\{x\in\mathbb R\mid a<x<b\}\) |
| Fechado | \([a;b]\) | \(\{x\in\mathbb R\mid a\leq x\leq b\}\) |
| Fechado à esquerda, aberto à direita | \([a;b)\) | \(\{x\in\mathbb R\mid a\leq x<b\}\) |
| Aberto à esquerda, fechado à direita | \((a;b]\) | \(\{x\in\mathbb R\mid a<x\leq b\}\) |

**Convenção tipográfica local:** usar preferencialmente **ponto e vírgula** para separar extremos em intervalos, evitando ambiguidade com a vírgula decimal brasileira. Reconhecer variantes usuais dos livros, sem adotá-las simultaneamente como notação principal.

**Gargalos:** extremos pertencem ou não pertencem? Pontos marcados na reta são amostras ou todos os elementos? Colchetes são parte da notação, não substitutos da compreensão das desigualdades.

**Representação essencial:** extremos preenchidos/vazios com legenda conceitualmente correta, alinhados com as desigualdades mostradas.

## 23. Parte II — Intervalos Ilimitados e Casos Especiais

**Função:** estender a seleção real aos sentidos ilimitados da reta e reconhecer casos limítrofes.

Exemplos canônicos:

\[
(-\infty;b]=\{x\in\mathbb R\mid x\leq b\},\qquad
[a;+\infty)=\{x\in\mathbb R\mid x\geq a\}.
\]

Incluem-se, sem necessidade de quadros gigantes, as variantes com \(<\) e \(>\) e a reta inteira:

\[
(-\infty;+\infty)=\mathbb R.
\]

**Esclarecimento obrigatório:** \(+\infty\) e \(-\infty\) **não são elementos de \(\mathbb R\)** nem extremos numéricos que possam ser incluídos no conjunto; sua notação é sempre aberta do lado infinito.

**Casos especiais:** quando os extremos coincidem, explicitar:

\[
[a;a]=\{a\},\qquad (a;a)=\varnothing.
\]

Para \(a=b\), os intervalos semiabertos com apenas um extremo incluído também são vazios. Se \(a>b\), a condição encadeada \(a\leq x\leq b\) não pode ser satisfeita; tratar casos com limites invertidos quando for funcional, sem multiplicar convenções.

**Distinção nuclear:** *limitado* não significa *finito*. Se \(a<b\), \([a;b]\) possui infinitos elementos reais, embora seus extremos sejam finitos. Não desenvolver cardinalidade infinita.

## 24. Parte III — Operações e Relações entre Intervalos

**Função:** empregar as operações já legitimadas no Tópico 1.2 em novos objetos, com foco em ordem, extremos, sobreposições e possíveis lacunas.

**Núcleo:**

- decidir pertinência e inclusão de intervalos com base nas desigualdades;
- executar \(A\cap B\) (condições simultâneas), \(A\cup B\) (alternativas) e \(A\setminus B\) (pertence ao primeiro e não ao segundo);
- distinguir intervalos disjuntos, apenas adjacentes, sobrepostos e contidos, sobretudo quando extremos coincidem;
- reconhecer se o resultado é um intervalo único, uma união de intervalos ou \(\varnothing\);
- utilizar a reta e a notação simbólica com fidelidade recíproca;
- quando conveniente, relacionar o complemento relativo ao universo \(\mathbb R\), **sem** reensinar a teoria geral de complementos.

**Contraste estrutural:**

\[
[1;5]\setminus(2;4)=[1;2]\cup[4;5].
\]

A diferença pode ter duas componentes separadas: não é um único intervalo. O exemplo serve à compreensão, não como lista obrigatória de exercícios.

**Limites:** não exigir inequações que precisem ser resolvidas por transformações algébricas ou estudo do sinal de expressões ainda não ensinados.

**Saída do Bloco III:** trânsito seguro entre \(\text{desigualdade}\leftrightarrow\text{intervalo}\leftrightarrow\text{reta real}\), operações conjuntistas simples e verificação dos extremos e da forma do resultado.

---

# VII. ESTATUTOS MATEMÁTICOS, NOTAÇÃO E CONTROLE DE RIGOR

## 25. Estatuto dos resultados mais sensíveis

| Enunciado ou conteúdo | Estatuto exigido no material |
|---|---|
| \(\mathbb N=\{0,1,\ldots\}\) | **Convenção local** sobre a inclusão do zero. |
| Caracterização de \(\mathbb Q\) por \(p/q\) | **Definição** no nível escolar do domínio considerado. |
| \(\mathbb Z\subseteq\mathbb Q\) | **Consequência justificável** por \(n=n/1\). |
| Decimal real racional \(\Leftrightarrow\) finito ou eventualmente periódico | **Caracterização/teorema**, apresentado sem demonstração geral nesta etapa. |
| Irracionalidade de \(\sqrt2\) ou de \(\pi\) | **Fato matemático informado**; sua demonstração não é exigida agora. |
| \(\mathbb R\) associado à reta sem lacunas | **Apresentação escolar do domínio**, não construção formal ou prova de completude. |
| Decomposição \(\mathbb R=\mathbb Q\cup(\mathbb R\setminus\mathbb Q)\) | **Identidade conjuntista**, após introduzir \(\mathbb R\); não constrói, sozinha, \(\mathbb R\). |
| Tricotomia, transitividade e existência de números entre reais distintos | **Propriedades básicas da ordem**, interpretadas e justificadas proporcionalmente. |
| Notações de intervalos e extremos | **Definições e convenção de escrita**, sempre ligadas às condições. |
| União/interseção/diferença de intervalos | **Aplicações** das operações por pertinência já construídas. |

Não apresentar ilustração como prova universal, conjectura como teorema, definição como consequência demonstrada ou simplificação escolar como construção axiomática.

## 26. Notação preferencial e advertências

- \(\mathbb N,\mathbb Z,\mathbb Q,\mathbb R\): conjuntos numéricos centrais.
- Irracionais: preferir **\(\mathbb R\setminus\mathbb Q\)**, depois de introduzir \(\mathbb R\). Variantes das fontes podem ser reconhecidas, não precisam competir como notações canônicas.
- Inclusão: \(\subseteq\); inclusão própria, quando necessária: \(\subsetneq\). Manter o significado adotado no Tópico 1.2.
- Pertinência: \(\in,\notin\); distinguir de inclusão.
- Intervalos: \((a;b),[a;b],[a;b),(a;b]\), mantendo ponto e vírgula entre os extremos no texto em português.
- Decimais: vírgula decimal, por exemplo \(0{,}5\), \(0{,}333\ldots\).
- \(\pm\infty\): símbolos que **não** representam elementos de \(\mathbb R\).
- Conjuntos por propriedade: explicitar domínio e condição quando isso evitar ambiguidade.

## 27. Regras locais de justificação

- Demonstrar diretamente inclusões simples porque isso ensina a aplicar definições.
- Apresentar testemunha para refutar uma inclusão, quando pertinente.
- Não transformar provas de irracionalidade, construção dos reais ou propriedades operatórias da ordem em obrigatoriedade.
- Explicar um “porquê” quando revelar significado, condição, limitação ou método; evitar demonstração cerimonial e microexplicação redundante.

---

# VIII. ESTRUTURA GERAL DOS TEXTOS TEÓRICOS

## 28. Objetivo e orientação de prosa

O Texto Teórico deve **construir compreensão matemática**, não registrar catálogo de definições, fórmulas e casos. Preservar o sentido antes, durante e após a simbolização. A presença professoral deve aparecer nas decisões sobre sequência, exemplos, distinções, precisão e economia — não em metadiscurso, entusiasmo artificial ou retrospectivas fixas.

| Bloco | Prosa predominante | Ritmo necessário |
|---|---|---|
| I | Conceitual, classificatória, simbólico-explicativa | Econômico nas convenções e exemplos familiares; desacelerar em racionalidade, diferença entre número e escrita e pertinências múltiplas. |
| II | Conceitual-explicativa, comparativa e geométrico-descritiva | Desacelerar em decimal não periódico, existência de irracionais e estatuto dos reais; integrar reta e ordem sem excursão axiomática. |
| III | Simbólico-explicativa, operacional e representacional | Desacelerar em inclusão de extremos e resultados de operações; reduzir texto onde uma reta matematicamente fiel esclarecer mais. |

**Retomada funcional:** um conceito anterior deve reaparecer realizando trabalho novo, sem introduções dedicadas a recapitular compulsoriamente o percurso inteiro.

## 29. Exemplos teóricos: funções, não quotas

- **Bloco I:** racional que também é inteiro; racional não inteiro; diferentes escritas para o mesmo número; inclusão própria e contraexemplos.
- **Bloco II:** decimal periódico versus não periódico; lei de formação de um exemplo não periódico; localização e comparação de reais; fato conhecido não demonstrado versus fato demonstrado.
- **Bloco III:** contraste entre extremos incluídos/excluídos; três registros de um mesmo intervalo; extremos compartilhados; diferença que produz união de intervalos.

Não impor três exemplos por Parte nem níveis fixos. Exemplos teóricos constroem significado; **exemplos resolvidos práticos**, quando legitimados, modelam decisões e estratégias de ação.

## 30. Representações essenciais

1. **Inclusões numéricas:** esquema de \(\mathbb N\subsetneq\mathbb Z\subsetneq\mathbb Q\subsetneq\mathbb R\) e distinção racional/irracional, sem insinuar separação espacial dos pontos na reta.
2. **Reta real:** origem, unidade, orientação e exemplos com posições coerentes; quando indispensável, localizar racionais e irracionais sem pretensão de medir cardinalidades.
3. **Intervalos:** regiões contínuas selecionadas, pontos abertos/fechados e representação dos intervalos ilimitados.
4. **Operações:** representações comparativas de intervalos, preservando extremos, lacunas e união de componentes.

Tabelas servem à comparação quando reduzem esforço cognitivo; não são exigência editorial universal. Determinar **função matemática → representação → fidelidade → implementação**; só então escolher SVG, HTML/CSS ou outro recurso.

---

# IX. ESTRUTURA GERAL DOS TEXTOS PRÁTICOS

## 31. Objeto e autonomia

O Texto Prático tem contrato próprio: transformar conhecimentos já construídos em **ações matemáticas observáveis**. A prática não precisa reproduzir exatamente a distribuição das Partes teóricas, mas deve respeitar seus pré-requisitos e fronteiras. O núcleo é **Exercícios + Gabarito Comentado**; exemplos resolvidos, quiz, desafio e seções diagnósticas são **condicionais**.

## 32. Contratos práticos por Bloco

| Bloco | Competências centrais observáveis | Competências mais exigentes, desde que preparadas |
|---|---|---|
| **I** | Identificar, classificar, reconhecer pertenças, justificar inclusões e distinguir escrita de número. | Analisar classificações equivocadas; decidir se uma testemunha refuta corretamente uma inclusão. |
| **II** | Diferenciar racionais/irracionais por critérios já construídos; representar e comparar pontos; interpretar ordem. | Diagnosticar inferências falsas sobre infinitude decimal, periodicidade, racionalidade e reta. |
| **III** | Traduzir desigualdade–intervalo–reta, decidir pertinência/inclusão, operar e conferir extremos. | Escolher representações, investigar casos com limites coincidentes, reconstruir intervalos a partir de condições e reconhecer resultados desconexos. |

**Contrato negativo prático:** não exigir redução de dízimas, frações complexas, argumentos de divisibilidade, extração de raízes, inequações algébricas, prova de irracionalidade ou teoremas de completude. Nenhuma atividade pode introduzir sua teoria essencial apenas no gabarito.

## 33. Progressão prática e apoio

A progressão deverá resultar da redução de apoio e do crescimento das decisões do estudante, não só da complexidade aparente dos números:

- reconhecimento e interpretação com condições claras;
- aplicação e tradução entre representações;
- escolha de método ou representação com menos apoio;
- justificativa, diagnóstico e verificação autônoma;
- integração e transferência, quando compatíveis com o contrato.

Não impor sequência ou quantidade rígida. **Bloco III** é candidato forte a Exemplos Resolvidos guiados quando a operação com extremos exigir planejamento que a teoria conceitual ainda não modelou. O gabarito posterior não substitui preparação anterior quando uma estratégia é genuinamente nova.

## 34. Gabarito Comentado

- Resolver e auditar efetivamente toda atividade.
- Explicar critérios matemáticos suficientes, preservando alternativas legítimas de construção ou justificativa.
- Ser proporcional à ação exigida; respostas imediatas não precisam virar demonstrações longas.
- Não corrigir por via de longa aula teórica uma lacuna que deveria ter sido suprida antes.
- Usar as mesmas convenções notacionais e, quando útil, representações correspondentes às propostas no enunciado.

## 35. Corpus prático e proveniência

O **Mapa de Uso do Corpus Teórico V1** é exclusivamente teórico e **não fecha** as fontes dos exercícios. Para a prática, selecionar conforme a arquitetura local: livros, fontes oficiais ENEM/FATEC, questões autorais e outras fontes pertinentes. Distinguir proveniência como **Autêntica**, **Baseada/Adaptada** e **Original**, nos termos das Regras Gerais Práticas V3.0; revalidar toda adaptação e preservar fidelidade quando a questão for identificada como autêntica.

**Estado da norma prática de referência:** a V3.0 disponível declara-se **candidata para auditoria e congelamento**. Sua função neste planejamento não deve ser falsamente identificada como a de uma versão normativa já congelada.

---

# X. CORPUS TEÓRICO E MAPA DE CONSULTA

## 36. Corpus e autoridade

O corpus está organizado no repositório privado **`AlanzitoGameplays/plano_estudo_matematico_corpus`**. O repositório principal **`AlanzitoGameplays/plano_estudo_matematico`**, pasta `macroestrutura-1/topico-1.2-conjuntos/`, fornece **precedentes críticos** de produção e materialização, não um molde a copiar.

O **Mapa de Uso do Corpus Teórico V1** é um **catálogo de navegação**, não auditoria integral das obras. O mapa indica para **1.3**:

- **Primeira consulta:** FGV Volume I (§2.2); OpenStax *Prealgebra 2e* (caps. 3 e 7); Serge Lang, *Basic Mathematics* (caps. 1 e 3).
- **Apoios seletivos:** FME Volume 1; OpenStax *Contemporary Mathematics* (cap. 3).

Prioridade de consulta **não** equivale a hierarquia absoluta de rigor. Uma obra deve ser lida nas passagens necessárias; nenhuma autoriza expandir o currículo por possuir mais capítulos relacionados.

## 37. Funções por fonte

| Fonte | Função principal no Tópico 1.3 | Onde consultar | Limite de importação |
|---|---|---|---|
| **FGV — Matemática para o Ensino Médio, vol. I** | Terminologia escolar, definições, números reais, ordem, intervalos, retas e contrastes. | Cap. 2, §2.2, sobretudo seções 2.2.1–2.2.5 e seus desdobramentos, páginas impressas iniciadas em 61. | Não copiar tratamentos algébricos ou demonstrações cujo pré-requisito não foi construído. |
| **OpenStax — Prealgebra 2e** | Explicação gradual, inteiros, reta e classificação racional/irracional. | Cap. 3 e §7.1 (em capítulo 7). | §7.1 pressupõe capítulos anteriores de cálculo com frações e decimais; o Plano 4.0 ainda não os sistematizou. |
| **Serge Lang — Basic Mathematics** | Precisão conceitual dos números, propriedades e apresentação dos reais como reta. | Caps. 1 e 3; especialmente abertura do cap. 3 e ordem/positividade. | Não transferir toda a axiomatização operatória, manipulações ou provas de ordem. |
| **FME — Fundamentos de Matemática Elementar, vol. 1** | Contraponto escolar estruturado: definições, inclusões, representações e intervalos. | Cap. III — Conjuntos Numéricos, seções pertinentes. | Não importar toda a aritmética, provas via divisibilidade, indução finita ou leituras laterais. |
| **OpenStax — Contemporary Mathematics** | Apoio didático adicional quando houver lacuna concreta nas fontes prioritárias. | Cap. 3, conforme mapa de corpus. | Usar seletivamente; o mapa não garante inspeção integral dessa seção. |

**Consulta complementar excepcional:** Hammack, *Book of Proof*, para calibrar prova, refutação e linguagem de conjuntos quando surgir dúvida real; métodos já ensinados em 1.2 não precisam ser reensinados em 1.3.

## 38. Prioridade por Bloco

- **Bloco I:** FGV §2.2 e OpenStax *Prealgebra*; Lang como controle conceitual; FME como contraste seletivo.
- **Bloco II:** FGV §2.2, Lang cap. 3, OpenStax §7.1; FME como apoio para representações e contraste.
- **Bloco III:** FGV §2.2.5 e FME cap. III para intervalos; Lang como controle da ordem; outras fontes apenas quando houver necessidade específica.

**Critério de leitura:** abrir o capítulo adequado, verificar hipóteses, esclarecer sua função e decidir o que será incorporado, reformulado ou rejeitado. Não atribuir a uma fonte demonstração ou exemplo não conferido.

## 39. Precedentes do Tópico 1.2 — o que herdar e evitar

**Herdar:** progressão por operações intelectuais; definições e resultados interpretados; distinção de prova/refutação; hipóteses explícitas; representações matematicamente fiéis; continuidade por uso real; composição editorial econômica; gabarito com critérios de suficiência.

**Evitar:** retrospectivas artificiais; metadiscurso sobre a própria aula; separação mecânica de expressões curtas; demonstrações excessivas; tratar toda investigação como obrigatória; exigir estratégia inédita sem preparação; copiar número de páginas ou Blocos; omitir trechos do Texto Mestre ao materializar HTML/PDF.

**Achado específico anterior:** a abertura conceitual do Texto Mestre do Bloco I de 1.2 não foi transposta integralmente ao HTML/PDF. Esse desvio exige conferência de integridade na etapa editorial, não reformulação geral das apostilas já aprovadas.

---

# XI. CRITÉRIOS DE AUDITORIA, PRODUÇÃO E ENCERRAMENTO

## 40. Auditoria matemática e curricular

Confirmar, antes de aprovar os materiais:

1. **Correção:** cada definição, inclusão, comparação e operação com intervalos é correta e conserva suas hipóteses.
2. **Estatutos:** definição, convenção, caracterização, consequência, propriedade e fato não demonstrado estão claramente diferenciados quando necessário.
3. **Dependências:** nenhuma justificativa ou exercício exige técnica posterior sem apoio local legítimo.
4. **Progressão:** I classifica/relaciona, II amplia/localiza e III seleciona/opera; sem reensino automático.
5. **Escopo:** frações, decimais, ordem, radicais e infinito não se transformaram em outros Tópicos antecipados.
6. **Representações:** retas, pontos, intervalos, extremos e operações conservam seu significado simbólico.
7. **Teoria–prática:** ações exigidas pela prática foram tornadas intelectualmente disponíveis; novidade estratégica relevante tem preparação adequada.
8. **Economia:** cada seção, exemplo, demonstração, tabela ou figura realiza trabalho matemático identificável.
9. **Fidelidade editorial:** Texto Mestre, HTML/CSS e PDF correspondem integralmente, inclusive aberturas e conclusões; examinar paginação e navegação.
10. **Documentação:** marcar claramente status dos artefatos e fontes efetivamente examinadas, sem inferir aprovação a partir da mera existência de um PDF.

## 41. Estratégia de produção

**Ordem funcional:** arquitetura do Tópico (este documento) → planejamento apenas do necessário para cada Bloco → Prompt-Mestre do Tópico, quando útil → produção por unidade adequada → auditoria → congelamento do respectivo artefato.

- Preferir **um Prompt-Mestre teórico para todo o Tópico**, como síntese operacional, em vez de um prompt novo por Bloco.
- O projeto prático pode ter seu próprio Prompt-Mestre porque executa uma tarefa distinta; não multiplicá-lo por tradição.
- Produzir o **Bloco completo** quando isso preservar a coesão; dividir por Partes apenas se a densidade realmente justificar.
- A unidade arquitetônica (Bloco/Parte) não obriga a mesma unidade de geração do texto.
- Não estabelecer antecipadamente páginas, quantidade de exemplos ou exercícios.
- Se surgir lacuna real que altera contratos, dependências, fronteiras ou competências, reabrir **somente** a camada necessária. Problema textual ou editorial isolado não é razão para redesenho curricular.

## 42. Critério de encerramento do Tópico

A estrutura está cumprida quando o aluno pode identificar e relacionar conjuntos numéricos, explicar a ampliação aos reais em seu nível escolar, interpretar a ordem e a reta, representar intervalos por três registros e executar operações conjuntistas simples verificando os extremos e a forma do resultado — **sem** depender de técnicas ainda não construídas e **sem** exigir aprofundamentos fora do escopo.

A possibilidade abstrata de acrescentar outros exemplos, provas ou representações não impede o congelamento de uma execução já suficiente.

---

# XII. SÍNTESE OPERACIONAL — CONSULTA RÁPIDA

| Decisão | Contrato estável |
|---|---|
| Identidade | Domínios numéricos, relações e subconjuntos de \(\mathbb R\) definidos pela ordem. |
| Organização | **3 Blocos / 9 Partes**, assimétricos em extensão. |
| I | Naturais e Inteiros → Racionais e Representações → Relações entre Domínios. |
| II | Insuficiência dos Racionais e Irracionais → Reais → Reta e Ordem. |
| III | Intervalos Limitados → Ilimitados/Casos Especiais → Operações/Relações. |
| Convenção | \(0\in\mathbb N\); \(\subseteq\)/\(\subsetneq\) com significado anterior; ponto e vírgula nos intervalos. |
| Racionais | Definição por \(p/q\), equivalência simples e caracterização decimal **sem prova geral**; sem aritmética completa. |
| Irracionais | Existência e significado, com exemplo decimal de lei explícita; \(\sqrt2\), \(\pi\) sem prova obrigatória. |
| Reais | Apresentação escolar ligada à reta, sem construção formal; decomposição só após o domínio fazer sentido. |
| Ordem | Comparação, tricotomia, transitividade e ausência de consecutivos; sem técnicas gerais de inequações. |
| Intervalos | Condição de pertinência, extremos, reta e operações; resultado pode não ser intervalo único. |
| Teoria | Compreensão, precisão, justificativa proporcional, representação funcional, economia. |
| Prática | Competência em ação, autonomia, preparação estratégica quando necessária, gabarito proporcional. |
| Corpus prioritário | FGV I (§2.2), Prealgebra (caps. 3 e 7), Lang (caps. 1 e 3). |
| Corpus seletivo | FME I; Contemporary Mathematics (cap. 3); Hammack só se surgir necessidade pertinente. |
| Processo | Sem quotas, seções ou etapas extras obrigatórias; congelar após suficiência auditada. |

---

# XIII. DOCUMENTOS DE AUTORIDADE E PROVENIÊNCIA

Este documento deriva da discussão de arquitetura e calibração do Tópico 1.3 e se subordina aos seguintes materiais do projeto:

1. `Plano_de_Estudo_Matematico_V4.0.pdf` — documento-mãe e currículo.
2. `Estruturas_Canonicas_Plano_Matematico_V1.1.md` — arquitetura de Tópicos, Blocos e Partes; contratos; regimes; corpus; representação; encerramento.
3. `Regras_Gerais_Construcao_Texto_Teorico_Matematico_V3.1.md` — execução, exemplos, demonstrações, prosa e auditoria do Texto Teórico (**definitiva e congelada**, conforme o documento).
4. `Regras_Gerais_Construcao_Texto_Pratico_Matematico_V3.0.md` — execução, atividades, proveniência, gabarito e auditoria da prática (**candidata**, conforme o documento disponível).
5. `Mapa_de_Uso_do_Corpus_Teorico_V1.md` — catálogo de navegação do corpus teórico; não certifica leitura integral de cada obra.
6. Repositórios `AlanzitoGameplays/plano_estudo_matematico` (precedentes do Tópico 1.2) e `AlanzitoGameplays/plano_estudo_matematico_corpus` (acervo bibliográfico).
7. Fontes temáticas efetivamente consultadas no planejamento: *Matemática para o Ensino Médio*, FGV, vol. I; *Basic Mathematics*, Serge Lang; *Prealgebra 2e*, OpenStax; *Fundamentos de Matemática Elementar*, vol. 1, com apoio do respectivo mapa do corpus. A consulta foi seletiva, não uma auditoria integral de cada livro.

**Situação dos artefatos:** este arquivo é uma **referência local produzida para consulta e continuidade**. Seu uso como estrutura consolidada não implica que os Textos Teóricos, Textos Práticos, HTML/CSS ou PDFs futuros estejam prontos ou aprovados. Nenhuma alteração nos repositórios decorre da criação deste arquivo.

**FIM — ESTRUTURA CANÔNICA DO TÓPICO 1.3 · VERSÃO LOCAL 1.0**
