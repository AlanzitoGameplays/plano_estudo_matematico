# AGENTS.md
## Plano de Estudo Matemático

Este arquivo é a **porta de entrada operacional de alta frequência** para agentes que trabalham neste repositório.

Ele **não é um Documento 07**, não substitui as normas canônicas em `regras/` e não deve duplicá-las integralmente.

> **AGENTS.md orienta a entrada; o Guia Codex resolve a operação.**

Escopo deste arquivo: a raiz do repositório e todos os seus descendentes, salvo existência futura de um `AGENTS.md` mais específico em subdiretório.

---

# 1. REGRA SUPERIOR

> **A forma deve servir ao conteúdo.**

O conteúdo não deve ser expandido, reduzido, reescrito, fragmentado, duplicado ou deformado para servir à composição.

Movimento padrão:

> **HERDAR → ADAPTAR → CRIAR SOMENTE O NOVO**

Preservar é preferível a reinventar quando a solução vigente continua funcionalmente adequada.

---

# 2. ORDEM DE PRECEDÊNCIA

Diante de decisão editorial, estrutural ou técnica, respeite exatamente:

1. **conteúdo mestre aprovado**;
2. `regras/02_Regras_Gerais_HTML_CSS_Plano_Matematico_V3.0.md`;
3. `regras/03_Arquitetura_Tecnica_HTML_CSS_Plano_Matematico_V1.0.md`;
4. componente canônico aplicável em `regras/04_Catalogo_de_Componentes_HTML_CSS_Plano_Matematico_V1.0.md`;
5. precedente comparável, quando necessário;
6. instruções específicas da tarefa.

Uma fonte inferior não pode contrariar silenciosamente uma fonte superior.

Para classificação sistêmica e níveis de canonicidade, consulte:

`regras/01_Arquitetura_e_Taxonomia_Canonica_do_Plano_de_Estudo_V1.0.md`

Para sequência de produção, validação, correção e congelamento, consulte:

`regras/05_Fluxo_de_Producao_HTML_CSS_Plano_Matematico_V1.0.md`

Para contexto, escopo, autonomia, classes de tarefa e operação do agente, consulte:

`regras/06_Guia_Codex_Plano_Matematico_V1.0.md`

---

# 3. REGRAS TEXTUAIS

Quando a tarefa envolver construção, revisão ou correção autorizada do conteúdo textual, consulte também:

- Texto Teórico: `regras/Regras_Gerais_Construcao_Texto_Teorico_Versao_2.0.md`
- Texto Prático: `regras/Regras_Gerais_Construcao_Texto_Pratico_Versao_2.0.md`

Esses documentos não substituem a precedência geral acima.

O conteúdo mestre aprovado continua sendo a autoridade semântica da apostila.

---

# 4. CONTEXTO MÍNIMO SUFICIENTE

Não carregue todo o repositório por padrão.

Selecione apenas o contexto necessário para executar corretamente a tarefa.

Ordem recomendada:

1. este `AGENTS.md`;
2. arquivos diretamente envolvidos;
3. conteúdo mestre pertinente;
4. normas canônicas necessárias;
5. componente realmente aplicável;
6. implementação atual;
7. menor precedente suficiente, somente se ainda houver dúvida.

Princípios:

> **O agente deve receber o menor contexto suficiente para executar corretamente a tarefa autorizada.**

> **Consulte o menor precedente suficiente.**

Precedentes são evidências históricas, não templates nem primeira fonte de autoridade.

---

# 5. CLASSIFIQUE A TAREFA ANTES DE ALTERAR

Antes de editar qualquer arquivo, identifique a natureza principal da tarefa conforme o Guia Codex, por exemplo:

- diagnóstico / auditoria;
- patch local;
- correção textual autorizada;
- construção nova;
- extensão local;
- ajuste de componente;
- mudança sistêmica autorizada;
- manutenção documental.

A autonomia deve ser proporcional à clareza, novidade, ambiguidade, alcance, dependências e risco de regressão.

Se a tarefa for apenas diagnóstico ou auditoria, **não altere arquivos**.

---

# 6. CONTEÚDO MESTRE

O conteúdo mestre aprovado define conceitos, sequência, explicações, exemplos, exercícios, respostas, argumentos e demonstrações.

HTML/CSS não tem autoridade para:

- resumir silenciosamente;
- reescrever conceitos;
- corrigir conteúdo sem autorização;
- alterar exemplos ou respostas;
- mudar a ordem pedagógica;
- acrescentar informação ausente;
- eliminar condição necessária;
- alterar o significado de fórmula ou representação.

