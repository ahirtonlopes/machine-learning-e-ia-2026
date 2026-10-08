# 🧠 Machine Learning e IA: Da máquina que aprende à IA que age

Material de apoio da palestra **"Machine Learning e IA: Da máquina que aprende à IA que age"**, apresentada em **08/10/2026** para alunos de graduação. 🎉

Se você chegou aqui pelo QR code do último slide: seja bem-vindo(a)! Este repositório reúne **10 exemplos práticos**, um para cada ideia da palestra, do modelo que separa links maliciosos de links seguros até um agente de IA que planeja passeios. Tudo roda no **Google Colab**, direto no navegador e de graça: você **não precisa instalar nada** no seu computador, e não precisa já saber programar para acompanhar. Se você nunca rodou um notebook na vida, comece pela seção [🚀 Comece por aqui](#-comece-por-aqui-passo-a-passo).

**Professor:** [Prof. Dr. Ahirton Lopes](https://github.com/ahirtonlopes) · [LinkedIn](https://www.linkedin.com/in/ahirtonlopes)

---

## 📂 Estrutura do repositório

```bash
.
├── README.md                 # Este guia
├── LICENSE                   # Licença MIT
├── Datasets/                 # Bases de dados (CSV) usadas nos exemplos 01 a 03
│   ├── url_data.csv          # URLs rotuladas como maliciosas (bad) ou benignas (good)
│   ├── payment_fraud.csv     # Transações de pagamento rotuladas como fraude ou não
│   └── Mall_Customers.csv    # Clientes de um shopping (idade, renda, nota de gastos)
└── Notebooks/                # Os 10 exemplos, na ordem da palestra
    ├── 01_Ciberseguranca_Links_Maliciosos.ipynb
    ├── 02_Financas_Deteccao_de_Fraude.ipynb
    ├── 03_Varejo_Segmentacao_de_Clientes.ipynb
    ├── 04_Atendimento_Previsao_Call_Center.ipynb
    ├── 05_Bastidores_Descida_do_Gradiente.ipynb
    ├── 06_Visao_Computacional_CNN.ipynb
    ├── 07_Marketing_Sentimento_de_Reviews.ipynb
    ├── 08_LLMs_Atencao_e_Transformers.ipynb
    ├── 09_Mobilidade_Q_Learning_Taxi.ipynb
    ├── 10_Turismo_Primeiro_Agente_ADK.ipynb
    └── assets/               # GIFs usados no exemplo 09
```

Os notebooks baixam sozinhos o que precisam (os CSVs vêm deste repositório; as bases CIFAR-10 e IMDB vêm direto da biblioteca Keras; os modelos do exemplo 08 vêm do Hugging Face). Você só precisa clicar e rodar.

---

## 🗺️ Mapa palestra → exemplos

| # | Exemplo | Área | Tipo de aprendizado / técnica | Abrir | Tempo de execução* |
|---|---|---|---|---|---|
| 01 | Links maliciosos | Cibersegurança | Supervisionado: classificação (TF-IDF + Regressão Logística) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ahirtonlopes/machine-learning-e-ia-2026/blob/main/Notebooks/01_Ciberseguranca_Links_Maliciosos.ipynb) | ~10 s |
| 02 | Detecção de fraude | Finanças / pagamentos | Supervisionado: classificação, métricas (precisão x recall) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ahirtonlopes/machine-learning-e-ia-2026/blob/main/Notebooks/02_Financas_Deteccao_de_Fraude.ipynb) | ~5 s |
| 03 | Segmentação de clientes | Varejo | Não supervisionado: agrupamento (K-Means) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ahirtonlopes/machine-learning-e-ia-2026/blob/main/Notebooks/03_Varejo_Segmentacao_de_Clientes.ipynb) | ~5 s |
| 04 | Previsão de chamadas | Atendimento / operações | Supervisionado: regressão sobre série temporal | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ahirtonlopes/machine-learning-e-ia-2026/blob/main/Notebooks/04_Atendimento_Previsao_Call_Center.ipynb) | ~2 s |
| 05 | Descida do gradiente | Bastidores do deep learning | Otimização: como uma rede neural aprende | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ahirtonlopes/machine-learning-e-ia-2026/blob/main/Notebooks/05_Bastidores_Descida_do_Gradiente.ipynb) | ~1 s |
| 06 | Reconhecendo imagens | Visão computacional | Deep Learning: rede convolucional (CNN) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ahirtonlopes/machine-learning-e-ia-2026/blob/main/Notebooks/06_Visao_Computacional_CNN.ipynb) | ~25 s + download da base (170 MB) |
| 07 | Sentimento de reviews | Marketing / reputação de marca | Deep Learning: rede recorrente (LSTM) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ahirtonlopes/machine-learning-e-ia-2026/blob/main/Notebooks/07_Marketing_Sentimento_de_Reviews.ipynb) | ~25 s |
| 08 | Atenção e Transformers | Base dos LLMs | Deep Learning: atenção Q/K/V, Transformer, modelos pré-treinados | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ahirtonlopes/machine-learning-e-ia-2026/blob/main/Notebooks/08_LLMs_Atencao_e_Transformers.ipynb) | ~15 s + download dos modelos (~2 GB) |
| 09 | Táxi que aprende rotas | Mobilidade | Aprendizado por reforço (Q-Learning) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ahirtonlopes/machine-learning-e-ia-2026/blob/main/Notebooks/09_Mobilidade_Q_Learning_Taxi.ipynb) | ~45 s |
| 10 | Primeiro agente de IA | Turismo | Agentes de IA (Google ADK + Gemini) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ahirtonlopes/machine-learning-e-ia-2026/blob/main/Notebooks/10_Turismo_Primeiro_Agente_ADK.ipynb) | ~5 min (depende da API) |

