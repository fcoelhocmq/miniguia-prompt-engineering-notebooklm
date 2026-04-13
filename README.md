# 🧠 Caderno Temático: Engenharia de Prompts — Da Teoria à Prática

> Projeto desenvolvido como parte do desafio prático da [DIO](https://www.dio.me/), utilizando o **NotebookLM do Google** como ferramenta de aprendizagem ativa com Inteligência Artificial.

---

## 📌 Contexto e Objetivos

### Por que Engenharia de Prompts?

A Engenharia de Prompts é uma das habilidades mais valorizadas no mercado de tecnologia atualmente. Saber "conversar" com modelos de linguagem de forma estratégica determina a qualidade dos resultados obtidos — seja para geração de código, análise de dados, criação de conteúdo ou automação de tarefas.

Este caderno temático foi criado com o objetivo de **construir uma base sólida sobre Engenharia de Prompts**, partindo do zero e chegando à aplicação prática de técnicas reconhecidas pelo mercado.

### 🎯 Objetivos de Estudo

- [ ] Compreender o que é Engenharia de Prompts e por que ela importa
- [ ] Conhecer os principais tipos e técnicas de prompts (Zero-shot, Few-shot, Chain-of-Thought etc.)
- [ ] Identificar boas práticas para estruturar prompts eficazes
- [ ] Entender como diferentes modelos de linguagem respondem a variações de prompts
- [ ] Criar um banco de prompts reutilizáveis para estudo e trabalho

---

## 📚 Curadoria de Fontes

As fontes abaixo foram selecionadas por serem abertas, confiáveis e adequadas para iniciantes. Todas foram carregadas no **NotebookLM** para análise e geração do material de estudo.

| # | Fonte | Tipo | Link |
|---|-------|------|------|
| 1 | **Prompt Engineering Guide** — DAIR.AI | Documentação Web | [promptingguide.ai](https://www.promptingguide.ai/pt) |
| 2 | **OpenAI — Prompt Engineering Best Practices** | Artigo Oficial | [platform.openai.com/docs/guides/prompt-engineering](https://platform.openai.com/docs/guides/prompt-engineering) |
| 3 | **Learn Prompting** — Guia Comunitário Open Source | Documentação Web | [learnprompting.org](https://learnprompting.org/pt/docs/intro) |
| 4 | **Anthropic — Introduction to Prompt Design** | Documentação Oficial | [docs.anthropic.com](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview) |
| 5 | **Artigo: Chain-of-Thought Prompting Elicits Reasoning in LLMs** — Google Brain (2022) | Paper Científico (PDF) | [arxiv.org/abs/2201.11903](https://arxiv.org/abs/2201.11903) |

> 💡 **Como usar:** Acesse o [NotebookLM](https://notebooklm.google.com), crie um novo caderno e faça o upload ou cole os links acima como fontes.

---

## 🧪 Engenharia de Prompts e "Cicatrizes" de Aprendizado

Esta seção documenta as perguntas estratégicas testadas no NotebookLM, os prompts utilizados, as respostas obtidas e as dificuldades encontradas ao longo do processo.

---

### 🔹 Sessão 1 — Entendendo o Conceito Base

**🎯 Objetivo:** Obter uma definição clara e didática de Engenharia de Prompts para iniciantes.

**Prompt Testado (v1 — vago):**
```
O que é engenharia de prompts?
```

**Resultado real obtido:**
> *"A engenharia de prompts (EP) pode ser definida como o campo de estudo voltado a aprender como falar com uma inteligência artificial para conseguir o que se deseja. Trata-se de uma disciplina relativamente nova que busca desenvolver e otimizar prompts para utilizar modelos de linguagem (LMs) de maneira eficiente em diversas aplicações e tópicos de pesquisa."*
> 
> A resposta detalhou quatro aspectos: Interação e Desenvolvimento, Melhoria de Desempenho, Segurança e Confiabilidade, e Prática Profissional. Também mencionou técnicas como Role Prompting e Chain-of-Thought.

**🔄 Revisão da hipótese inicial:** Ao contrário do que eu esperava, o NotebookLM **aproveitou bem as fontes** mesmo com um prompt curto, entregando uma resposta estruturada e embasada. Isso mostra que o NotebookLM tem um comportamento diferente de outros LLMs: como as fontes estão fixadas no caderno, ele as consulta por padrão, mesmo sem instrução explícita.

**⚠️ Limitação real observada:** A resposta, embora correta e bem estruturada, **não indicou de qual fonte específica** cada trecho foi extraído. Para fins acadêmicos ou de estudo aprofundado, isso pode ser insuficiente. A solução é refinar o prompt pedindo citações explícitas — o que foi testado na versão v2 abaixo.

**💡 Aprendizado real:** Prompts simples no NotebookLM já geram respostas razoáveis. O refinamento do prompt não é sobre "forçar a IA a usar as fontes", mas sobre **controlar o formato, a profundidade e a rastreabilidade das referências**.

---

**Prompt Testado (v2 — refinado com contexto):**
```
Com base nas fontes do meu caderno, explique o que é Engenharia de Prompts 
para alguém que nunca teve contato com o assunto. Use uma linguagem simples, 
com exemplos práticos do dia a dia e destaque por que essa habilidade é 
importante no mercado de trabalho atual.
```

**✅ Resultado real obtido:**
A IA entregou uma explicação em camadas progressivas de complexidade:

> *"Imagine que a inteligência artificial (IA) é um assistente extremamente inteligente e capaz, mas que não consegue ler sua mente. Para que ele entregue um bom resultado, você precisa dar as instruções corretas."*

A resposta incluiu **4 exemplos práticos do cotidiano** (e-mails, resumos de textos, estudo e criação de imagens) e **4 razões de mercado** organizadas numericamente: aumento de eficiência, melhores resultados, entendimento da tecnologia e resolução de problemas complexos. Encerrou com uma metáfora de alto impacto: *"dominar a engenharia de prompts é como aprender um novo idioma"*.

**🔄 Comparação direta: v1 vs v2**

| Critério | v1 — Prompt simples | v2 — Prompt refinado |
|----------|--------------------|--------------------|
| Tom | Técnico e formal | Acessível para iniciantes |
| Exemplos | Mencionados superficialmente | 4 exemplos concretos do dia a dia |
| Estrutura | Lista de aspectos técnicos | Narrativa com analogia + listas |
| Apelo ao mercado | Citado genericamente | 4 razões práticas e numeradas |
| Memorabilidade | Baixa | Alta (metáfora do "novo idioma") |

**💡 Aprendizado confirmado:** Especificar o **público-alvo** ("alguém que nunca teve contato"), o **tom desejado** ("linguagem simples") e o **objetivo final** ("exemplos do dia a dia + importância no mercado") transformou a resposta de um verbete técnico em um texto que qualquer pessoa consegue ler e reter. O mesmo conteúdo das fontes, extraído de formas completamente diferentes.

---

### 🔹 Sessão 2 — Mapeando as Técnicas Principais

**🎯 Objetivo:** Criar uma visão geral das principais técnicas de prompting.

**Prompt Testado:**
```
Com base nas minhas fontes, liste as principais técnicas de Engenharia de Prompts 
em ordem de complexidade, do mais simples ao mais avançado. Para cada técnica, 
forneça: nome, descrição em 2 linhas e um exemplo de uso prático.
```

**✅ Resultado real obtido:**
O NotebookLM gerou **6 técnicas em ordem crescente de complexidade**, com descrição e exemplo prático para cada uma:

| # | Técnica | Nível |
|---|---------|-------|
| 1 | Zero-shot Prompting | Básico |
| 2 | Role Prompting | Básico-Intermediário |
| 3 | Few-shot Prompting | Intermediário |
| 4 | Chain-of-Thought | Intermediário |
| 5 | Prompt Chaining | Avançado |
| 6 | RAG (Retrieval Augmented Generation) | Avançado |

Destaque para o exemplo de **Prompt Chaining** gerado: primeiro extrair pontos-chave de um relatório, depois usar esse output para redigir um e-mail à diretoria — mostrando na prática como encadear prompts em fluxos reais de trabalho.

**🔄 Diferença em relação ao esperado:** A lista não incluiu *Tree of Thought* nem *ReAct*. Em vez disso, o NotebookLM trouxe **RAG**, mais aplicado e relevante para contextos profissionais — mas que tecnicamente não é uma técnica de prompting puro, e sim uma arquitetura de sistema. O modelo não fez essa distinção por conta própria.

**⚠️ Cicatriz registrada:** Para evitar essa mistura em contextos acadêmicos, seria necessário refinar o prompt com: *"considere apenas técnicas aplicadas diretamente no prompt, sem alterações de arquitetura ou retreinamento do modelo"*.

**💡 Aprendizado:** Pedir ordenação por complexidade ("do mais simples ao mais avançado") é uma estratégia poderosa — força o modelo a organizar o conteúdo de forma pedagogicamente útil, ideal para quem está aprendendo progressivamente.

---

### 🔹 Sessão 3 — Aplicação Prática com Chain-of-Thought

**🎯 Objetivo:** Entender na prática como o Chain-of-Thought (CoT) funciona.

**Prompt Testado:**
```
Explique o que é Chain-of-Thought Prompting com base no paper científico 
das minhas fontes. Depois, me dê um exemplo comparativo: primeiro resolvendo 
um problema SEM CoT e depois COM CoT, para eu visualizar a diferença.
```

**✅ Resultado real obtido:**
O NotebookLM citou diretamente o paper de **Jason Wei et al.** e explicou que o CoT:

> *"explora a capacidade dos modelos de linguagem de gerar uma série de etapas intermediárias de raciocínio antes de chegar a uma resposta final"*

Dois pontos técnicos importantes foram destacados pelas fontes: (1) o CoT **surge naturalmente com o aumento do tamanho do modelo** — modelos menores não se beneficiam da técnica; (2) pode ser ativado apenas adicionando *"Pense passo a passo"* ao final do prompt (técnica chamada de **Zero-shot CoT**).

**Exemplo comparativo gerado — mesmo problema, dois formatos:**

| | Sem CoT | Com CoT |
|--|---------|---------|
| **Prompt** | "João tem 5 maçãs, compra 2 sacos com 6 cada. Total?" | Mesma pergunta + *"Pense passo a passo."* |
| **Resposta** | "João ficou com 17 maçãs." | Etapa 1 → 2 → 3 → resposta final: 17 |
| **Risco** | Em problemas complexos, a IA pode "alucicar" o resultado | Cada etapa pode ser verificada individualmente |

A resposta deixou claro que **o resultado numérico foi idêntico** nos dois casos (17 maçãs) — mas o CoT adiciona **rastreabilidade e verificabilidade**, o que é especialmente valioso para evitar alucinações em problemas mais complexos.

**⚠️ Nuance registrada:** Para problemas simples, o CoT não muda o resultado — apenas o caminho. O real ganho aparece em cálculos encadeados, lógica simbólica e problemas de múltiplas etapas onde a IA sem CoT tende a "pular" partes cruciais.

**💡 Aprendizado confirmado:** Pedir exemplos **comparativos** (sem X vs. com X) é uma das estratégias mais eficazes para consolidar conceitos novos — você vê a diferença na prática, não apenas na teoria. A simples adição de *"Pense passo a passo"* ao final de um prompt já ativa o comportamento de CoT.

---

### 🔹 Sessão 4 — Geração do Glossário

**Prompt Testado:**
```
Com base em todas as minhas fontes, crie um glossário com os 15 termos técnicos 
mais importantes relacionados à Engenharia de Prompts. Para cada termo, escreva 
uma definição curta (máximo 3 linhas) em português, adequada para iniciantes.
Organize em ordem alfabética.
```

**✅ Resultado real obtido:**
O NotebookLM gerou os 15 termos em ordem alfabética, todos em português, com linguagem acessível para iniciantes. O glossário cobriu não apenas técnicas de prompting, mas também **conceitos de segurança** que não foram explicitamente solicitados — como Adversarial Prompting, Prompt Injection, Jailbreaking e Prompt Leaking.

**🔄 Surpresa positiva:** A IA expandiu o escopo de forma inteligente. Sem pedir, ela identificou que segurança em prompts é um tema relevante nas fontes e o incluiu no glossário. Isso enriqueceu o material de estudo.

**⚠️ Ponto de atenção:** 4 dos 15 termos são sobre ataques e vulnerabilidades (Adversarial Prompting, Prompt Injection, Jailbreaking, Prompt Leaking). Para um glossário puramente técnico de uso profissional, pode ser necessário separar em duas seções: *Técnicas* e *Segurança*. Refinamento sugerido: adicionar ao prompt *"separe os termos em categorias: Técnicas de Prompting e Segurança/Ataques"*.

**💡 Aprendizado:** Pedir organização em ordem alfabética + limite de linhas por definição é uma combinação eficaz para gerar materiais de referência rápida. O glossário gerado está diretamente aproveitado na seção do Miniguia abaixo.

---

### 🔹 Sessão 5 — Geração do Podcast de Revisão (Funcionalidade Audio Overview)

**Experimento:** Utilizei a funcionalidade **"Audio Overview"** do NotebookLM para gerar um podcast de revisão sobre o conteúdo do caderno.

> 🎙️ *Arquivo gerado: `A_mecânica_real_da_engenharia_de_prompt.m4a`*

**✅ Resultado real obtido:**
O podcast de **~21 minutos** cobriu os principais conceitos em formato conversacional entre dois apresentadores simulados — um fazendo perguntas e o outro respondendo, simulando uma entrevista de divulgação técnica. O áudio percorreu desde a definição de Engenharia de Prompts até técnicas como Chain-of-Thought e boas práticas de uso profissional.

O formato é excelente para **revisão passiva**: é possível absorver o conteúdo enquanto se realiza outra atividade (transporte, exercício, tarefas domésticas).

**🔄 Diferença em relação ao estimado:** A duração real foi de **~21 minutos** — significativamente maior que os ~8 minutos estimados inicialmente. Isso indica que o NotebookLM gerou uma cobertura mais abrangente do que o esperado, provavelmente por conta do volume de conteúdo das 5 fontes carregadas.

**⚠️ Limitação observada:** O áudio é gerado em **inglês por padrão**. Para obter o podcast em português, é necessário instruir o NotebookLM explicitamente no campo de customização antes de gerar — por exemplo: *"Gere o podcast inteiramente em português brasileiro, com linguagem acessível para iniciantes."*

**💡 Aprendizado:** O Audio Overview funciona melhor como ferramenta de **revisão**, não de primeiro contato. Recomenda-se usá-lo após já ter lido as fontes e feito as sessões de perguntas — assim o ouvido reconhece os conceitos e a retenção é maior. Para estudantes com rotina corrida, é um diferencial real de produtividade.


---

## 📖 Miniguia de Estudo — Entrega Final

### 📝 Resumos Estruturados

#### 1. O que é Engenharia de Prompts?

Engenharia de Prompts é a prática de **projetar e otimizar instruções (prompts)** enviadas a modelos de linguagem (LLMs) para obter respostas mais precisas, úteis e alinhadas ao objetivo desejado. É uma habilidade que combina clareza de comunicação, conhecimento sobre como os modelos funcionam e pensamento iterativo.

Não se trata de "truques mágicos", mas de uma disciplina com princípios claros: contexto, especificidade, estrutura e iteração.

---

#### 2. Anatomia de um Bom Prompt

Um prompt eficaz geralmente contém alguns ou todos os elementos abaixo:

| Elemento | Descrição | Exemplo |
|----------|-----------|---------|
| **Papel/Persona** | Define quem a IA deve ser | *"Você é um professor de programação..."* |
| **Contexto** | Fornece informações de fundo | *"Estou aprendendo Python pela primeira vez..."* |
| **Tarefa** | O que exatamente deve ser feito | *"Explique o conceito de listas..."* |
| **Formato** | Como a resposta deve ser estruturada | *"Use bullet points e exemplos de código..."* |
| **Restrições** | O que evitar ou limitar | *"Em no máximo 200 palavras..."* |

---

#### 3. Principais Técnicas de Prompting

**🔵 Zero-shot Prompting**
Faz uma pergunta diretamente sem fornecer exemplos. Funciona bem para tarefas simples e modelos mais poderosos.
```
Traduza para o inglês: "O gato está em cima do telhado."
```

**🟢 Few-shot Prompting**
Fornece 2 a 5 exemplos antes da tarefa real, guiando o modelo sobre o padrão esperado.
```
Positivo: "Adorei o produto!" → Sentimento: Positivo
Negativo: "Péssimo atendimento." → Sentimento: Negativo
Neutro: "O produto chegou." → Sentimento: ???
```

**🟠 Chain-of-Thought (CoT)**
Instrui o modelo a "pensar em voz alta", decompondo o raciocínio em etapas antes de dar a resposta final. Ideal para problemas complexos.
```
Resolva passo a passo: Se João tem 3 caixas com 8 maçãs cada, 
e dá 10 maçãs para Maria, quantas maçãs ficam com João?
```

**🔴 Role Prompting**
Atribui uma persona específica ao modelo para moldar o estilo e profundidade da resposta.
```
Você é um especialista em cibersegurança com 15 anos de experiência. 
Explique o que é phishing para um usuário leigo.
```

**🟣 Tree of Thought (ToT)**
Técnica avançada onde o modelo explora múltiplos caminhos de raciocínio simultaneamente antes de convergir para a melhor resposta.

---

#### 4. Boas Práticas Essenciais

- ✅ **Seja específico**: quanto mais contexto, melhor a resposta
- ✅ **Use delimitadores**: separe partes do prompt com `###`, `""" """` ou `[ ]`
- ✅ **Itere**: raramente o primeiro prompt é o melhor
- ✅ **Defina o formato de saída**: peça JSON, tabela, lista, parágrafo etc.
- ✅ **Teste variações**: pequenas mudanças de palavra podem gerar resultados muito diferentes
- ❌ **Evite ambiguidade**: instruções vagas geram respostas vagas
- ❌ **Evite prompts negativos isolados**: prefira dizer o que quer, não só o que não quer

---

### 📘 Glossário de Conceitos-Chave

> ✅ *Gerado diretamente pelo NotebookLM na Sessão 4, a partir das fontes do caderno. 15 termos em ordem alfabética.*

#### 🔵 Técnicas e Conceitos Fundamentais

| Termo | Definição |
|-------|-----------|
| **Cadeia de Pensamento (Chain-of-Thought)** | Técnica que incentiva a IA a mostrar o raciocínio passo a passo antes de chegar à conclusão final, melhorando o desempenho em tarefas lógicas. |
| **Encadeamento de Prompts (Prompt Chaining)** | Processo de dividir uma tarefa complexa em várias etapas menores, onde o resultado de um comando é usado como entrada para o comando seguinte. |
| **Engenharia de Prompts** | Campo de estudo focado em desenvolver, otimizar e refinar comandos para utilizar modelos de linguagem de maneira eficiente e produtiva. |
| **Few-shot Prompting** | Método que consiste em fornecer ao modelo alguns exemplos práticos de como realizar uma tarefa antes de pedir que ele execute o comando final. |
| **Grandes Modelos de Linguagem (LLMs)** | Sistemas de IA treinados com volumes gigantescos de texto para entender, processar e gerar linguagem humana natural. |
| **Prompt** | O texto, pergunta ou instrução inicial que você envia para o modelo de IA para orientar o que ele deve gerar como resposta. |
| **Prompt de Sistema (System Prompt)** | Instrução de alto nível que define a personalidade, as regras básicas e o comportamento geral que a IA deve adotar durante toda a conversa. |
| **Prompting de Atuação (Role Prompting)** | Técnica de atribuir um papel ou cargo específico à IA, como pedir para ela agir como um "professor de história" ou "recrutador". |
| **RAG (Retrieval Augmented Generation)** | Método que permite que a IA consulte bases de conhecimento externas e específicas para fornecer respostas mais precisas e atualizadas. |
| **Zero-shot Prompting** | Consiste em dar uma ordem direta à IA sem fornecer nenhum exemplo anterior, esperando que ela resolva a tarefa apenas com seu conhecimento prévio. |

#### 🔴 Segurança e Vulnerabilidades

| Termo | Definição |
|-------|-----------|
| **Adversarial Prompting** | Técnicas de ataque que tentam enganar o modelo para que ele ignore suas instruções originais ou gere respostas perigosas e inadequadas. |
| **Alucinação (Hallucination)** | Ocorre quando a IA gera informações que parecem convincentes e corretas, mas que são, na verdade, inventadas ou factualmente erradas. |
| **Injeção de Prompt (Prompt Injection)** | Ataque onde o usuário insere comandos maliciosos para tentar "sequestrar" ou mudar o comportamento original definido para a IA. |
| **Jailbreaking** | Tentativa deliberada de contornar as regras de segurança e os filtros da IA para fazê-la responder a perguntas proibidas ou realizar tarefas restritas. |
| **Vazamento de Prompt (Prompt Leaking)** | Ataque que tenta forçar a IA a revelar suas instruções internas e secretas que não deveriam ser vistas pelo usuário final. |

---

### 🔁 Banco de Prompts Reutilizáveis

Estes prompts foram testados e podem ser reutilizados para futuras sessões de estudo sobre qualquer tema.

#### 📌 Para Aprender um Novo Conceito
```
Você é um professor especialista em [TEMA]. Explique o conceito de [CONCEITO] 
para um iniciante absoluto, usando: 
1) Uma analogia do cotidiano
2) Uma definição técnica simples
3) Um exemplo prático real
```

#### 📌 Para Criar Resumos de Documentos
```
Com base nas fontes do meu caderno, crie um resumo estruturado sobre [TEMA] 
contendo: introdução (2 parágrafos), pontos principais (em tópicos) e 
conclusão com os 3 aprendizados mais importantes.
```

#### 📌 Para Gerar Questões de Revisão
```
Crie 10 perguntas de revisão sobre [TEMA] em níveis progressivos de dificuldade:
- 3 perguntas de nível básico (conceitos fundamentais)
- 4 perguntas de nível intermediário (aplicação)
- 3 perguntas de nível avançado (análise e síntese)
Inclua as respostas ao final.
```

#### 📌 Para Comparar Conceitos
```
Compare [CONCEITO A] e [CONCEITO B] usando uma tabela com as seguintes colunas:
Definição, Quando usar, Vantagens, Limitações e Exemplo prático.
Base sua resposta nas fontes do meu caderno.
```

#### 📌 Para Troubleshooting de Prompts
```
O prompt abaixo não está gerando bons resultados:
[COLE SEU PROMPT AQUI]

Analise os problemas e reescreva em uma versão melhorada, explicando 
o que foi mudado e por quê.
```

#### 📌 Para Criar um Plano de Estudos
```
Com base no conteúdo das minhas fontes sobre [TEMA], crie um plano de estudos 
para 4 semanas, com dedicação de [X horas] por semana. Inclua: objetivos semanais, 
recursos sugeridos das fontes e uma atividade prática por semana.
```

---

## 🛠️ Stack e Ferramentas Utilizadas

- **[NotebookLM](https://notebooklm.google.com)** — Plataforma principal de estudo com IA
- **[GitHub](https://github.com)** — Repositório e portfólio do projeto
- **Markdown** — Formatação da documentação

---

## 🚀 Como Reproduzir Este Projeto

1. Acesse o [NotebookLM](https://notebooklm.google.com) com sua conta Google
2. Clique em **"New Notebook"** e dê o nome: `Engenharia de Prompts - Da Teoria à Prática`
3. Adicione as 5 fontes listadas na seção de Curadoria (via link ou upload de PDF)
4. Aguarde o NotebookLM processar as fontes
5. Utilize os prompts da seção **"Engenharia de Prompts e Cicatrizes"** como ponto de partida
6. Explore a funcionalidade **"Audio Overview"** para gerar um podcast de revisão
7. Documente seus próprios aprendizados e dificuldades!

---

## 📈 Próximos Passos

- [ ] Estudar técnicas avançadas: Tree of Thought e ReAct
- [ ] Criar prompts específicos para área de Dados
- [ ] Explorar Prompt Injection e questões de segurança
- [ ] Desenvolver um prompt template para projetos profissionais reais

---

## 🤝 Contribuições

Este é um projeto de aprendizado pessoal, mas sugestões são bem-vindas! Abra uma *issue* ou envie um *pull request*.

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

<div align="center">

**Feito com 🧠 e ☕ como parte do desafio prático da [DIO](https://www.dio.me/)**

*"A qualidade de suas perguntas determina a qualidade das suas respostas."*

</div>
