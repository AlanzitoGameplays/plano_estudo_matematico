# Guia Codex
## Plano de Estudo Matemático — Versão 1.0

**Documento 06 da Consolidação Pós-Tópico 1.1**  
**Escopo:** orientação operacional para delegar tarefas ao Codex com contexto, escopo, autonomia e validação proporcionais ao trabalho.

Este documento define **como um agente executa tarefas dentro do sistema editorial e técnico do Plano de Estudo Matemático**.

Ele não substitui os documentos anteriores:

- **Documento 01 — Arquitetura e Taxonomia Canônica:** define o que pertence ao sistema e em que nível;
- **Documento 02 — Regras Gerais HTML/CSS:** define o que deve ser respeitado normativamente;
- **Documento 03 — Arquitetura Técnica HTML/CSS:** define como a infraestrutura técnica funciona;
- **Documento 04 — Catálogo de Componentes HTML/CSS:** define soluções opcionais aprovadas, suas funções, usos e limites;
- **Documento 05 — Fluxo de Produção HTML/CSS:** define a ordem de construção, validação, correção e congelamento;
- **Documento 06 — Guia Codex:** define como selecionar contexto, delimitar escopo, calibrar autonomia, executar, validar e encerrar uma tarefa delegada a um agente;
- **AGENTS.md:** será a camada curta de instruções operacionais de alta frequência.

> **O Codex deve receber o menor contexto suficiente para executar corretamente a tarefa autorizada.**

---

# 1. FINALIDADE E ESCOPO

O Guia responde à pergunta:

> **Como delegar ao Codex uma tarefa do Plano Matemático fornecendo apenas o contexto, o escopo, a autonomia e os critérios de validação necessários?**

Seu objetivo é impedir dois erros opostos:

1. **contexto insuficiente**, que força o agente a improvisar ou reconstruir decisões já consolidadas;
2. **contexto excessivo**, que aumenta custo, ruído, releitura e risco de misturar precedentes locais com regras sistêmicas.

O Guia rege principalmente:

- diagnóstico e auditoria;
- patches locais;
- correções textuais autorizadas;
- construção de novas apostilas;
- extensões locais;
- ajustes de componentes;
- mudanças sistêmicas autorizadas;
- manutenção documental.

O Guia não ensina programação, HTML, CSS, Git, VS Code ou o produto Codex de forma genérica.

Também não depende de nomes específicos de modelos, quotas, preços ou limitações temporárias de produto.

---

# 2. RELAÇÃO COM OS DOCUMENTOS 01–05

O sistema possui separação deliberada de responsabilidades.

| Documento | Pergunta principal |
|---|---|
| **01 — Arquitetura e Taxonomia** | O que pertence ao sistema e em que nível? |
| **02 — Regras Gerais** | O que uma produção precisa respeitar? |
| **03 — Arquitetura Técnica** | Como a infraestrutura canônica funciona? |
| **04 — Catálogo de Componentes** | Que soluções opcionais aprovadas já existem? |
| **05 — Fluxo de Produção** | Em que ordem a produção e a validação acontecem? |
| **06 — Guia Codex** | Como um agente recebe e executa uma tarefa dentro desse sistema? |

O Documento 05 define **o processo**.

O Documento 06 define **a delegação e a operação do agente dentro desse processo**.

Para construção nova, o agente respeita o fluxo completo pertinente.

Para manutenção, utiliza o fluxo abreviado adequado.

---

# 3. PRINCÍPIOS OPERACIONAIS

## 3.1 Contexto proporcional à novidade

Uma tarefa recebe apenas o conjunto de informações necessário para sua execução correta.

Mais contexto só é útil quando acrescenta informação necessária.

## 3.2 Consultar o menor precedente suficiente

Precedentes são evidências de soluções anteriores, não a primeira fonte de autoridade.

Quando regra, arquitetura ou componente já resolvem a dúvida, não é necessário reler apostilas antigas.

## 3.3 Uma apostila herda antes de criar

O movimento normal é:

**HERDAR → ADAPTAR → CRIAR SOMENTE O NOVO**

O agente não deve reinventar infraestrutura, identidade ou componente que já possuam solução adequada.

## 3.4 Autonomia proporcional ao risco

A autonomia cresce ou diminui conforme:

- clareza da tarefa;
- novidade;
- ambiguidade;
- alcance da alteração;
- risco de regressão;
- número de dependências afetadas.

## 3.5 Modificar somente o necessário

O agente deve alterar apenas os arquivos e trechos necessários para cumprir a tarefa autorizada.

## 3.6 Extensão local não nasce canônica

Uma solução nova pode surgir localmente quando necessária.

Ela não deve ser promovida ao Catálogo, à Base ou às Regras durante a própria construção apenas por ser nova ou bem-sucedida.

## 3.7 Conteúdo mestre não é superfície de correção silenciosa

Uma tarefa HTML/CSS não autoriza automaticamente alterações conceituais no conteúdo.

## 3.8 Congelado está fora da superfície normal de alteração

Versões congeladas só são reabertas por motivo real e com autorização compatível.

## 3.9 Validar o que realmente mudou

A extensão da validação deve acompanhar o alcance da alteração.

## 3.10 O fluxo seleciona contexto; não acumula contexto

O passado deve ser condensado em sistema, não reaprendido indefinidamente.

---

# 4. MOVIMENTO GERAL DA DELEGAÇÃO

```text
IDENTIFICAR A TAREFA
        ↓
DELIMITAR O ESCOPO
        ↓
SELECIONAR O CONTEXTO
        ↓
CALIBRAR A AUTONOMIA
        ↓
EXECUTAR
        ↓
VALIDAR
        ↓
RELATAR
        ↓
ENCERRAR
```

