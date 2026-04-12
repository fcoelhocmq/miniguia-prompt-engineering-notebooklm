# 🧠 Miniguia de Estudos: Engenharia de Prompts com NotebookLM
> **Desafio de Projeto — DIO | Explorando IA como Ferramenta de Aprendizagem Ativa**
## 📌 Contexto e Objetivos
### Tema Escolhido: **Engenharia de Prompts — Da Teoria à Prática**

A Engenharia de Prompts é hoje uma das habilidades mais valorizadas no mercado de tecnologia. Com o crescimento acelerado de modelos de linguagem como GPT-4, Claude e Gemini, saber *como* formular perguntas e instruções para esses sistemas tornou-se um diferencial competitivo real.
Escolhi este tema por acreditar que compreender os fundamentos de Prompt Engineering permite não apenas usar a IA de forma mais eficiente, mas também entender seus limites, vieses e o raciocínio por trás das respostas geradas.

### Objetivos de Estudo
- Compreender os principais padrões e técnicas de Engenharia de Prompts (Zero-Shot, Few-Shot, Chain-of-Thought, etc.)
- Aprender a estruturar prompts para diferentes casos de uso: geração de código, análise de textos, tutoriais e resolução de problemas
- Identificar boas práticas e armadilhas comuns ao interagir com LLMs
- Criar um conjunto de prompts reutilizáveis para revisões futuras
- Documentar o processo de aprendizagem com IA como metodologia replicável

## 📚 Curadoria de Fontes

As fontes abaixo foram selecionadas por serem **abertas, acadêmicas ou técnicas** e estarem disponíveis publicamente. Todas foram inseridas no NotebookLM para análise.