Se a composição revelar erro matemático, ambiguidade, contradição ou insuficiência pedagógica:

**PARE.**

Relate o problema e solicite decisão ou correção no conteúdo mestre.

Não corrija conhecimento silenciosamente apenas no HTML final.

---

# 7. BASE HTML/CSS CANÔNICA V1.0

A Base vigente está em:

- `ferramentas/base/Plano_Matematico_Base_V1.0.html`
- `ferramentas/base/Plano_Matematico_Base_V1.0.css`

Para fins operacionais do projeto, a **Base HTML/CSS Canônica V1.0 está aprovada e congelada**.

Trate esses arquivos como fonte de instanciação, não como dependência mutável das apostilas já produzidas.

Nova apostila:

> **BASE VIGENTE + COMPONENTES NECESSÁRIOS + EXTENSÃO LOCAL MÍNIMA**

A Base contém infraestrutura universal, como:

- identidade e tokens;
- A4;
- capa;
- página;
- cabeçalho e rodapé;
- hierarquia editorial;
- prosa;
- primitivas matemáticas;
- tabela genérica;
- source-content e source-section;
- paginação e atomicidade;
- outline;
- screen e print;
- ponto genérico de extensão visual.

Não transformar a Base em biblioteca de todos os componentes possíveis.

Não alterar a Base congelada durante a construção normal de uma nova apostila.

Uma mudança na Base exige tarefa sistêmica explícita.

---

# 8. COMPONENTES E EXTENSÕES

Componentes opcionais pertencem ao Catálogo.

Não utilizar um componente apenas porque ele existe.

Use-o somente quando a função pedagógica correspondente estiver realmente presente.

Uma solução nova deve nascer, por padrão, como **extensão local**.

Não promova silenciosamente solução local para:

- Base;
- Catálogo;
- Arquitetura;
- Regras Gerais;
- convenção de todo o Plano.

Promoção posterior exige função recorrente, semântica estável, reutilização real e validação em implementação e PDF.

Princípio de suficiência:

> **prosa → tipografia → espaçamento → estrutura → tabela/componente existente → componente novo → recurso gráfico mais complexo**

Visuais devem possuir função cognitiva real e preservar fidelidade matemática.

---

# 9. ARQUIVOS CONGELADOS

Versões aprovadas e congeladas estão fora da superfície normal de alteração.

Em especial, não retronormalize os Blocos I–V do Tópico 1.1 apenas porque normas ou arquitetura evoluíram depois deles.

Não reabra arquivo congelado para:

- modernizar estilo;
- reduzir duplicação;
- aplicar convenção nova;
- uniformizar diferenças históricas;
- tornar código mais elegante;
- copiar melhoria descoberta em material posterior.

Reabrir somente por:

- defeito concreto;
- erro comprovado;
- necessidade funcional real;
- mudança sistêmica deliberadamente autorizada.

Congelado significa:

> **fora da superfície normal de alteração.**

---

# 10. PATCHES

Para defeito localizado, siga:

> **DIAGNÓSTICO → CAUSA → MENOR PATCH SUFICIENTE → VALIDAÇÃO PROPORCIONAL**

Não faça refatoração oportunista.

Não altere arquivos não relacionados apenas porque estão próximos do defeito.

Quanto mais maduro o artefato, menor deve ser a superfície de alteração.

Se uma correção aparentemente local começar a exigir mudança de:

- identidade global;
- tokens;
- Base;
- paginator universal;
- arquitetura;
- componente compartilhado;
- documentação canônica;
- vários blocos ou apostilas;

trate a situação como possível mudança sistêmica e **pare se ela não estiver explicitamente autorizada**.

---

# 11. PAGINAÇÃO E ATOMICIDADE

A paginação preserva dependências pedagógicas; não busca preenchimento máximo da folha.

Use com parcimônia:

- `.keep-with-next`;
- `data-keep-count`;
- `.atomic-group`.

Princípio:

> **Proteja dependências pequenas; deixe unidades longas quebrarem naturalmente.**

Não use atomicidade excessiva para obter composição estética.

Espaço branco legítimo não é defeito por si só.

Overflow real não deve ser ocultado.

Warnings de overflow exigem inspeção no preflight.

---

# 12. HTML, CSS E PDF

HTML é artefato de produção.

PDF é o produto final de estudo.

Como princípio:

- HTML concentra conteúdo, semântica e estrutura;
- CSS concentra identidade, tipografia, espaçamento, paginação e acabamento.

Não trate a apostila como site ou aplicação interativa quando essa função não pertence ao documento.

A produção não está concluída apenas porque o HTML abre corretamente no navegador.

---