Quando surgir incerteza relevante:

```text
INCERTEZA
    ↓
É RESOLVIDA PELAS FONTES VIGENTES?
      ↙                         ↘
    SIM                          NÃO
     ↓                            ↓
RESOLVER PELA              A DECISÃO ALTERA
PRECEDÊNCIA                ESCOPO, CONTEÚDO
                           OU SISTEMA?
                           ↙             ↘
                         NÃO              SIM
                          ↓                ↓
                 ESCOLHER A SOLUÇÃO       PARAR
                 MAIS SIMPLES             E PEDIR
                 SUFICIENTE               ORIENTAÇÃO
```

---

# 5. PAPEL DO CODEX NO SISTEMA

O Codex é tratado como **agente de execução técnica dentro de um sistema já governado**.

Pode, conforme a tarefa e a autonomia autorizada:

- ler arquivos;
- comparar fontes;
- analisar estrutura;
- construir HTML/CSS;
- instanciar infraestrutura;
- selecionar componentes existentes;
- produzir extensões locais;
- realizar patches;
- diagnosticar defeitos;
- executar auditorias;
- preparar candidatos a PDF;
- validar o que seu ambiente permite;
- trabalhar com Git dentro do escopo autorizado.

Não possui autoridade automática para:

- redefinir currículo;
- reescrever conteúdo mestre;
- alterar identidade canônica;
- criar regra do sistema;
- promover componente;
- redefinir Arquitetura Técnica;
- alterar Base canônica;
- reabrir versão congelada;
- atualizar vários blocos porque encontrou solução preferível;
- transformar microajuste em convenção;
- decidir sozinho uma mudança sistêmica.

---

# 6. CLASSES DE TAREFA

O agente deve identificar a classe da tarefa antes de executar.

## A — Diagnóstico / Auditoria

**Objetivo:** investigar sem alterar.

Exemplos:

- localizar causa de overflow;
- identificar CSS morto;
- comparar HTML e conteúdo mestre;
- verificar conformidade;
- analisar paginação;
- determinar alcance de um defeito.

## B — Patch Local

**Objetivo:** corrigir defeito delimitado.

Exemplos:

- quebra inadequada;
- largura de tabela;
- espaçamento localizado;
- atributo de atomicidade;
- seletor específico.

## C — Correção Textual Autorizada

**Objetivo:** alterar texto ou conteúdo quando a correção já estiver definida ou explicitamente autorizada.

Exemplos:

- erro de digitação;
- símbolo incorreto;
- trecho corrigido no conteúdo mestre;
- resposta formalmente substituída.

## D — Construção Nova

**Objetivo:** materializar nova apostila a partir de conteúdo mestre aprovado.

Exemplos:

- novo bloco;
- novo tópico;
- nova apostila de conteúdo.

## E — Ajuste de Componente

**Objetivo:** alterar solução compartilhada já existente.

Possui risco maior porque pode afetar múltiplas instâncias.

## F — Extensão Local Nova

**Objetivo:** representar uma função real ainda não atendida pelo sistema, sem promover a solução.

## G — Correção Sistêmica

**Objetivo:** alterar infraestrutura, Base, componente compartilhado, documentação canônica ou outra convenção geral.

Exige autorização explícita.

## H — Manutenção Documental

**Objetivo:** atualizar registros e documentação sistêmica quando solicitado.

Exemplos:

- `VERSOES.md`;
- documento canônico;
- futura Base;
- futuro `AGENTS.md`;
- registro de congelamento.

---

# 7. NÍVEIS DE AUTONOMIA

## Autonomia 0 — Leitura / Diagnóstico

Pode:

- ler;
- comparar;
- diagnosticar;
- apontar riscos;
- recomendar.

Não pode modificar arquivos.

## Autonomia 1 — Patch Determinístico

Pode:

- corrigir defeito local claramente identificado;
- modificar apenas arquivos autorizados;
- escolher microajustes equivalentes;
- aplicar solução já prevista pelo sistema.

Não pode:

- expandir escopo;
- alterar conteúdo;
- alterar componente compartilhado;
- alterar Base;
- alterar documentação canônica.

## Autonomia 2 — Implementação Delimitada

Pode:

- construir nova apostila;
- instanciar Base ou infraestrutura vigente;
- selecionar componentes;
- tomar decisões locais compatíveis com os documentos;
- criar extensão local quando claramente necessária.

Não pode:

- promover extensão;
- redefinir arquitetura;
- alterar currículo;
- criar nova norma;
- reabrir congelados sem autorização.

## Autonomia 3 — Alteração Sistêmica Autorizada

Somente quando explicitamente solicitada.

Pode atingir, dentro do escopo definido:

- Base;
- componente compartilhado;
- infraestrutura;
- documentação canônica;
- comportamento geral.

Exige:

- alcance explícito;
- identificação de impacto;
- validação ampliada;
- relato claro das instâncias afetadas.

---

# 8. PRINCÍPIO DE AUTONOMIA

A autonomia não é determinada pelo tamanho do arquivo ou pelo volume bruto de código.

A avaliação deve considerar:

```text
NOVIDADE
+
AMBIGUIDADE
+
ALCANCE
+
RISCO DE REGRESSÃO
=
NÍVEL DE CONTROLE NECESSÁRIO
```

Uma mudança pequena em um token global pode possuir risco maior que a criação de várias páginas dentro de uma estrutura já estabilizada.

Uma apostila nova pode ser extensa, mas altamente governada por conteúdo, Base, arquitetura e componentes existentes.

---

# 9. HIERARQUIA DAS FONTES

A precedência normativa permanece a definida pelas Regras Gerais vigentes:

