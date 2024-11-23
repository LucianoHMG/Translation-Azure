
## 📑 Índice

- [📁 Estrutura do Projeto](#-estrutura-do-projeto)
- [📑 Índice](#-índice)
- [📋 Sobre o Projeto](#-sobre-o-projeto)
  - [🎯 Tradutor de Artigos](#-tradutor-de-artigos)
  - [📄 Tradutor de Documentos](#-tradutor-de-documentos)
- [🚀 Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [📦 Requisitos](#-requisitos)
- [⚙️ Instalação e Execução](#️-instalação-e-execução)
  - [💻 Execução Local com Poetry](#-execução-local-com-poetry)
- [🎯 Conclusão e Aprendizados](#-conclusão-e-aprendizados)
  

## 📋 Sobre o Projeto

O Tradutor Multifuncional é uma aplicação web que oferece duas ferramentas de tradução integradas em uma única plataforma. Desenvolvida com foco na experiência do usuário, a solução atende diferentes necessidades de tradução em um ambiente profissional e intuitivo.

### 🎯 Tradutor de Artigos

O módulo de tradução de artigos utiliza a avançada API do Azure OpenAI GPT-4o mini para oferecer traduções precisas e contextualmente relevantes de artigos web. Características principais:

- Extração automática de conteúdo de URLs
- Preservação da formatação markdown
- Suporte a múltiplos idiomas
- Download do arquivo traduzido
- Interface intuitiva e responsiva

### 📄 Tradutor de Documentos
[🔝 Voltar ao índice](#-índice)

O módulo de tradução de documentos é alimentado pela Azure Translator API, oferecendo tradução profissional de documentos Word. Destaques:

- Suporte a arquivos .docx
- Múltiplos pares de idiomas
- Preservação da formatação do documento
- Download do arquivo traduzido
- Interface amigável para upload de arquivos

## 🚀 Tecnologias Utilizadas

**Core:**
- Python
- Azure OpenAI
- Azure Translator

**Bibliotecas Principais:**
- `python-docx`: Manipulação de documentos Word
- `beautifulsoup4`: Extração de conteúdo web
- `python-dotenv`: Gerenciamento de variáveis de ambiente

## 📦 Requisitos

- Python
- Poetry para gerenciamento de dependências
- Conta Azure com acesso às APIs: 
  - Azure OpenAI
  - Azure Translator

## ⚙️ Instalação e Execução

### 💻 Execução Local com Poetry
[🔝 Voltar ao índice](#-índice)

1. Clone o repositório:
```bash
git clone https://github.com/Jcnok/Bootcamp-Microsoft-Certification-Challenge--1-AI_102.git

```
2. Navegue até a pasta do repositório:
```bash	
cd Bootcamp-Microsoft-Certification-Challenge--1-AI_102
```

3. Instale o Poetry (caso não tenha):
```bash
curl -sSL https://install.python-poetry.org | python3 -
```

4. Configure o ambiente virtual e instale as dependências:
```bash
poetry install
```

5. Configure as variáveis de ambiente:
```bash
cp .env.example .env
```

6. Edite o arquivo `.env` com suas credenciais:
```env
AZURE_OPENAI_KEY=sua_chave_openai
AZURE_ENDPOINT=seu_endpoint_openai
TRANSLATOR_API_KEY=sua_chave_translator
TRANSLATOR_ENDPOINT=seu_endpoint_translator
TRANSLATOR_LOCATION=sua_localizacao_translator
```

6. Execute a aplicação:
```bash
poetry run streamlit run desafios_de_projeto/desafio_1/src/app.py
```
7. Local URL: http://localhost:8501
	   


## 🎯 Conclusão e Aprendizados
[🔝 Voltar ao índice](#-índice)

Durante o desenvolvimento deste projeto, enfrei o desafio de criar uma solução que não apenas traduzisse conteúdo, mas o fizesse de maneira inteligente e contextual. A jornada me levou a explorar diferentes APIs da Azure e integrar múltiplas tecnologias em uma única aplicação coesa.




### 🚀 Próximos Passos:
 

Este projeto não é apenas uma ferramenta de tradução, mas um exemplo de como tecnologias modernas podem ser combinadas para criar soluções empresariais robustas e escaláveis.
