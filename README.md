# Chatbot Baseado em Conteúdo de PDFs

## Introdução

Imagine que você é um estudante de Engenharia de Software, prestes a escrever seu Trabalho de Conclusão de Curso (TCC). Para isso, você precisa revisar e correlacionar diversos artigos científicos. Entretanto, à medida que acumula mais documentos, torna-se cada vez mais difícil extrair informações relevantes e conectar ideias entre diferentes textos.

Diante desse desafio, você decide utilizar inteligência artificial para facilitar esse processo, criando um sistema de busca inteligente capaz de interpretar os PDFs, organizar informações e gerar respostas relevantes com base no conteúdo carregado.

## Objetivo

O objetivo deste projeto é permitir que você:

✅ Carregue arquivos PDF contendo informações relevantes para seu estudo ou projeto.
✅ Implemente um sistema de busca vetorial para indexar e recuperar informações dos PDFs.
✅ Utilize inteligência artificial para gerar respostas baseadas no conteúdo dos documentos carregados.
✅ Desenvolva um chat interativo onde seja possível realizar perguntas e obter respostas contextuais fundamentadas nos arquivos.

## Tecnologias Utilizadas

- **Python**: Linguagem principal do projeto.
- **LangChain**: Framework para manipulação e processamento de linguagem natural.
- **FAISS**: Biblioteca para indexação e busca vetorial.
- **OpenAI GPT**: Modelo de linguagem para geração de respostas.
- **Streamlit**: Interface web interativa para o chatbot.
- **PyMuPDF ou PDFPlumber**: Extração de texto de PDFs.

## Como Executar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/chatbot-pdf.git
   cd chatbot-pdf
   ```

2. Crie um ambiente virtual e instale as dependências:
   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows use: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Execute o chatbot:
   ```bash
   streamlit run app.py
   ```

## Como Funciona

1. **Upload de PDFs**: O usuário faz o upload dos documentos.
2. **Processamento e Indexação**: O texto é extraído e convertido em embeddings vetoriais.
3. **Interação via Chat**: O usuário faz perguntas, e o chatbot responde com base nas informações indexadas.
4. **Geração de Respostas**: O modelo de IA busca no banco de dados vetorial e gera respostas relevantes.

## Como Entregar o Projeto

1. **Repositório GitHub**: Hospede seu código em um repositório público.
2. **Demonstração**: Grave um vídeo curto apresentando o funcionamento.
3. **Documentação**: Inclua este README.md com instruções claras.
4. **Deploy (Opcional)**: Publique o chatbot em plataformas como **Streamlit Sharing**, **Render** ou **Hugging Face Spaces**.

## Melhorias Futuras

- Implementar suporte para diferentes formatos de documentos (Word, TXT, etc.).
- Melhorar a precisão das respostas com técnicas de RAG (Retriever-Augmented Generation).
- Criar uma versão com API para integração em outros sistemas.