\* Tempo medido executando o notebook inteiro, de uma vez, em um notebook pessoal (CPU, sem GPU), sem contar instalação de bibliotecas nem downloads. No Colab os números variam um pouco: a primeira execução também inclui o download das bases e dos modelos, e os exemplos 06 a 08 podem levar alguns minutos na CPU do Colab, ficando bem mais rápidos com GPU. O tempo do exemplo 10 é uma estimativa, porque ele depende das respostas da API do Gemini.

---

## 🚀 Comece por aqui (passo a passo)

Nunca usou o Colab? Sem problema, é só seguir estes passos:

### 1. Abra o notebook no Colab

Na tabela acima, clique no botão **"Open in Colab"** do exemplo que você quer rodar. Ele abre direto no navegador. Faça login com sua conta Google se o Colab pedir.

### 2. Salve uma cópia sua

No menu do Colab, clique em **Arquivo → Salvar uma cópia no Drive**. Assim você pode editar, testar e mexer à vontade sem medo: a cópia é sua.

### 3. Rode célula por célula

Um notebook é uma sequência de **células**: algumas têm texto explicativo, outras têm código. Clique em uma célula de código e aperte **`Shift + Enter`** para executá-la e pular para a próxima. Vá descendo na ordem, lendo o texto entre as células. Se preferir rodar tudo de uma vez: **Ambiente de execução → Executar tudo**.

> 💡 Na primeira execução, o Colab pode mostrar o aviso *"Este notebook não foi criado pelo Google"*. É um aviso padrão para notebooks vindos do GitHub: clique em **Executar assim mesmo**.

### 4. Deu erro? Calma, acontece

- **Rode as células na ordem.** A maioria dos erros (`NameError`, `FileNotFoundError`) vem de pular uma célula de cima, como a que baixa o CSV ou a que importa as bibliotecas.
- **Recomece do zero:** **Ambiente de execução → Reiniciar sessão** e depois rode de novo desde a primeira célula.
- **Leia a última linha do erro:** ela quase sempre diz o que faltou. Copiar essa linha no buscador (ou perguntar a um assistente de IA) costuma resolver.
- **Avisos em vermelho nem sempre são erros:** mensagens de *warning* durante a instalação ou o treino são normais; o que importa é a célula terminar.