1. **conteúdo mestre aprovado**;
2. **Regras Gerais vigentes**;
3. **Arquitetura Técnica vigente**;
4. **componente canônico aplicável no Catálogo**;
5. **precedente comparável, quando necessário**;
6. **instruções específicas da tarefa**.

O **Fluxo de Produção** governa a sequência operacional e os estados de produção; ele não altera essa ordem de autoridade sobre conteúdo, conformidade ou implementação.

Uma instrução específica não pode violar silenciosamente fonte superior.

Quando houver conflito real:

1. identificar as fontes em conflito;
2. preservar a autoridade superior;
3. verificar se a diferença é apenas de escopo ou aplicação;
4. pedir orientação quando a resolução puder alterar substancialmente a execução.

---

# 10. SELEÇÃO DE CONTEXTO

Antes de executar, deve-se identificar:

- classe da tarefa;
- objetivo;
- arquivos que podem ser modificados;
- arquivos que devem permanecer somente leitura;
- documentos que governam diretamente a decisão;
- componentes envolvidos;
- necessidade ou não de precedente;
- forma de validação;
- limites ambientais.

O contexto é selecionado **por função**, não por proximidade histórica.

---

# 11. EQUAÇÃO OPERACIONAL DE CONTEXTO

O contexto normal pode ser representado como:

```text
CONTEXTO NECESSÁRIO
=
AUTORIDADE CANÔNICA RELEVANTE
+
CONTEÚDO DA TAREFA
+
INFRAESTRUTURA NECESSÁRIA
+
COMPONENTES NECESSÁRIOS
+
PRECEDENTE MÍNIMO, SE NECESSÁRIO
```

Não assumir como padrão:

```text
TODAS AS REGRAS
+
TODOS OS RELATÓRIOS
+
TODOS OS BLOCOS
+
TODOS OS HTML
+
TODOS OS CSS
+
TODOS OS PDFs
+
TODO O HISTÓRICO
```

---

# 12. CAMADAS DE CONTEXTO

## Camada A — Contexto da tarefa

Normalmente obrigatório:

- objetivo;
- escopo;
- arquivos-alvo;
- conteúdo pertinente;
- resultado esperado;
- critérios de validação.

## Camada B — Autoridade canônica relevante

Selecionar os documentos ou seções que governam diretamente a tarefa.

Não é necessário carregar integralmente todos os documentos em toda tarefa local.

## Camada C — Implementação

Pode incluir:

- HTML/CSS Base;
- arquivos-alvo;
- componente envolvido;
- infraestrutura diretamente relacionada.

## Camada D — Precedente

Somente quando as camadas anteriores não forem suficientes ou quando a tarefa exigir comparação concreta.

> **O precedente é a última camada, não a primeira.**

---

# 13. CONTEXTO POR CLASSE DE TAREFA

| Classe | Contexto normal | Contexto normalmente desnecessário |
|---|---|---|
| **Diagnóstico** | arquivos-alvo + evidência do defeito + fonte técnica pertinente | todos os blocos e relatórios |
| **Patch local** | alvo + regra/arquitetura/componente diretamente envolvidos + página/PDF quando útil | Plano inteiro, Catálogo inteiro, precedentes não relacionados |
| **Correção textual autorizada** | conteúdo mestre ou correção formal + arquivo-alvo | infraestrutura não afetada |
| **Construção nova** | conteúdo mestre + Regras + Arquitetura Técnica + Fluxo + Base + componentes pertinentes | releitura integral das apostilas anteriores |
| **Extensão local** | conteúdo + Catálogo pertinente + Arquitetura Técnica + arquivo-alvo | promoção sistêmica, precedentes indiscriminados |
| **Ajuste de componente** | ficha + implementação + instâncias afetadas + Regras/Arquitetura pertinentes | documentos sem relação funcional |
| **Correção sistêmica** | documentos canônicos pertinentes + implementação + casos afetados + autorização explícita | histórico sem relação com o defeito |
| **Manutenção documental** | documento-alvo + fontes que determinam a atualização | código das apostilas quando não necessário |

A matriz é orientadora, não rígida.

---

# 14. CONTEXTO QUE NÃO DEVE SER ENVIADO POR PADRÃO

Não fornecer indiscriminadamente:

- todas as apostilas;
- todos os PDFs;
- todos os HTML;
- todos os CSS;
- todos os relatórios;
- histórico completo de conversas;
- explicações já convertidas em norma ou arquitetura;
- componentes que não participam da tarefa;
- precedentes sem relação funcional.

Quando um arquivo já estiver acessível no repositório, preferir indicar seu caminho em vez de duplicar integralmente seu conteúdo no contrato da tarefa.

---

# 15. LEITURA DO REPOSITÓRIO

Quando `AGENTS.md` existir, a ordem operacional normal é:

1. ler `AGENTS.md`;
2. identificar a classe da tarefa;
3. localizar arquivos-alvo;
4. ler o conteúdo mestre pertinente;
5. ler as fontes canônicas necessárias;
6. ler as fichas dos componentes envolvidos;
7. inspecionar a implementação atual;
8. consultar precedente somente se restar dúvida.

Enquanto `AGENTS.md` não existir:

1. partir das fontes indicadas pela tarefa;
2. utilizar este Guia para selecionar contexto e autonomia;
3. ler apenas o necessário para resolver a tarefa.

Não realizar exploração ampla do repositório quando os caminhos relevantes já estiverem definidos.

---

# 16. CONTRATO DA TAREFA

Uma instrução ao Codex deve tornar explícito apenas o que é necessário para evitar ambiguidade relevante.

Estrutura recomendada:

