# Chat DeepSeek 🤖💬

Uma interface de chat simples para interagir com o modelo DeepSeek, usando Streamlit e LangChain.

## 📋 Visão Geral

Chat DeepSeek é uma aplicação que permite conversar com o modelo DeepSeek através de uma interface web intuitiva. A aplicação utiliza:

- **Streamlit** para a interface de usuário
- **LangChain** para integração com o Ollama
- **Modelo DeepSeek** executando localmente via Ollama

## ✨ Funcionalidades

- Interface de chat amigável
- Histórico de conversas durante a sessão
- Processamento local dos dados (privacidade garantida)
- Respostas em tempo real

## 🛠️ Pré-requisitos

- Python 3.8 ou superior
- Ollama instalado localmente
- Modelo DeepSeek disponível no Ollama

## 📦 Instalação

1. Clone o repositório:

```bash
git clone https://github.com/joaooliveira10/Chat-DeepSeek.git
cd Chat-DeepSeek
```

2. Instale as dependências:

```bash
pip install -r requirements.txt
```

3. Certifique-se que o Ollama está em execução e que o modelo DeepSeek está disponível:

```bash
ollama pull deepseek-r1:1.5b
```

## 🚀 Como Usar

1. Inicie o Ollama em um terminal:

```bash
ollama serve
```

2. Em outro terminal, execute a aplicação Streamlit:

```bash
streamlit run chat_deepseek.py
```

3. Acesse a interface web através do navegador (geralmente http://localhost:8501)

4. Digite suas mensagens no campo de entrada na parte inferior da tela e pressione Enter para enviar.

## 🧩 Estrutura do Projeto

```
Chat DeepSeek/
├── chat_deepseek.py    # Arquivo principal da aplicação
├── requirements.txt    # Dependências do projeto
└── README.MD           # Documentação do projeto
```

## 🔧 Personalização

Para alterar o modelo utilizado, modifique a seguinte linha no arquivo `chat_deepseek.py`:

```python
llm = ChatOllama(model="seu-modelo-preferido", base_url='http://localhost:11434')
```