### 5. GPU grátis para os exemplos de Deep Learning (06, 07 e 08)

Os exemplos 06, 07 e 08 treinam ou usam redes neurais e ficam bem mais rápidos com GPU. No Colab: **Ambiente de execução → Alterar o tipo de ambiente de execução → T4 GPU → Salvar**. Faça isso **antes** de rodar a primeira célula (trocar o ambiente reinicia a sessão). A GPU gratuita tem cota de uso; se ela não estiver disponível no momento, os notebooks também rodam na CPU, só que mais devagar.

---

## 📊 Machine Learning clássico (exemplos 01 a 04)

Os primeiros exemplos mostram a "máquina que aprende" no formato mais clássico: dados em tabela, um algoritmo do scikit-learn e uma métrica para saber se ficou bom.

### 01 - Cibersegurança: detectando links maliciosos

**O que você vai ver:**
- Como transformar texto (a URL) em números com **TF-IDF**, para o modelo conseguir "ler".
- Uma **Regressão Logística** aprendendo a separar links maliciosos (`bad`) de benignos (`good`) a partir de 420 mil exemplos rotulados.
- Por que comparar com um **baseline** (chutar sempre a resposta mais comum) antes de comemorar a acurácia.

**Resultado esperado:** acurácia de **96,4%** no teste, contra **82,2%** do baseline, ou seja, um ganho real de cerca de 14 pontos percentuais. Os quatro links de exemplo no final são classificados corretamente (`phishing.ru` e `free-robux-generator.xyz` como `bad`, `github.com` e `example.com` como `good`).

### 02 - Finanças: detecção de fraude em pagamentos

**O que você vai ver, em 3 atos:**
- **Ato 1, resultado bom demais:** o modelo acerta 100%. Investigando, descobrimos um **vazamento de alvo**: uma única coluna (`accountAgeDays`) entrega a resposta.
- **Ato 2, a armadilha da acurácia:** sem a coluna vazada, o modelo chega a **98,5% de acurácia** e mesmo assim pega **0 de 112 fraudes** (recall 0). Como só 1,4% das transações são fraude, "dizer que nada é fraude" já acerta quase tudo.
- **Ato 3, o trade-off:** balanceando as classes, a Regressão Logística passa a pegar **109 de 112 fraudes** (recall 97,3%), mas com **4.003 alarmes falsos** (precisão 2,7%). A Árvore de Decisão balanceada pega 84 de 112 com 2.305 alarmes falsos.

**Lição:** em problemas raros, acurácia engana; o que importa é decidir quanto custa cada tipo de erro.

### 03 - Varejo: segmentação de clientes com K-Means

**O que você vai ver:**
- **Aprendizado não supervisionado:** 200 clientes de um shopping, sem nenhum rótulo, agrupados por **renda anual** e **nota de gastos**.
- Como escolher o número de grupos com o **método do cotovelo** e o **coeficiente de silhueta**.
- A transformação de clusters em **personas de negócio** (por exemplo: renda alta e gasto alto, renda alta e gasto baixo).

**Resultado esperado:** a melhor silhueta aparece com **K = 5** (0,554), formando 5 grupos com 81, 39, 35, 23 e 22 clientes.

### 04 - Atendimento: previsão de demanda em um call center

**O que você vai ver:**
- Uma **série temporal** simulada de chamadas diárias, com tendência, sazonalidade semanal, picos no início do mês e ruído.
- Criação de variáveis a partir do tempo (dia da semana, fim de semana, valores de ontem e da semana passada) e divisão treino/teste **respeitando a ordem do tempo**.
- Uma **Regressão Linear** comparada com um baseline ingênuo ("amanhã será igual a hoje").