```text
TAREFA
[objetivo]

ESCOPO
[onde a tarefa começa e termina]

FONTES
[arquivos e documentos relevantes]

ARQUIVOS AUTORIZADOS
[arquivos que podem ser modificados]

ARQUIVOS SOMENTE LEITURA
[fontes, precedentes e congelados]

REQUISITOS
[critérios específicos]

NÃO FAZER
[proibições relevantes]

VALIDAÇÃO
[o que precisa ser verificado]

PARAR SE
[condições que exigem orientação]

ENTREGA
[resultado esperado]
```

Nem todos os campos precisam aparecer sempre.

O contrato existe para impedir omissões relevantes, não para transformar toda tarefa em formulário extenso.

---

# 17. ARQUIVOS AUTORIZADOS E SOMENTE LEITURA

## 17.1 Arquivos autorizados

> **O agente modifica apenas o conjunto de arquivos necessário à tarefa autorizada.**

Um novo arquivo pode ser criado quando:

- é necessário para cumprir o resultado solicitado;
- sua criação está claramente contida no escopo;
- não institui nova convenção sistêmica por conta própria.

Se a criação alterar arquitetura ou convenção do sistema, a tarefa deve ser interrompida e reclassificada ou autorizada.

## 17.2 Arquivos somente leitura

Por padrão, quando não forem alvo explícito:

- documentos canônicos;
- conteúdo mestre;
- versões congeladas;
- PDFs aprovados;
- precedentes;
- arquivos de outros blocos;
- Base canônica;
- componentes compartilhados.

Consultar um arquivo não autoriza modificá-lo.

---

# 18. ARQUIVOS CONGELADOS

> **Congelado significa fora da superfície normal de alteração.**

O agente não deve modificar uma versão congelada apenas porque:

- existe estilo mais recente;
- encontrou código mais elegante;
- uma nova Base foi criada;
- seria possível reduzir CSS;
- outra apostila apresenta composição diferente;
- seria possível aumentar uniformidade retrospectiva.

Reabertura exige motivo real e autorização compatível com o Documento 05.

A criação deste Guia não obriga retronormalização dos Blocos I–V.

---

# 19. POLÍTICA DE MODIFICAÇÃO

Antes de alterar arquivos:

1. identificar a causa;
2. identificar o menor arquivo responsável;
3. identificar o alcance;
4. verificar se o sistema já possui solução;
5. verificar se a alteração está autorizada;
6. somente então editar.

Evitar:

- alterações globais por conveniência;
- formatação ampla sem necessidade;
- renomeações não solicitadas;
- limpeza generalizada durante patch;
- refatorações oportunistas;
- alteração estética fora do alvo;
- atualização de arquivos adjacentes apenas por estarem abertos.

---

# 20. POLÍTICA DE PATCH

O movimento normal é:

```text
DIAGNÓSTICO
    ↓
CAUSA
    ↓
MENOR PATCH SUFICIENTE
    ↓
VALIDAÇÃO PROPORCIONAL
```

Um patch local deve corrigir o defeito real sem acumular melhorias paralelas.

Quanto mais madura a apostila, menor deve ser a superfície de alteração.

Se durante o diagnóstico ficar claro que a causa é compartilhada ou sistêmica, o agente não deve fingir que se trata de defeito puramente local.

---

# 21. ALTERAÇÃO DO CONTEÚDO

Durante tarefa HTML/CSS, o agente não deve corrigir silenciosamente:

- erro conceitual;
- inconsistência matemática;
- resposta incorreta;
- ambiguidade relevante;
- contradição;
- definição incompleta.

Ao encontrar problema desse tipo:

1. identificar o trecho;
2. separar problema de conteúdo de problema editorial;
3. não realizar alteração conceitual sem autorização;
4. solicitar orientação quando necessário.

Quando a correção já estiver formalmente definida ou explicitamente autorizada:

1. aplicar na origem apropriada;
2. propagar ao HTML;
3. verificar a paginação e o resultado afetados.

---

# 22. EXTENSÃO LOCAL NOVA

Quando nenhuma solução existente representar adequadamente uma função real:

```text
FUNÇÃO REAL
    ↓
SOLUÇÃO MAIS SIMPLES SUFICIENTE
    ↓
EXTENSÃO LOCAL
    ↓
TESTE
    ↓
VALIDAÇÃO NO PRODUTO
```

A extensão local:

- não entra automaticamente no Catálogo;
- não altera a Base;
- não recebe status canônico;
- não deve ser replicada em outros blocos por padrão.

Promoção é decisão posterior e separada.

---

# 23. MUDANÇA SISTÊMICA

É sistêmica uma alteração que afete, por exemplo:

- identidade;
- tokens globais;
- paginação geral;
- Base;
- componente compartilhado;
- convenção recorrente;
- arquitetura;
- documentação canônica;
- várias apostilas por herança.

Se a tarefa não autorizar mudança sistêmica:

**PARAR.**

Também não se deve esconder defeito sistêmico com remendo local quando a causa estiver comprovadamente no sistema.

A resposta correta é identificar a causa e solicitar ampliação explícita do escopo.

---

# 24. AMBIGUIDADE E INCERTEZA

## A — Microdecisão local

Exemplo: duas variações pequenas de espaçamento preservam igualmente função e sistema.

Ação:

- escolher a solução mais simples suficiente;
- não pedir confirmação.

## B — Ambiguidade estrutural

Exemplo: duas interpretações produzem arquiteturas diferentes.

Ação:

1. consultar fontes vigentes;
2. aplicar a precedência;
3. se continuar aberta, pedir orientação.

## C — Ambiguidade conceitual

Exemplo: o conteúdo permite duas interpretações matemáticas substantivamente diferentes.

Ação:

- não decidir silenciosamente;
- pedir orientação.

---

