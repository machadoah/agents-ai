# Domine LLMs com LangChain 🦜🔗

Curso: [Domine LLMs com LangChain](https://www.udemy.com/course/domine-llms-com-langchain)

## Conteúdo do Curso

- Introdução sobre LLMs
- LLM com Hugging Face 🤗
- LLM com LangChain 🦜🔗
- Aplicação RAG
- Agentes e Tools
- Projeto 01 : Transcrição e compreensção de vídeos
- Projeto 02 : Chatbot com memória e interface gráfica (streamlit)
- Projeto 03 : Converse com seus documentos

## 1. Introdução sobre LLMs

### O que são LLMs?

- **LLMs (Large Language Models)** - "grandes modelos de linguagem" ou "Modelos de Linguagem de grande escala" -  são modelos de IA que utilizam técnicas de  Aprendizado de Máquina para entender e gerar linguagem humana.

- Utilizam Processamento de Linguagem Natural (**NLP**) para interagir com linguagem humana.

- É importante esclarecer e saber a diferença entre os conceitos:
  - Inteligência Artificial (**IA**)
  - Aprendizado de Máquina / Machine Learning (**ML**)
  - Processamento de Linguagem Natural (**NLP**)
  - Redes Neurais Artificiais (**ANN**)
  - IA Generativa
  - LLM (Large Language Models)

### Como funcionam os LLMs?

-  Utilizam aprendizados não-supervisionados para entender a estrutura da linguagem humana.
- Um modelos de ML é alimentado com conjuntos de dados de texto para aprender a estrutura da linguagem.
- O modelo aprende com esses exemplos sem instrução explícita.
- Extrai informações dos dados, cria conexões e aprende a estrutura da linguagem.
- Como resultado, o modelo captura as relações complexas entre as palavras e frases.
- LLMs requerem recursos computacionais significativos para treinamento e inferência.
- Utilizam unidades de processamento gráfico (**GPU**) para acelerar o treinamento e lidar com cálculos complexos.
- O uso de GPUs é essencial para treinar modelos de linguagem de grande escala, acelera o treinamento e a operação dos transformadores.

![Trasnformadores](boards/como%20funcionam%20os%20llms%20-%20transformadores.excalidraw.png)

#### Transformadores (Transformers)

- **Transformers** são uma arquitetura de rede neural que utiliza mecanismos de atenção para processar sequências de dados. 
- Transforma ou altera a representação de uma sequência de dados em outra sequência de dados.
- Foi apresentado no artigo "Attention is All You Need".
- A arquitetura melhora a capacidade dos modelos de ML ao capturar relações de longo alcance.

> [!NOTE]
> Por exemplo:
> Em "Qual é a cor do céu?", o modelo identifica a relação entre "cor", "céu" e "azul" para gerar "O céu é azul".

### Embeddings e Tokens

- **Embeddings** são representações vetoriais de palavras ou frases.
- No contexto de LLMs, embeddings são vetores que representam palavras ou frases.

![Embeddings](boards/embedding%20-%20espaço%20vetorial.excalidraw.png)

- O modelo aprende a separar e agrupar esses textos com base em suas similaridades.

> [!NOTE]
> Por exemplo:
> Quando o modelo receber uma nova palavra, como "abacaxi", ele sabe exatamente onde colocá-la no espaço vetorial, muito provavelmnete perto de "frutas".

Para palavra como "banco", o modelo pode colocá-la perto de "dinheiro" ou "sentar", dai se dá a importancia do mecanismo de atenção.

- **Tokens** são unidades menores de texto criadas através da tokenização.

Não obrigatoriamente uma palavra representa um token, pode ser uma parte de uma palavra, ou até mesmo um caractere.

