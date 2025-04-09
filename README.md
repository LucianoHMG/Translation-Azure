
# Tradutor Multifuncional

Uma aplicação web que integra duas poderosas ferramentas de tradução em uma única plataforma, focada em proporcionar uma excelente experiência ao usuário com resultados precisos e contextualizados.

---

## 📑 Índice

- [📁 Estrutura do Projeto](#-estrutura-do-projeto)
- [📋 Sobre o Projeto](#-sobre-o-projeto)
  - [🎯 Tradutor de Artigos](#-tradutor-de-artigos)
  - [📄 Tradutor de Documentos](#-tradutor-de-documentos)
- [🚀 Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [📦 Requisitos](#-requisitos)
- [⚙️ Instalação e Execução](#-instalação-e-execução)
  - [💻 Execução Local com Poetry](#-execução-local-com-poetry)
- [🎯 Conclusão e Aprendizados](#-conclusão-e-aprendizados)
  - [🚀 Próximos Passos](#-próximos-passos)

---

## 📋 Sobre o Projeto

O **Tradutor Multifuncional** é uma aplicação web que reúne duas ferramentas de tradução integradas em uma única interface. Desenvolvida com foco na experiência do usuário e na qualidade dos resultados, a solução foi pensada para atender demandas diversas de tradução em ambientes profissionais.

### 🎯 Tradutor de Artigos

Utiliza a avançada API do Azure OpenAI (GPT-4o mini) para oferecer traduções precisas e contextualmente relevantes de artigos web. Entre suas principais funcionalidades, destacam-se:

- **Extração automática:** Coleta o conteúdo diretamente de URLs.
- **Preservação de Formatação:** Mantém a formatação markdown do texto original.
- **Multi-idioma:** Suporte à tradução para diversos idiomas.
- **Download:** Permite baixar o arquivo traduzido.
- **Interface Responsiva:** Design intuitivo e adaptável a diferentes dispositivos.

### 📄 Tradutor de Documentos

Baseado na Azure Translator API, este módulo proporciona tradução profissional de documentos Word (.docx) com os seguintes destaques:

- **Compatibilidade:** Suporte nativo para arquivos .docx.
- **Pares de Idiomas:** Traduz entre múltiplos idiomas.
- **Formatação Preservada:** Mantém a formatação original do documento.
- **Download Rápido:** Possibilita o download do documento já traduzido.
- **Interface Amigável:** Processo de upload simples e intuitivo.

---

## 🚀 Tecnologias Utilizadas

**Core:**
- Python
- Azure OpenAI
- Azure Translator

**Principais Bibliotecas:**
- `python-docx` – Manipulação de documentos Word
- `beautifulsoup4` – Extração de conteúdo web
- `python-dotenv` – Gerenciamento de variáveis de ambiente

---

## 📦 Requisitos

- Python (versão compatível com o projeto)
- Poetry (para gerenciamento de dependências)
- Conta Azure com acesso às APIs:
  - Azure OpenAI
  - Azure Translator

---

## ⚙️ Instalação e Execução

### 💻 Execução Local com Poetry

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/Jcnok/Bootcamp-Microsoft-Certification-Challenge--1-AI_102.git

2. Navegue até a pasta do repositório:

cd Bootcamp-Microsoft-Certification-Challenge--1-AI_102


3. Instale o Poetry (caso não esteja instalado):

curl -sSL https://install.python-poetry.org | python3 -


4. Configure o ambiente virtual e instale as dependências:

poetry install


5. Configure as variáveis de ambiente:

cp .env.example .env

Em seguida, edite o arquivo .env inserindo suas credenciais:

AZURE_OPENAI_KEY=sua_chave_openai
AZURE_ENDPOINT=seu_endpoint_openai
TRANSLATOR_API_KEY=sua_chave_translator
TRANSLATOR_ENDPOINT=seu_endpoint_translator
TRANSLATOR_LOCATION=sua_localizacao_translator


6. Execute a aplicação:

poetry run streamlit run desafios_de_projeto/desafio_1/src/app.py


7. Acesse a aplicação via URL:

Abra o navegador e digite: http://localhost:8501





---

🎯 Conclusão e Aprendizados

Durante o desenvolvimento deste projeto, enfrentei o desafio de criar uma solução que não apenas traduzisse conteúdo, mas que também preservasse o contexto e a formatação dos textos originais. Essa jornada envolveu a exploração de diversas APIs da Azure e a integração de múltiplas tecnologias, resultando em uma aplicação coesa e robusta.

🚀 Próximos Passos

Este projeto não é apenas uma ferramenta de tradução, mas um exemplo de como tecnologias modernas podem ser combinadas para criar soluções escaláveis e empresariais. Futuramente, pretendo:

Integrar novas funcionalidades e suporte a outros tipos de documentos.

Otimizar ainda mais a interface do usuário.

Expandir o suporte a mais idiomas e modelos de tradução.

Investir em melhorias de performance e segurança.



---

Este README está alinhado com as melhores práticas de documentação e foi estruturado para facilitar a compreensão e a utilização do projeto por desenvolvedores e usuários finais.

---

### Notas de Atualização:
- A estrutura do documento foi mantida, mas os textos foram revisados para clareza e coesão.
- Foram adicionadas seções de "Próximos Passos" e melhorias na descrição dos módulos.