# 25. CRITÉRIOS DE INTERRUPÇÃO

O agente deve parar e solicitar orientação quando:

- falta arquivo indispensável;
- existe conflito não resolvido entre fontes de autoridade;
- seria necessário alterar conteúdo sem autorização;
- seria necessário reabrir versão congelada;
- seria necessário modificar sistema fora do escopo;
- a decisão criaria nova convenção canônica;
- duas soluções substantivamente diferentes permanecem igualmente plausíveis;
- o resultado final exigido não pode ser validado no ambiente disponível;
- o defeito real está fora dos arquivos autorizados;
- a correção exigiria alcance muito maior que o declarado;
- a tarefa pressupõe estado do repositório que não corresponde ao estado encontrado.

Não pedir orientação para:

- microajustes equivalentes;
- decisões locais reversíveis;
- escolhas já determinadas pelo sistema;
- uso normal de componente cujo contrato é claro.

---

# 26. EVITAR PERGUNTAS DESNECESSÁRIAS

> **O agente não deve transformar toda pequena decisão em pedido de confirmação.**

Quando tarefa, fontes e precedência forem suficientes, executar.

Perguntar somente quando a resposta puder alterar substancialmente:

- significado;
- escopo;
- arquitetura;
- arquivos modificados;
- conteúdo mestre;
- estado congelado;
- regra ou componente sistêmico;
- validação exigida.

---

# 27. VALIDAÇÃO

O agente deve distinguir quatro níveis.

## Validação A — Estática

Pode envolver:

- HTML;
- CSS;
- estrutura;
- conteúdo;
- seletores;
- referências;
- semântica;
- correspondência entre arquivos;
- consistência previsível.

## Validação B — Renderização Auxiliar

Quando disponível:

- preview;
- navegador auxiliar;
- screenshot;
- render local.

Serve a diagnóstico e antecipação.

Não possui autoridade final sobre paginação oficial.

## Validação C — PDF Oficial

O ambiente oficial de geração e validação de paginação é:

**Windows + Chrome**

## Validação D — Preflight

O PDF real é avaliado nos eixos definidos pelo Documento 05.

O agente não deve declarar uma versão **CONGELADA** quando o estágio oficial de PDF e preflight ainda não ocorreu.

---

# 28. LIMITES AMBIENTAIS

> **O agente deve distinguir o que verificou, o que inferiu e o que ainda depende do ambiente oficial.**

Se o ambiente de execução não for o ambiente oficial:

pode entregar, conforme o caso:

- HTML/CSS concluído;
- auditoria estática concluída;
- renderização auxiliar;
- **CANDIDATA A PDF**.

Não pode declarar:

- paginação oficialmente aprovada;
- PDF definitivo;
- versão congelada;

apenas porque uma renderização auxiliar parece correta.

---

# 29. USO PROPORCIONAL DE CAPACIDADE

A intensidade de análise e validação deve acompanhar:

- novidade;
- ambiguidade;
- alcance;
- risco;
- número de dependências;
- dificuldade de diagnosticar regressão.

Exemplos:

| Situação | Necessidade típica |
|---|---|
| troca textual evidente | análise localizada |
| patch de tabela | análise e validação locais |
| construção nova | execução ampla governada pelo sistema |
| ajuste de componente compartilhado | análise de impacto e regressão |
| alteração de paginator | alta atenção sistêmica |

Não se presume que tarefa longa seja conceitualmente difícil, nem que alteração curta seja de baixo risco.

---

# 30. ECONOMIA DE EXECUÇÃO

O agente deve:

- evitar reler arquivos já compreendidos dentro da mesma tarefa;
- evitar buscas amplas quando o caminho exato é conhecido;
- evitar abrir PDF quando HTML/CSS responde integralmente à dúvida;
- evitar abrir apostila anterior quando a ficha do componente basta;
- agrupar validações coerentes;
- evitar regenerações caras após cada microajuste;
- concluir uma unidade lógica antes de validar quando isso for seguro;
- não repetir auditorias que o patch não pode afetar;
- reutilizar informação já obtida na própria execução;
- consultar somente as seções dos documentos necessárias a uma tarefa local quando sua autoridade já estiver clara.

Economia não significa omitir verificação necessária.

Significa eliminar trabalho sem função.

---

# 31. TAREFAS LONGAS

Uma tarefa longa não deve ser automaticamente fragmentada em dezenas de subtarefas.

Dividir quando:

- uma decisão intermediária condiciona etapas posteriores;
- um resultado precisa de aprovação antes de ampliar escopo;
- a validação pode revelar mudança estrutural;
- o volume dificultaria diagnosticar regressão;
- existem módulos realmente independentes que podem ser validados separadamente.

Não dividir apenas para criar checkpoints artificiais.

> **Uma unidade coerente de trabalho deve permanecer uma unidade enquanto isso for seguro.**

---

# 32. PLANEJAMENTO INTERNO

Antes de modificar arquivos, o agente deve conseguir responder:

- qual é o objetivo;
- qual é a classe da tarefa;
- quais arquivos mudam;
- quais arquivos não mudam;
- quais fontes governam as decisões;
- qual é o risco principal;
- qual é o nível de autonomia;
- como o resultado será validado;
- quando deverá parar.

Esse planejamento serve à execução.

Não exige relatório extenso para o usuário, salvo solicitação.

---

# 33. GIT — PAPEL OPERACIONAL

O Guia estabelece princípios de trabalho, não comandos.

O agente deve:

- identificar o estado de trabalho antes de modificar;
- respeitar a política de branch definida para a tarefa;
- preservar alterações não relacionadas já existentes;
- não incluir arquivos fora do escopo apenas porque estão modificados;
- manter mudanças coerentes e rastreáveis;
- não assumir autorização para alterar diretamente o estado integrado em tarefas novas, relevantes ou sistêmicas.