**Resultado esperado:** o modelo erra em média **7,1 chamadas por dia** (MAE), contra **19,5** do baseline: quase 3 vezes melhor.

---

## 🧬 Deep Learning (exemplos 05 a 08)

Aqui a máquina passa a aprender com **redes neurais**: em vez de nós escolhermos as variáveis, a rede aprende sozinha as representações a partir de pixels ou palavras.

### 05 - Bastidores: como uma rede neural aprende

**O que você vai ver:**
- A **descida do gradiente** encontrando o mínimo de uma função, passo a passo, em um gráfico.
- As **funções de ativação** mais usadas (Sigmoid, ReLU, Tanh) e por que elas permitem que a rede aprenda padrões não lineares.
- Como as **camadas** de uma rede se empilham.

**Resultado esperado:** partindo de x = 5, em 30 passos a descida do gradiente chega a **x = 0,0062**, praticamente o mínimo da função (x = 0).

### 06 - Visão computacional: reconhecendo imagens com uma CNN

**O que você vai ver:**
- A base **CIFAR-10**: 60 mil imagens pequenas (32x32) de aviões, carros, pássaros, gatos, cervos, cachorros, sapos, cavalos, navios e caminhões.
- Uma **rede convolucional** (CNN) com 3 camadas de convolução treinada do zero.
- Uma grade com as previsões: em verde os acertos, em vermelho os erros.

**Resultado esperado:** em 5 épocas de treino, a rede chega a cerca de **62% de acurácia no teste** (na execução de referência, 62,2%; validação em 62,9%). Parece pouco? Chutando ao acaso entre 10 classes, a acurácia seria 10%. Quer melhorar? Aumente `EPOCHS` para 10 ou 20 e compare.

### 07 - Marketing: sentimento de avaliações com LSTM

**O que você vai ver:**
- A base **IMDB**: 50 mil avaliações de filmes, rotuladas como positivas ou negativas.
- Um **embedding** transformando palavras em vetores e camadas **LSTM** lendo o texto em sequência.
- As curvas de treino e validação, para identificar **overfitting**.

**Resultado esperado:** em 3 épocas, a rede acerta cerca de **81% a 83% das avaliações do teste** (duas execuções de referência: 80,2% e 82,7%). O número varia um pouco a cada execução, porque os pesos começam aleatórios.

### 08 - LLMs: atenção e Transformers, do zero ao ChatGPT

**O que você vai ver:**
- O mecanismo de **atenção** (Query, Key, Value) implementado do zero com NumPy, com mapas de atenção desenhados.
- **Multi-Head Attention**, **Positional Encoding** e um bloco Transformer completo em TensorFlow.
- Modelos **pré-treinados do Hugging Face** em ação: análise de sentimento, reconhecimento de entidades (NER), perguntas e respostas e os mapas de atenção de um BERT de verdade.

**Resultado esperado:** o modelo de sentimento dá 5 estrelas para "Esse produto é incrível!", 1 estrela para "Péssima experiência" e 3 estrelas para a frase neutra; o NER encontra **Microsoft** (organização), **Satya Nadella** (pessoa) e **Seattle** (local) com mais de 97% de confiança; e o modelo de perguntas e respostas acerta "2017" e "Vaswani et al." direto do texto.

> ⏳ Este notebook baixa cerca de 2 GB de modelos do Hugging Face na primeira execução. No Colab isso leva poucos minutos; tenha paciência na seção 9.

---

## 🎮 Reinforcement Learning (exemplo 09)

### 09 - Mobilidade: um táxi que aprende rotas com Q-Learning

**O que você vai ver:**
- O ambiente **Taxi** do Gymnasium: um táxi precisa buscar o passageiro e deixá-lo no destino com o menor número de movimentos.
- Primeiro um táxi **aleatório**, perdido no mapa; depois, a **tabela Q** sendo preenchida por tentativa e erro, guiada por recompensas.
- O dilema **explorar x aproveitar** (epsilon-greedy).

