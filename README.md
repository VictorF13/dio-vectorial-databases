# Bancos de Dados Vetoriais - Mentoria DIO

Este repositório contém os exemplos práticos e materiais de apoio para a mentoria sobre Bancos de Dados Vetoriais, realizada no dia 21 de julho de 2025 para o bootcamp de IA/Dados da DIO.

## Sobre o Projeto

O objetivo deste projeto é demonstrar o uso de bancos de dados vetoriais e embeddings para resolver problemas comuns no campo da Inteligência Artificial, como busca semântica, sistemas de recomendação, detecção de plágio e agrupamento de documentos.

## Conteúdo

O repositório está estruturado com exemplos práticos, cada um contido em um Jupyter Notebook na pasta `practical_examples/`:

* **encontrando\_felinos.ipynb**: Demonstra como realizar uma busca semântica para encontrar informações específicas (felinos) em um conjunto de textos sobre animais, utilizando embeddings, FAISS para a busca inicial e um Cross-Encoder para re-ranking dos resultados.
* **sistema\_de\_recomendacao.ipynb**: Apresenta a construção de um sistema de recomendação de produtos baseado na similaridade de suas descrições, utilizando `SentenceTransformerEmbeddings` e FAISS.
* **deduplicacao\_e\_plagio.ipynb**: Mostra como identificar textos duplicados ou com alta similaridade (potenciais plágios) em um conjunto de dados, vetorizando os textos e comparando suas distâncias.
* **tagueando\_documentos.ipynb**: Ensina a agrupar documentos por temática através da clusterização (K-Means) de seus vetores e, em seguida, utiliza um modelo de linguagem (LLM) para gerar rótulos descritivos para cada grupo.

## Como Usar

Para executar os exemplos contidos neste repositório, siga os passos abaixo.

### Pré-requisitos

* Python 3.12 ou superior.

### Instalação

1. Clone o repositório para a sua máquina local.

2. Navegue até o diretório do projeto.

3. Instale as dependências necessárias executando o comando abaixo:

    ```bash
    pip install -r requirements.txt
    ```

4. Para o notebook `tagueando_documentos.ipynb`, é necessário ter uma chave de API da OpenAI. Crie um arquivo chamado `.env` na raiz do projeto e adicione sua chave:

    ```env
    OPENAI_API_KEY="sua-chave-aqui"
    ```

### Execução

Após a instalação, você pode navegar pela pasta `practical_examples/` e abrir os notebooks (`.ipynb`) utilizando o Jupyter Notebook ou qualquer editor de código compatível (como o VS Code) para explorar e executar os exemplos.