**`main` representa o estado integrado do projeto.**

Trabalho novo ou de risco deve ocorrer em branch apropriada quando a política do projeto assim determinar.

---

# 34. BRANCHES E COMMITS

Conceitualmente:

**BRANCH DE CONSTRUÇÃO**  
→ trabalho novo.

**BRANCH DE PATCH**  
→ correção delimitada, quando necessária.

**MAIN**  
→ estado integrado.

O Guia não impõe nomenclatura de branches enquanto ela não for formalmente definida.

Um commit deve:

- representar mudança coerente;
- possuir escopo compreensível;
- não misturar alterações não relacionadas;
- permitir reconstruir o que mudou.

Não se estabelece aqui política rígida de número, formato ou frequência de commits.

---

# 35. NÃO MODIFICAR `MAIN` SILENCIOSAMENTE

Quando a tarefa envolver:

- construção nova;
- mudança relevante;
- ajuste compartilhado;
- alteração sistêmica;

o agente não deve presumir autorização para modificar diretamente `main`.

Deve seguir a política indicada na tarefa ou no futuro `AGENTS.md`.

Quando alteração direta estiver explicitamente autorizada, ela continua submetida às normas superiores do sistema.

---

# 36. RELATO DA EXECUÇÃO

Ao encerrar, o agente deve relatar de forma curta:

- o que foi alterado;
- quais arquivos foram alterados;
- que validação foi realizada;
- o que ainda depende do ambiente oficial;
- eventual incerteza relevante restante.

Não produzir, sem solicitação:

- diário completo da execução;
- narrativa extensa;
- repetição das Regras;
- relatório de raciocínio interno;
- lista de ações sem utilidade operacional.

---

# 37. RESULTADO PARCIAL

Quando o ambiente não permitir atingir o estado final solicitado, o agente deve entregar o maior estado validado possível.

Exemplo:

```text
HTML/CSS CONCLUÍDO
+
AUDITORIA ESTÁTICA CONCLUÍDA
+
RENDERIZAÇÃO AUXILIAR LIMPA
+
PDF OFICIAL AINDA PENDENTE
```

Estado correto:

**CANDIDATA A PDF**

Estado incorreto:

**CONGELADA**

Nomear corretamente o estado faz parte da integridade da execução.

---

# 38. MATRIZ TAREFA × CONTEXTO × AUTONOMIA × VALIDAÇÃO

| Tarefa | Contexto normal | Autonomia típica | Validação |
|---|---|---:|---|
| **Diagnóstico** | alvo + evidência + fonte pertinente | 0 | análise e diagnóstico |
| **Patch local** | alvo + regra/arquitetura/componente pertinente | 1 | localizada + efeitos plausíveis |
| **Correção textual autorizada** | conteúdo/correção + alvo | 1 | trecho + paginação afetada |
| **Construção nova** | conteúdo + sistema relevante + Base + Fluxo | 2 | ampla, até o limite ambiental |
| **Extensão local** | alvo + Catálogo pertinente + Arquitetura | 2 | função + paginação + produto |
| **Ajuste de componente** | ficha + implementação + instâncias | 2 ou 3 | todas as instâncias plausivelmente afetadas |
| **Correção sistêmica** | sistema + implementação + casos afetados | 3 | regressão ampliada |
| **Manutenção documental** | documento-alvo + fontes determinantes | 1 a 3 | consistência documental |

O nível final depende do risco real, não apenas da classe nominal.

---

# 39. EXEMPLO DE CONTRATO — PATCH LOCAL

```text
TAREFA
Corrigir a quebra inadequada de uma tabela na página indicada.

ESCOPO
Somente a tabela e sua paginação imediata.

FONTES
Arquitetura Técnica — paginação e atomicidade.
Ficha do componente correspondente, se existir.

ARQUIVOS AUTORIZADOS
HTML/CSS da apostila diretamente envolvidos.

ARQUIVOS SOMENTE LEITURA
Conteúdo mestre.
Documentos canônicos.
Outras apostilas.

NÃO FAZER
Não alterar conteúdo.
Não alterar tokens globais.
Não modificar outras tabelas sem relação causal.

VALIDAÇÃO
Regenerar o produto disponível.
Verificar a tabela, a página e páginas cuja paginação possa ter mudado.

PARAR SE
A causa estiver em componente compartilhado ou infraestrutura geral.

ENTREGA
Patch mínimo e relato da validação.
```

---

# 40. EXEMPLO DE CONTRATO — CONSTRUÇÃO NOVA

```text
TAREFA
Construir HTML/CSS de nova apostila a partir do conteúdo mestre aprovado.

ESCOPO
A nova apostila e seus arquivos próprios.

FONTES
Conteúdo mestre.
Regras Gerais pertinentes.
Arquitetura Técnica.
Fluxo de Produção.
Base vigente.
Fichas dos componentes necessários.

AUTONOMIA
Implementação delimitada.

NÃO FAZER
Não copiar apostila anterior como template informal.
Não alterar conteúdo mestre.
Não promover extensões locais.
Não alterar Base ou componentes compartilhados.

VALIDAÇÃO
Auditoria estática.
Preview ou renderização auxiliar, quando disponível.
Preparar estado de CANDIDATA A PDF quando o ambiente oficial não estiver disponível.

PARAR SE
Surgir ambiguidade conceitual, necessidade de alteração sistêmica ou conflito de autoridade.

ENTREGA
HTML/CSS completos, validação realizada e limites ambientais declarados.
```

---

# 41. EXEMPLO DE CONTRATO — MUDANÇA SISTÊMICA