**Resultado esperado:** após 2.000 episódios de treino (poucos segundos), o táxi treinado completa a corrida em **13 passos**, com pontuação **+8**, enquanto o táxi aleatório só anda a esmo pelo mapa durante 100 passos.

---

## 🤖 Agentes de IA (exemplo 10)

### 10 - Turismo: seu primeiro agente de IA com Google ADK

Aqui chegamos à "IA que age": um **LLM (Gemini)** que, além de responder, **decide usar ferramentas** (busca no Google, uma API de clima em tempo real) e **lembra da conversa**.

**O que você vai ver:**
- Um agente que monta passeios de um dia em São Paulo, criado do zero com o [Google ADK](https://google.github.io/adk-docs/).
- Uma **ferramenta customizada** que consulta o clima em tempo real (API Open-Meteo) em pontos de **São Paulo** (Parque Ibirapuera, MASP, Mercadão, Pinacoteca, Theatro Municipal) antes de sugerir o roteiro.
- Um **time de agentes**, em que um agente principal delega tarefas para especialistas.
- **Sessions**: a diferença entre um agente com memória e um agente que esquece tudo a cada pergunta.

Este exemplo precisa de uma **API key gratuita** do Google AI Studio. Siga os passos:

#### 1. Gere sua API key do Google AI Studio

1. Acesse https://aistudio.google.com/app/apikey com sua conta Google.
2. Clique em **"Create API key"** e copie a chave (os formatos atuais começam com `AIza...` ou `AQ...`).

#### 2. Abra o notebook 10 no Colab

Use o botão **"Open in Colab"** da tabela lá em cima e salve uma cópia sua: `Arquivo → Salvar uma cópia no Drive`.

#### 3. Guarde a chave no Colab

1. No menu lateral esquerdo do Colab, clique no ícone de **chave (🔑 Secrets)**.
2. Crie um secret chamado `GOOGLE_API_KEY`, cole sua chave e habilite o acesso do notebook.

> 🔒 **Nunca cole sua chave direto no código** nem publique um notebook com ela. O Secrets do Colab existe justamente para isso.

#### 4. Rode as células na ordem

Execute célula por célula (`Shift+Enter`). Uma das primeiras células lista **todos os modelos Gemini disponíveis para a sua chave**. O notebook usa por padrão o `gemini-3.1-flash-lite`, que tem a maior cota no plano gratuito; para trocar de modelo, basta editar a variável `MODEL_NAME`.

> ⚠️ Se aparecer o erro **`429 RESOURCE_EXHAUSTED`**, você atingiu o limite de requisições por minuto do plano gratuito. Espere cerca de 1 minuto e rode a célula de novo.

**Créditos:** este notebook é uma adaptação do material **ADK Adventure**, criado por [Qingyue (Annie) Wang](https://www.linkedin.com/in/anniewangtech/), Developer Advocate no Google, traduzido para o português, atualizado para os modelos Gemini atuais e ambientado em São Paulo pelo Prof. Dr. Ahirton Lopes.

---

## 🧭 Glossário rápido

| Termo | Em uma frase |
|---|---|
| **Dataset** | O conjunto de dados usado para treinar e avaliar um modelo, geralmente uma tabela em que cada linha é um exemplo. |
| **Feature (atributo)** | Uma característica usada como entrada do modelo, como a renda de um cliente ou o texto de uma URL. |
| **Rótulo (label / alvo)** | A resposta certa que queremos prever, como "fraude" ou "não fraude". Só existe no aprendizado supervisionado. |
| **Treino e teste** | Separamos os dados em duas partes: uma para o modelo aprender (treino) e outra, que ele nunca viu, para medir se aprendeu de verdade (teste). |
| **Acurácia** | A porcentagem de previsões certas no total. Intuitiva, mas engana quando uma das classes é muito rara. |
| **Precisão** | Dos casos que o modelo apontou como positivos (ex.: fraude), quantos eram positivos de verdade. Precisão baixa = muito alarme falso. |
| **Recall (revocação)** | Dos casos positivos que existiam, quantos o modelo conseguiu encontrar. Recall baixo = muita fraude passando. |
| **Baseline** | Uma referência simples (como chutar sempre a resposta mais comum) que o modelo precisa superar para ter valor. |
| **Overfitting** | Quando o modelo decora os dados de treino e vai mal em dados novos, como um aluno que decorou a prova antiga. |
| **Rede neural** | Um modelo formado por camadas de "neurônios" artificiais que aprendem ajustando milhões de pesos. É a base do deep learning. |
| **Época** | Uma passada completa da rede neural por todos os dados de treino. Treinar por 5 épocas é ver os dados 5 vezes. |
| **Embedding** | Uma forma de representar palavras (ou imagens, produtos...) como vetores de números, de modo que coisas parecidas fiquem próximas. |
| **Token** | O pedaço de texto que um modelo de linguagem processa de cada vez: pode ser uma palavra, parte de uma palavra ou um sinal. |
| **Transformer / Atenção** | A arquitetura de rede neural por trás dos LLMs; a atenção permite que cada token "olhe" para todos os outros e pese o que importa. |
| **LLM** | Large Language Model: um Transformer enorme treinado com muito texto para prever o próximo token, como o Gemini e o ChatGPT. |
| **Aprendizado por reforço** | O agente aprende por tentativa e erro, recebendo recompensas ou punições pelas ações que toma. |
| **Agente de IA** | Um sistema em que um LLM decide quais ações e ferramentas usar (buscar, chamar uma API, delegar) para cumprir um objetivo. |

---

## 📚 Para continuar estudando

Gostou e quer ir além? Estes repositórios públicos do professor aprofundam cada bloco da palestra, com mais exemplos e explicações:

| Repositório | O que tem lá |
|---|---|
| [Machine-Learning-Foundations-and-Classic-Models](https://github.com/ahirtonlopes/Machine-Learning-Foundations-and-Classic-Models) | Machine Learning clássico: classificação, métricas, agrupamento, séries temporais e Q-Learning |
| [AI-Foundation-and-Learning-Models](https://github.com/ahirtonlopes/AI-Foundation-and-Learning-Models) | Deep Learning: CNNs, RNNs/LSTMs, autoencoders, GANs, Transformers, YOLO e mais |
| [Mastering-Reinforcement-Learning](https://github.com/ahirtonlopes/Mastering-Reinforcement-Learning) | Aprendizado por reforço na prática: Q-Learning, equação de Bellman e Deep Q-Networks (Breakout, LunarLander) |
| [Open-Deep-Learning](https://github.com/ahirtonlopes/Open-Deep-Learning) | Projeto aberto, em português, de ensino de Deep Learning com Keras e TensorFlow (MNIST, CNNs, RNNs, autoencoders) |
| [build-with-ai-curitiba-2026](https://github.com/ahirtonlopes/build-with-ai-curitiba-2026) | Material extra: workshop completo de agentes com ADK (inclui multiagentes: Sequential, Loop, Parallel e Router) |

E fontes oficiais gratuitas para estudar no seu ritmo:

- [Google Machine Learning Crash Course](https://developers.google.com/machine-learning/crash-course): curso introdutório de ML do Google, com exercícios interativos.
- [Kaggle Learn](https://www.kaggle.com/learn): microcursos práticos de Python, pandas, ML e deep learning, todos rodando no navegador.
- [Curso de LLMs do Hugging Face (em português)](https://huggingface.co/learn/llm-course/pt/chapter1/1): Transformers e modelos de linguagem na prática.
- [Documentação do Google ADK](https://google.github.io/adk-docs/): para construir seus próprios agentes.

---

*Prof. Dr. Ahirton Lopes - Palestra "Machine Learning e IA", 08/10/2026*
