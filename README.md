# Projeto Oráculo

Oráculo é um assistente de IA conversacional que permite interagir com diversos tipos de documentos usando modelos de linguagem avançados.

## 📋 Descrição

O Projeto Oráculo é uma aplicação Streamlit que permite carregar diferentes tipos de documentos (sites, vídeos do YouTube, PDFs, CSVs e arquivos de texto) e interagir com eles através de uma interface de chat, utilizando modelos de linguagem de grandes provedores como Groq e OpenAI.

## ✨ Funcionalidades

- **Múltiplas fontes de dados**: Carregue e interaja com conteúdo de:
  - Sites web
  - Vídeos do YouTube
  - Arquivos PDF
  - Arquivos CSV
  - Arquivos de texto (TXT)

- **Escolha de modelos de IA**:
  - Suporte para modelos da Groq (llama-3.1-70b-versatile, gemma2-9b-it, mixtral-8x7b-32768)
  - Suporte para modelos da OpenAI (gpt-4o-mini, gpt-4o, o1-preview, o1-mini)

- **Interface amigável**:
  - Chat interativo com histórico de conversas
  - Upload fácil de arquivos
  - Configuração simples de modelos e APIs

## 🚀 Como usar

1. Execute a aplicação Streamlit:
   ```
   streamlit run streamlit.py
   ```

2. No painel lateral:
   - Selecione o tipo de arquivo que deseja carregar
   - Forneça a URL ou faça upload do arquivo
   - Escolha o provedor de modelo (Groq ou OpenAI)
   - Selecione o modelo específico
   - Insira sua chave de API
   - Clique em "Inicializar Oráculo"

3. Comece a conversar com o Oráculo sobre o conteúdo carregado!

## 🛠️ Requisitos

- Python 3.6+
- Streamlit
- LangChain
- Bibliotecas de integração com Groq e OpenAI
- Bibliotecas para processamento de documentos (PyPDF, etc.)

Para instalar todas as dependências necessárias:
```
pip install -r requirements.txt
```

Conteúdo do arquivo requirements.txt:
```
streamlit==1.38.0
langchain==0.3.0
langchain-community==0.3.0
langchain-groq==0.2.0
langchain-openai==0.2.0
python-dotenv==1.0.1
beautifulsoup4==4.12.3
pypdf==5.0.0
unstructured==0.15.13
fake_useragent==1.5.1
youtube_transcript_api==0.6.2
```

## 📦 Estrutura do projeto

```
app/
├── streamlit.py         # Aplicação principal Streamlit
├── loaders_documents.py # Funções para carregar diferentes tipos de documentos
├── requirements.txt     # Dependências do projeto
└── README.md            # Este arquivo
```

## 🔑 Configuração de API

Para usar o Oráculo, você precisará de chaves de API válidas:
- Para modelos da Groq: [Obtenha uma chave API da Groq](https://console.groq.com/)
- Para modelos da OpenAI: [Obtenha uma chave API da OpenAI](https://platform.openai.com/api-keys)

## 📝 Notas

- O Oráculo mantém um histórico de conversas que pode ser apagado a qualquer momento
- Para melhores resultados, certifique-se de que os documentos carregados estejam em um formato legível
- Alguns sites podem não ser carregados corretamente devido a restrições de acesso

---

Desenvolvido como pojeto de LangChain da plataforma Asimov Academy