Uma mudança sistêmica exige contrato mais explícito.

```text
TAREFA
Corrigir problema sistêmico identificado.

PROBLEMA
Descrever a causa comprovada e o comportamento esperado.

ALCANCE
Indicar infraestrutura, Base, componente ou documentação afetados.

FONTES
Documentos canônicos pertinentes.
Implementação atual.
Casos reais afetados.

ARQUIVOS AUTORIZADOS
Lista explícita dos arquivos sistêmicos que podem mudar.

CASOS DE REGRESSÃO
Instâncias que precisam continuar funcionando.

VALIDAÇÃO
Auditoria sistêmica proporcional.
Verificação de todas as instâncias plausivelmente afetadas.
PDF/preflight quando a mudança afetar renderização oficial.

PARAR SE
A alteração exigir decisão normativa ou curricular ainda não autorizada.

ENTREGA
Mudança sistêmica delimitada, impacto identificado e validação ampliada.
```

---

# 42. ANTI-PADRÕES

## Anti-padrão 1 — Reaprender o projeto

> “Vou ler todos os blocos para entender o estilo.”

**Correção:** ler o sistema vigente e consultar o menor precedente suficiente.

## Anti-padrão 2 — Refatoração oportunista

> “Já que estou aqui, limpei o CSS inteiro.”

**Correção:** respeitar o escopo e aplicar patch mínimo.

## Anti-padrão 3 — Retronormalização espontânea

> “Encontrei solução melhor e atualizei todos os blocos.”

**Correção:** documentos congelados não são retronormalizados por preferência.

## Anti-padrão 4 — Promoção silenciosa

> “Criei um componente novo e já o coloquei no Catálogo.”

**Correção:** primeiro extensão local; promoção é processo separado.

## Anti-padrão 5 — Correção conceitual no HTML

> “Corrigi a matemática diretamente na página.”

**Correção:** alterar a origem apropriada somente quando autorizado.

## Anti-padrão 6 — Confundir preview com produto final

> “O preview ficou bom, então está definitivo.”

**Correção:** PDF oficial + preflight determinam o estado final.

## Anti-padrão 7 — Confirmação excessiva

> “Pedi autorização para cada microajuste.”

**Correção:** autonomia proporcional; perguntar somente quando a resposta mudar substancialmente a execução.

## Anti-padrão 8 — Improvisação conceitual

> “Havia duas interpretações possíveis, então escolhi uma.”

**Correção:** ambiguidade conceitual exige orientação.

---

# 43. CHECKLIST ANTES DE EXECUTAR

- [ ] Sei qual é a classe da tarefa.
- [ ] Sei qual é o escopo.
- [ ] Sei quais arquivos podem mudar.
- [ ] Sei quais arquivos não podem mudar.
- [ ] Tenho o conteúdo necessário.
- [ ] Identifiquei a autoridade canônica pertinente.
- [ ] Não carreguei precedentes sem necessidade.
- [ ] Sei o nível de autonomia.
- [ ] Sei quando devo parar.
- [ ] Sei como validar.
- [ ] Sei quais limitações ambientais existem.

---

# 44. CHECKLIST ANTES DE ENCERRAR

- [ ] A tarefa solicitada foi concluída no maior estado validável.
- [ ] Não houve expansão de escopo não autorizada.
- [ ] Apenas arquivos necessários foram alterados.
- [ ] Conteúdo mestre foi preservado, salvo autorização explícita.
- [ ] Nenhuma solução local foi promovida silenciosamente.
- [ ] Arquivos congelados foram preservados.
- [ ] A validação foi proporcional ao alcance.
- [ ] Efeitos colaterais plausíveis foram verificados.
- [ ] Limites ambientais foram declarados.
- [ ] O estado final foi nomeado corretamente.
- [ ] O relato final é curto e suficiente.

---

# 45. CRITÉRIOS DE PARADA DO AGENTE

A execução termina quando:

```text
A TAREFA FOI CUMPRIDA
+
A VALIDAÇÃO PROPORCIONAL FOI CONCLUÍDA
+
NÃO HÁ DEFEITO DENTRO DO ESCOPO
+
NOVAS ALTERAÇÕES SERIAM
FORA DO ESCOPO
OU APENAS PREFERÊNCIA
```

O agente não deve continuar com lógica equivalente a:

> “Já que ainda há oportunidade, vou melhorar outras partes.”

Encerrar corretamente é parte da qualidade da execução.

---

# 46. CUSTO PROPORCIONAL

> **O custo de contexto, execução e validação deve ser proporcional à novidade, ao risco e ao alcance da tarefa.**

```text
PATCH LOCAL
→ contexto local
→ patch local
→ validação local
```

```text
CONSTRUÇÃO NOVA
→ contexto mais amplo
→ execução ampla
→ validação ampla
```

```text
MUDANÇA SISTÊMICA
→ contexto sistêmico
→ autorização explícita
→ regressão ampliada
```

Esse princípio não autoriza omitir etapa necessária.

Ele impede apenas que tarefas simples carreguem custo de tarefas sistêmicas.

---

# 47. RELAÇÃO COM `AGENTS.md`

O Guia Codex é o manual operacional completo.

O futuro `AGENTS.md` será a camada curta de entrada e alta frequência.

`AGENTS.md` deverá:

- ser lido primeiro pelo agente;
- apontar para os documentos canônicos;
- resumir somente instruções recorrentes;
- registrar a precedência essencial;
- lembrar a política de congelamento;
- lembrar o princípio de patch mínimo;
- lembrar a autoridade do PDF oficial;
- indicar quando consultar este Guia.

`AGENTS.md` não deverá:

