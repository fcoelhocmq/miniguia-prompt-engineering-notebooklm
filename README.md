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

**Resultado:** A resposta foi genérica e superficial, sem aprofundamento nas fontes carregadas. A IA trouxe uma definição padrão sem citar os materiais do caderno.

**⚠️ Dificuldade encontrada:** Prompts curtos e vagos fazem o NotebookLM responder de forma genérica, sem aproveitar o conteúdo das fontes adicionadas.

---

**Prompt Testado (v2 — refinado com contexto):**
```
Com base nas fontes do meu caderno, explique o que é Engenharia de Prompts 
para alguém que nunca teve contato com o assunto. Use uma linguagem simples, 
com exemplos práticos do dia a dia e destaque por que essa habilidade é 
importante no mercado de trabalho atual.
```

**✅ Resultado obtido:**
A IA utilizou as fontes carregadas para montar uma explicação em camadas: partiu de uma analogia (o prompt como "instrução para um assistente humano"), contextualizou com o mercado de trabalho e citou trechos do Prompt Engineering Guide e do LearnPrompting. A resposta foi muito mais rica e referenciada.

**💡 Aprendizado:** Especificar o **público-alvo**, o **tom desejado** e o **objetivo final** transforma completamente a qualidade da resposta.

---

### 🔹 Sessão 2 — Mapeando as Técnicas Principais

**🎯 Objetivo:** Criar uma visão geral das principais técnicas de prompting.

**Prompt Testado:**
```
Com base nas minhas fontes, liste as principais técnicas de Engenharia de Prompts 
em ordem de complexidade, do mais simples ao mais avançado. Para cada técnica, 
forneça: nome, descrição em 2 linhas e um exemplo de uso prático.
```

**✅ Resultado obtido:**
O NotebookLM gerou uma tabela estruturada com 6 técnicas (Zero-shot, Few-shot, Chain-of-Thought, Role Prompting, Tree of Thought e ReAct), com descrições e exemplos extraídos diretamente das fontes, incluindo citações. Excelente para usar como material de revisão.

**⚠️ Dificuldade encontrada:** Na primeira tentativa, a IA misturou técnicas de prompt com conceitos de fine-tuning. Foi necessário adicionar ao prompt: *"considere apenas técnicas de prompting em tempo de inferência, sem retreinamento do modelo"* para delimitar o escopo.

---

### 🔹 Sessão 3 — Aplicação Prática com Chain-of-Thought

**🎯 Objetivo:** Entender na prática como o Chain-of-Thought (CoT) funciona.

**Prompt Testado:**
```
Explique o que é Chain-of-Thought Prompting com base no paper científico 
das minhas fontes. Depois, me dê um exemplo comparativo: primeiro resolvendo 
um problema SEM CoT e depois COM CoT, para eu visualizar a diferença.
```

**✅ Resultado obtido:**
A IA citou o paper do Google Brain (Wei et al., 2022) e construiu um exemplo comparativo claro com um problema de raciocínio matemático simples. A diferença de qualidade entre as respostas com e sem CoT ficou evidente.

**💡 Aprendizado:** Pedir exemplos **comparativos** (com X vs. sem X) é uma das estratégias mais poderosas para consolidar conceitos novos.

---

### 🔹 Sessão 4 — Geração do Glossário

**Prompt Testado:**
```
Com base em todas as minhas fontes, crie um glossário com os 15 termos técnicos 
mais importantes relacionados à Engenharia de Prompts. Para cada termo, escreva 
uma definição curta (máximo 3 linhas) em português, adequada para iniciantes.
Organize em ordem alfabética.
```

**✅ Resultado:** Gerou o glossário completo com citações das fontes. Usado diretamente na seção de Miniguia abaixo.

---

### 🔹 Sessão 5 — Geração do Podcast de Revisão (Funcionalidade Audio Overview)

**Experimento:** Utilizei a funcionalidade **"Audio Overview"** do NotebookLM para gerar um podcast de revisão sobre o conteúdo do caderno.

**Resultado:** O podcast de ~8 minutos cobriu os principais conceitos de forma conversacional entre dois apresentadores simulados. Excelente para revisar o conteúdo enquanto se faz outra atividade.

**⚠️ Limitação observada:** O áudio gerado está em inglês por padrão. Para contornar, instrua o NotebookLM em português no campo de customização do podcast antes de gerar.

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

| Termo | Definição |
|-------|-----------|
| **Prompt** | Instrução ou entrada de texto enviada a um modelo de linguagem para gerar uma resposta. |
| **LLM (Large Language Model)** | Modelo de linguagem de grande escala treinado em enormes volumes de texto. Ex: GPT-4, Claude, Gemini. |
| **Token** | Unidade básica de processamento de texto em LLMs. Pode ser uma palavra, parte de palavra ou pontuação. |
| **Temperatura** | Parâmetro que controla a criatividade/aleatoriedade das respostas. Valores altos = mais criativo; valores baixos = mais determinístico. |
| **Zero-shot** | Técnica onde o modelo realiza uma tarefa sem receber exemplos prévios. |
| **Few-shot** | Técnica onde alguns exemplos são fornecidos no prompt para guiar o modelo. |
| **Chain-of-Thought** | Estratégia que induz o modelo a raciocinar passo a passo antes de responder. |
| **Role Prompting** | Atribuição de uma persona ou papel específico ao modelo no prompt. |
| **Hallucination** | Quando o modelo gera informações falsas ou inventadas com aparência de verdade. |
| **Context Window** | Limite máximo de tokens que um modelo pode processar em uma única interação. |
| **System Prompt** | Instrução inicial que define o comportamento geral do modelo em uma conversa. |
| **Fine-tuning** | Processo de retreinar um modelo em dados específicos (diferente de prompting). |
| **Inference** | O processo de o modelo gerar uma resposta a partir de um prompt. |
| **Grounding** | Técnica de fornecer fontes/documentos ao modelo para basear suas respostas em fatos verificáveis. |
| **RAG (Retrieval-Augmented Generation)** | Arquitetura que combina busca em base de conhecimento com geração de texto para respostas mais precisas. |

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