# 13. VALIDAÇÃO

Fluxo geral:

> **ENTENDER → CLASSIFICAR → HERDAR → CONSTRUIR → VALIDAR → CORRIGIR SOMENTE O NECESSÁRIO → CONGELAR**

Validação mínima proporcional à tarefa:

1. auditoria estática;
2. renderização auxiliar, quando útil;
3. geração oficial do PDF, quando a tarefa chegar a esse estágio;
4. preflight;
5. patch mínimo, se houver defeito real;
6. regeneração e revalidação.

Ambiente oficial de renderização:

> **Windows + Chrome**

Outros ambientes são auxiliares.

Se o ambiente oficial não estiver disponível, não declare uma nova apostila como congelada apenas com base em renderização auxiliar.

No PDF, verifique conforme pertinente:

- integridade do conteúdo;
- legibilidade;
- paginação;
- matemática;
- tabelas;
- clipping;
- overflow;
- cabeçalho e rodapé;
- outline/bookmarks;
- identidade editorial.

Classificação prática de correções:

- defeito crítico → corrigir;
- defeito real/local → menor patch suficiente;
- imperfeição cosmética sem impacto → normalmente não reabrir.

> **A ausência de perfeição absoluta não impede o congelamento; a presença de defeito real, sim.**

---

# 14. GIT E SUPERFÍCIE DE ALTERAÇÃO

Antes de editar:

- confirme a branch;
- execute/verifique `git status`;
- identifique os arquivos autorizados;
- preserve mudanças não relacionadas;
- confirme quais arquivos são somente leitura.

Não assuma autorização para escrever diretamente em `main`.

Não inclua arquivos fora do escopo no commit.

Prefira commits de propósito único e superfície claramente auditável.

Não modifique Blocos congelados durante a construção de uma nova apostila.

Não faça alterações no Git remoto se a tarefa não autorizar operações Git.

---

# 15. AMBIGUIDADE E REGRA DE PARADA

Microdecisão local, reversível e sem impacto sistêmico:

→ escolha a solução mais simples suficiente.

Ambiguidade estrutural:

→ consulte as fontes vigentes segundo a precedência.

Ambiguidade conceitual:

→ não improvise.

Pare e peça orientação quando a decisão puder alterar:

- significado;
- conteúdo mestre;
- arquitetura;
- identidade;
- convenção global;
- Base;
- componente compartilhado;
- status de arquivo congelado;
- várias apostilas;
- escopo originalmente autorizado.

Não transforme dúvida sistêmica em decisão local silenciosa.

---

# 16. RELATÓRIO DE ENTREGA

Ao concluir uma tarefa, reporte de forma curta e verificável:

- o que foi alterado;
- quais arquivos foram alterados;
- validações executadas;
- defeitos encontrados;
- limitações restantes;
- estado final do artefato.

Não continue alterando um artefato apenas em busca de perfeição abstrata.

Encerre quando a tarefa autorizada estiver cumprida e validada proporcionalmente.

---

# 17. ROTEAMENTO RÁPIDO

Use esta tabela apenas como ponto de entrada; os documentos canônicos continuam sendo a fonte de autoridade.

| Tarefa | Contexto mínimo típico |
|---|---|
| Classificação sistêmica | AGENTS + Documento 01 |
| Nova apostila HTML/CSS | AGENTS + conteúdo mestre + Documentos 02–05 + Base + componentes pertinentes |
| Texto Teórico | AGENTS + conteúdo mestre + regra de Texto Teórico |
| Texto Prático | AGENTS + conteúdo mestre + regra de Texto Prático |
| Componente existente | AGENTS + Documento 04 + implementação pertinente |
| Extensão local nova | AGENTS + Documentos 02–04 + conteúdo que exige a função |
| Patch local | AGENTS + arquivo defeituoso + norma diretamente pertinente |
| Auditoria/preflight | AGENTS + Documento 05 + artefato avaliado |
| Tarefa Codex complexa | AGENTS + Documento 06 + fontes específicas da tarefa |
| Mudança sistêmica | Documentos 01–06 + autorização explícita + impacto relevante |

---

# 18. REGRA DE ENCERRAMENTO

O sistema deve reduzir improvisação sem criar rigidez artificial.

O passado deve ser condensado em sistema, não reaprendido indefinidamente.

A estrutura serve ao conteúdo.

O agente herda antes de criar.

O patch deve ser proporcional ao defeito.

O arquivo congelado permanece preservado.

Quando as fontes vigentes resolvem a tarefa, execute.

Quando a decisão ultrapassa a autorização ou altera o sistema, pare e peça orientação.