- duplicar o Guia;
- duplicar Regras;
- duplicar Catálogo;
- recatalogar componentes;
- tornar-se documento extenso.

> **AGENTS.md orienta a entrada; o Guia resolve a operação.**

Este documento não escreve integralmente o futuro `AGENTS.md`.

---

# 48. TESTES DE USABILIDADE

## 48.1 Economia de contexto

**Tarefa:** corrigir spacing de uma tabela.

Precisa:

- alvo;
- contexto local;
- regra, arquitetura ou componente pertinente;
- validação necessária.

Não precisa:

- ler os cinco blocos;
- carregar todos os relatórios;
- carregar o Plano inteiro.

## 48.2 Construção nova

**Tarefa:** construir novo bloco.

Precisa:

- conteúdo mestre;
- sistema vigente;
- Fluxo;
- Base;
- componentes pertinentes.

Não precisa reler todas as apostilas anteriores.

## 48.3 Mudança de paginator

**Tarefa:** alterar paginação geral.

Precisa:

- Arquitetura Técnica;
- implementação atual;
- casos afetados;
- regras pertinentes;
- autorização sistêmica;
- regressão ampliada.

## 48.4 Autonomia local

**Situação:** microdiferença de espaçamento.

Se não altera significado, identidade ou convenção, o agente pode escolher solução local adequada.

## 48.5 Função inédita

Pode criar extensão local quando a autonomia permitir.

Não pode promovê-la ao Catálogo durante a construção.

## 48.6 Erro matemático percebido

Não pode corrigir silenciosamente durante tarefa HTML/CSS.

## 48.7 Limite ambiental

Se não há Windows + Chrome oficial, o agente pode produzir candidata a PDF, mas não declarar congelamento.

---

# 49. NÃO RETRONORMALIZAR

A existência deste Guia não obriga:

- reprocessar Blocos I–V;
- reescrever HTML/CSS antigos;
- reorganizar branches históricas;
- modificar commits passados;
- reconstruir apostilas congeladas.

O Guia rege principalmente:

- novas tarefas;
- manutenção futura;
- reaberturas justificadas;
- novos agentes;
- futuras produções.

---

# 50. QUESTÕES ABERTAS

Permanecem abertas até decisão sustentada:

- se haverá apenas um `AGENTS.md` na raiz ou instruções locais adicionais;
- se haverá manifesto formal de versões congeladas além do registro já existente;
- se será criada nomenclatura canônica para branches;
- se haverá template de contrato de tarefa versionado;
- quais auditorias estáticas poderão ser automatizadas antes da execução;
- quais verificações poderão ser automatizadas depois da alteração;
- em que momento a futura Base HTML/CSS será formalmente declarada canônica;
- se haverá uma única Base ou variantes especializadas;
- como gráficos, SVG, imagens e geometria complexa alterarão os contratos de validação;
- quais princípios deste Guia poderão ser generalizados para outros Planos de Estudo;
- se outros Planos precisarão de Guia próprio ou de uma camada geral compartilhada.

Questões abertas não devem ser convertidas silenciosamente em norma.

---

# 51. BASE EMPÍRICA E DOCUMENTAL

Este Guia foi consolidado a partir de:

- **Documento 01 — Arquitetura e Taxonomia Canônica do Sistema de Apostilas — Versão 1.0**;
- **Documento 02 — Regras Gerais HTML/CSS do Plano de Estudo Matemático — Versão 3.0**;
- **Documento 03 — Arquitetura Técnica HTML/CSS do Plano de Estudo Matemático — Versão 1.0**;
- **Documento 04 — Catálogo de Componentes HTML/CSS do Plano de Estudo Matemático — Versão 1.0**;
- **Documento 05 — Fluxo de Produção HTML/CSS do Plano de Estudo Matemático — Versão 1.0**;
- experiência consolidada na produção, correção e congelamento dos Blocos I–V do Tópico 1.1 — Lógica Matemática;
- experiência de uso de agentes na construção e manutenção do sistema, quando convertida em decisão documental verificável.

Os precedentes permanecem fonte empírica sob demanda, não leitura obrigatória de toda nova tarefa.

---

# 52. SÍNTESE OPERACIONAL

O Guia pode ser condensado nos seguintes princípios:

1. **Identificar a tarefa antes de selecionar contexto.**
2. **Contexto proporcional à novidade.**
3. **Consultar o menor precedente suficiente.**
4. **Uma apostila herda antes de criar.**
5. **Autonomia proporcional ao risco.**
6. **Modificar somente o necessário.**
7. **Corrigir a causa com a menor superfície de alteração.**
8. **Quanto mais madura a apostila, menor a superfície de alteração.**
9. **Uma extensão local não nasce canônica.**
10. **Conteúdo mestre não é superfície de correção silenciosa.**
11. **Congelado está fora da superfície normal de alteração.**
12. **Perguntar quando a resposta mudar substancialmente a execução.**
13. **Não perguntar quando o sistema já determina a resposta.**
14. **Validar o que realmente mudou.**
15. **Distinguir o que foi validado do que ainda depende do ambiente oficial.**
16. **O custo de contexto, execução e validação deve ser proporcional ao alcance e ao risco.**
17. **Uma tarefa local não deve carregar o projeto inteiro.**
18. **Uma tarefa nova não precisa reaprender as apostilas anteriores.**
19. **O fluxo seleciona contexto; não acumula contexto.**
20. **O passado deve ser condensado em sistema, não reaprendido indefinidamente.**

O agente começa com uma tarefa delimitada.

Termina quando a tarefa foi executada, a validação proporcional foi concluída, os limites ambientais foram declarados e qualquer nova alteração seria fora de escopo ou apenas preferência.

Esse é o ponto em que execução disciplinada substitui revisão indefinida.