| # | Título | Tipo | Link |
|---|--------|------|------|
| 1 | **Prompt Engineering Guide** — DAIR.AI | Guia Web/PDF | [promptingguide.ai](https://www.promptingguide.ai/) |
| 2 | **Chain-of-Thought Prompting Elicits Reasoning in Large Language Models** — Wei et al. (2022) | Artigo Científico (PDF) | [arxiv.org/abs/2201.11903](https://arxiv.org/abs/2201.11903) |
| 3 | **Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in NLP** — Liu et al. (2023) | Artigo Científico (PDF) | [arxiv.org/abs/2107.13586](https://arxiv.org/abs/2107.13586) |
| 4 | **OpenAI Prompt Engineering Best Practices** | Documentação Técnica | [platform.openai.com/docs/guides/prompt-engineering](https://platform.openai.com/docs/guides/prompt-engineering) |
| 5 | **Large Language Models are Zero-Shot Reasoners** — Kojima et al. (2022) | Artigo Científico (PDF) | [arxiv.org/abs/2205.11916](https://arxiv.org/abs/2205.11916) |

> 💡 **Critério de curadoria:** priorizei fontes com alto número de citações, publicadas por instituições reconhecidas ou por empresas que desenvolvem os próprios LLMs, garantindo confiabilidade e profundidade técnica.

## 🛠️ Engenharia de Prompts & "Cicatrizes" de Aprendizado

Esta seção documenta as perguntas estratégicas, variações de prompts testados e as dificuldades encontradas durante a exploração do material no NotebookLM.

### 🔍 Sessão 1 — Mapeamento Inicial do Conteúdo

**Prompt inicial (exploração ampla):**
Quais são os principais conceitos abordados nas fontes que eu carreguei? 
Faça um resumo em tópicos hierárquicos.

**Resultado:** O NotebookLM 
As fontes fornecidas exploram a Engenharia de Prompt como uma disciplina essencial para o desenvolvimento, otimização e compreensão das capacidades dos Modelos de Linguagem Grandes (LLMs).
Ele fez um resumo dos principais conceitos abordados, organizados em tópicos hierárquicos:


**⚠️ Dificuldade encontrada:** A resposta era genérica demais. Não havia distinção clara entre os documentos.

**Prompt refinado (com âncora de fonte):**
Com base APENAS no artigo de Wei et al. (2022) sobre Chain-of-Thought, 
explique o que é essa técnica, qual problema ela resolve e quais foram 
os principais experimentos realizados pelos autores.

**✅ Resultado melhorado:** A resposta ficou focada, com referências diretas ao paper, mencionando os benchmarks utilizados (GSM8K, SVAMP) e o ganho percentual de performance demonstrado pelos autores.

**💡 Lição aprendida:** Ancorar o prompt em uma fonte específica aumenta a precisão e a rastreabilidade das respostas.


### 🔍 Sessão 2 — Aprofundamento Técnico

**Prompt (comparação entre técnicas):**
Compare as técnicas Zero-Shot, Few-Shot e Chain-of-Thought Prompting. 
Apresente: definição, quando usar, vantagens e limitações de cada uma. 
Use o formato de tabela comparativa.

**✅ Resultado:** Excelente tabela comparativa com distinções claras. O NotebookLM cruzou os artigos de Wei et al. e Kojima et al. de forma coerente.

**⚠️ Dificuldade encontrada:** O modelo inseriu uma informação sobre "Self-Consistency Prompting" sem que eu tivesse pedido, e sem indicar a fonte. Precisei verificar manualmente se o conceito estava presente nos documentos carregados.

**Prompt de verificação (troubleshooting):**
A técnica "Self-Consistency" foi mencionada em algum dos documentos 
que eu carreguei? Se sim, em qual deles e em qual contexto?

**✅ Resultado:** O NotebookLM confirmou que o conceito aparecia de forma marginal no survey de Liu et al., mas não era o foco de nenhum dos papers. Isso me ensinou a sempre questionar informações não solicitadas.

### 🔍 Sessão 3 — Geração de Material de Estudo

**Prompt (geração de quiz):**
Com base nos documentos, crie 5 perguntas de múltipla escolha sobre 
Engenharia de Prompts, com 4 alternativas cada, indicando a resposta 
correta e a justificativa baseada nas fontes.
**✅ Resultado:** Quiz de alta qualidade com justificativas rastreáveis. Útil para revisão ativa.

**⚠️ Dificuldade encontrada:** Duas perguntas tinham alternativas ambíguas — a IA não conseguiu criar distratores (alternativas erradas) suficientemente plausíveis. Precisei pedir uma revisão.

**Prompt de refinamento:**
As perguntas 2 e 4 têm alternativas incorretas muito óbvias. 
Reescreva-as com distratores mais plausíveis, baseados em 
confusões conceituais comuns que um estudante iniciante cometeria.

**✅ Resultado após refinamento:** Muito melhor. As alternativas erradas passaram a exigir real compreensão do tema para serem descartadas.

### 🔍 Sessão 4 — Síntese e Glossário

**Prompt:**
Liste os 15 termos técnicos mais importantes presentes nos documentos. 
Para cada um, forneça: (1) definição em até 3 linhas, (2) exemplo prático 
de uso e (3) referência ao documento de origem.

**✅ Resultado:** Base do glossário desta entrega. Excelente para consolidação do vocabulário técnico.


## 📖 Miniguia de Estudo — Entrega Final

### 📋 Resumos Estruturados

#### 1. O que é Engenharia de Prompts?
Engenharia de Prompts é a prática de projetar e refinar as entradas (inputs) fornecidas a modelos de linguagem de grande escala (LLMs) com o objetivo de obter outputs mais precisos, relevantes e úteis. Não se trata apenas de "fazer perguntas melhores" — é uma disciplina que combina conhecimento sobre o funcionamento dos modelos, o domínio do problema em questão e técnicas estruturadas de comunicação.

#### 2. Técnicas Fundamentais

**Zero-Shot Prompting**
Solicitar ao modelo que execute uma tarefa sem fornecer exemplos. Funciona bem para tarefas simples e quando o modelo já foi treinado extensivamente no domínio. Limitação: falha em tarefas que exigem raciocínio encadeado.

**Few-Shot Prompting**
Fornecer de 2 a 5 exemplos do comportamento desejado antes da instrução principal. Melhora significativamente a performance em tarefas que exigem formato específico ou padrão de resposta. Custo: aumenta o tamanho do contexto.

**Chain-of-Thought (CoT) Prompting**
Técnica introduzida por Wei et al. (2022) que instrui o modelo a "pensar passo a passo" antes de dar a resposta final. Demonstrou ganhos expressivos em benchmarks de raciocínio matemático e lógico. Pode ser combinada com Few-Shot para resultados ainda melhores.

**Zero-Shot CoT**
Variante do CoT proposta por Kojima et al. (2022): basta adicionar a frase *"Let's think step by step"* ao final do prompt. Surpreendentemente eficaz, sem necessidade de exemplos.

**Role Prompting**
Atribuir uma persona ou papel ao modelo antes da tarefa ("Você é um especialista em segurança da informação..."). Altera o tom, vocabulário e profundidade das respostas.

#### 3. Boas Práticas

- **Seja específico:** prompts vagos geram respostas vagas. Detalhe o formato, extensão e perspectiva desejados.
- **Itere:** raramente o primeiro prompt é o melhor. Documente variações e resultados.
- **Âncora em fontes:** ao usar ferramentas como NotebookLM, especifique de qual documento quer a informação.
- **Verifique informações não solicitadas:** o modelo pode "alucinar" dados que parecem plausíveis mas não estão nas fontes.
- **Use delimitadores:** separe instruções de contexto com marcadores como `###`, `---` ou tags XML.

#### 4. Limitações Importantes

- LLMs não "sabem" — eles *predizem*. Respostas confiantes podem estar erradas.
- A performance varia significativamente entre modelos diferentes para o mesmo prompt.
- Prompts eficazes para um modelo podem falhar em outro.
- O viés das fontes de treinamento influencia as respostas.

### 📚 Glossário de Conceitos

| Termo | Definição | Origem |
|-------|-----------|--------|
| **LLM (Large Language Model)** | Modelo de linguagem treinado em grandes volumes de texto, capaz de gerar, resumir e transformar linguagem natural | Liu et al. (2023) |
| **Prompt** | Entrada de texto fornecida ao modelo para orientar sua resposta | DAIR.AI Guide |
| **Zero-Shot** | Solicitação sem exemplos prévios; o modelo executa a tarefa apenas com a instrução | Kojima et al. (2022) |
| **Few-Shot** | Técnica que fornece exemplos da tarefa no próprio prompt para guiar o comportamento do modelo | Wei et al. (2022) |
| **Chain-of-Thought (CoT)** | Estratégia que induz o modelo a externalizar etapas de raciocínio antes da resposta final | Wei et al. (2022) |
| **Token** | Unidade básica de processamento dos LLMs; aproximadamente ¾ de uma palavra em inglês | OpenAI Docs |
| **Context Window** | Limite máximo de tokens que o modelo pode processar em uma única interação | OpenAI Docs |
| **Hallucination** | Fenômeno onde o modelo gera informações plausíveis mas incorretas ou inventadas | Liu et al. (2023) |
| **Temperature** | Parâmetro que controla a aleatoriedade das respostas; valores altos = mais criatividade, baixos = mais determinismo | OpenAI Docs |
| **System Prompt** | Instrução inicial que define o comportamento, persona ou restrições do modelo para toda a conversa | OpenAI Docs |
| **Role Prompting** | Técnica de atribuir um papel ou persona ao modelo para direcionar o estilo e profundidade das respostas | DAIR.AI Guide |
| **Distrator** | Alternativa incorreta em questões de múltipla escolha, usada para testar compreensão real | — |
| **Benchmark** | Conjunto de tarefas padronizadas usado para avaliar e comparar a performance de modelos de IA | Wei et al. (2022) |
| **RAG (Retrieval-Augmented Generation)** | Técnica que combina busca em documentos externos com geração de linguagem para respostas mais factuais | Liu et al. (2023) |
| **In-Context Learning** | Capacidade dos LLMs de aprender padrões a partir de exemplos fornecidos no próprio prompt, sem retreinamento | Liu et al. (2023) |

### 🔁 Prompts Reutilizáveis

Coleção de prompts testados e validados, prontos para reutilização em sessões futuras de estudo.

**🗺️ Mapeamento de conteúdo de um documento específico**
Com base no documento [NOME DO DOCUMENTO], identifique:
1. Os 5 conceitos centrais abordados
2. A tese ou argumento principal dos autores
3. As metodologias ou experimentos utilizados
4. As principais conclusões e limitações reconhecidas pelos autores

**📊 Tabela comparativa entre conceitos**
Compare [CONCEITO A] e [CONCEITO B] considerando:
- Definição
- Casos de uso ideais
- Vantagens
- Limitações
- Exemplo prático

Apresente no formato de tabela.

**❓ Geração de quiz para revisão ativa**
Com base nas fontes carregadas, crie [N] perguntas de múltipla escolha sobre [TEMA].
Cada pergunta deve ter:
- 4 alternativas (A, B, C, D)
- Alternativas incorretas plausíveis baseadas em confusões conceituais comuns
- Indicação da resposta correta
- Justificativa com referência ao documento de origem

**📖 Geração de glossário temático**
Liste os [N] termos técnicos mais importantes sobre [TEMA] presentes nos documentos.
Para cada termo, forneça:
1. Definição objetiva (máximo 3 linhas)
2. Exemplo prático de aplicação
3. Documento de origem da definição

**🔍 Verificação de fonte de uma informação**
A afirmação "[AFIRMAÇÃO]" está presente em algum dos documentos carregados?
Se sim: em qual documento, em qual contexto e com quais nuances?
Se não: indique que a informação não consta nas fontes disponíveis.

**🧩 Síntese integrativa entre múltiplas fontes**
Com base em TODOS os documentos carregados, elabore uma síntese sobre [TEMA] que:
- Identifique pontos de convergência entre os autores
- Destaque contradições ou perspectivas divergentes
- Indique lacunas que os documentos não cobrem
- Sugira perguntas abertas para aprofundamento futuro

**📝 Criação de resumo executivo**
Crie um resumo executivo do documento [NOME] com:
- 1 parágrafo de contexto (por que esse documento importa)
- Principais argumentos em bullet points (máximo 7)
- Citação direta mais relevante do documento
- 1 parágrafo com minha opinião crítica sobre o conteúdo

## 🏁 Conclusão

Este projeto me permitiu experimentar o NotebookLM não como uma ferramenta de busca passiva, mas como um **parceiro de aprendizagem ativa**. A maior lição foi entender que a qualidade do output depende diretamente da qualidade do input — e que documentar as iterações (incluindo os erros) é tão valioso quanto o resultado final.

A Engenharia de Prompts é, paradoxalmente, um tema ideal para estudar *usando* Engenharia de Prompts: cada sessão no NotebookLM foi, ela mesma, um experimento prático dos conceitos estudados.

## 🔗 Referências Completas

1. DAIR.AI. *Prompt Engineering Guide*. Disponível em: https://www.promptingguide.ai/
2. WEI, Jason et al. *Chain-of-Thought Prompting Elicits Reasoning in Large Language Models*. arXiv:2201.11903, 2022.
3. LIU, Pengfei et al. *Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in NLP*. arXiv:2107.13586, 2023.
4. OPENAI. *Prompt Engineering Best Practices*. Disponível em: https://platform.openai.com/docs/guides/prompt-engineering
5. KOJIMA, Takeshi et al. *Large Language Models are Zero-Shot Reasoners*. arXiv:2205.11916, 2022.

*Projeto desenvolvido como parte do desafio prático da DIO — Explorando IA como Ferramenta de Aprendizagem Ativa.*
