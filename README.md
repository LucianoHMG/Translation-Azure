# Translation-Azure 🚀

[![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)](https://azure.microsoft.com/)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![API](https://img.shields.io/badge/API-REST-blue?style=for-the-badge)](https://learn.microsoft.com/en-us/azure/cognitive-services/translator/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

## 📋 Descrição

**Tradutor Multifuncional** integrado com **Azure Cognitive Services (Translator API)**. Uma aplicação web que oferece traducões de alta qualidade com suporte a múltiplos idiomas, proporcionando uma excelente experiência ao usuário com resultados precisos e contextualizados.

### 🎯 Recursos Principais
- ✅ Integração com Azure Translator API
- ✅ Suporte para 100+ idiomas
- ✅ Interface web intuitiva e responsiva
- ✅ Tradução em tempo real
- ✅ Suporte a texto e URL
- ✅ Detecção automática de idioma

---

## 📦 Estrutura do Projeto

```
Translation-Azure/
├── README.md           # Este arquivo
├── app.py              # Aplicação Flask principal
├── requirements.txt    # Dependências Python
├── templates/          # Templates HTML
│  ├── index.html
│  └── resultado.html
├── static/             # CSS e JavaScript
│  ├── style.css
│  └── script.js
└── config.py           # Configuração de variáveis
```

---

## 🚀 Quick Start

### 1. Pré-requisitos
- Python 3.8+
- Conta Azure com Translator API criada
- Chave de acesso da Azure (API Key)

### 2. Clone o repositório
```bash
git clone https://github.com/LucianoHMG/Translation-Azure.git
cd Translation-Azure
```

### 3. Instale as dependências
```bash
pip install -r requirements.txt
```

### 4. Configure as variáveis de ambiente
```bash
# Crie um arquivo .env na raiz do projeto
echo "AZURE_API_KEY=sua_chave_aqui" > .env
echo "AZURE_REGION=eastus" >> .env
echo "FLASK_ENV=development" >> .env
```

### 5. Execute a aplicação
```bash
python app.py
```

Acesse em: `http://localhost:5000`

---

## 📊 Sobre o Projeto

Este projeto foi desenvolvido para demonstrar a integração com serviços cloud, especificamente **Azure Cognitive Services**. É um excelente exemplo de como utilizar APIs cloud para criar aplicações escalavéis e profissionais.

### O que faz:
1. Recebe texto em qualquer idioma
2. Detecta automaticamente o idioma de origem
3. Permite seleção do idioma de destino
4. Utiliza Azure Translator para traduzir
5. Exibe resultado com formatação clara

---

## 📊 Guia de Uso

### Interface Web
1. Acesse `http://localhost:5000`
2. Cole ou digite o texto a traduzir
3. Selecione o idioma de destino
4. Clique em "Traduzir"
5. Veja o resultado imediatamente

### Exemplo com cURL
```bash
curl -X POST http://localhost:5000/translate \
  -H "Content-Type: application/json" \
  -d '{"text": "Olá, mundo!", "target_language": "en"}'

# Resposta:
# {"translated_text": "Hello, world!", "source_language": "pt"}
```

---

## 😐 Tecnologias Utilizadas

| Tecnologia | Versão | Propósito |
|-----------|--------|----------|
| **Python** | 3.8+ | Backend |
| **Flask** | 2.x | Framework Web |
| **Azure Translator** | API | Serviço de Tradução |
| **HTML5** | - | Frontend |
| **CSS3** | - | Estilização |
| **JavaScript** | - | Interação |
| **Requests** | - | HTTP Client |

---

## 🎉 Casos de Uso

- 👤 Traducão de documentos
- 🌐 Localizacão de websites
- 📄 Tradução de conteúdo
- 🗣️ Assistente de suporte multilingué
- 👦 Ferramentas educacionais

---

## 🔐 Segurança

### ⚠️ Recomendações
1. **Não exponha a API Key** no código
2. Use **variáveis de ambiente** para credenciais
3. Implemente **rate limiting** para uso da API
4. Mantenha registros (logs) de traduções
5. Valide inputs do usuário

### Configuração de API Key
```bash
# NÃO FAÇA ISTO:
export AZURE_API_KEY="abc123def456"  # Inseguro!

# FAÇA ISTO:
# Use arquivo .env com python-dotenv
from dotenv import load_dotenv
load_dotenv()
api_key = os.getenv('AZURE_API_KEY')
```

---

## 📝 Exemplo de Configuração

### requirements.txt
```
Flask==2.3.0
requests==2.31.0
python-dotenv==1.0.0
```

### Variáveis de Ambiente
```bash
AZURE_API_KEY=sua_chave_da_azure
AZURE_REGION=eastus
FLASK_ENV=development
FLASK_DEBUG=True
```

---

## 📄 API Endpoints

### GET /
Página principal com formulário

### POST /translate
Realiza a tradução

**Request:**
```json
{
  "text": "Olá, mundo!",
  "target_language": "en"
}
```

**Response:**
```json
{
  "translated_text": "Hello, world!",
  "source_language": "pt",
  "target_language": "en",
  "confidence": 0.98
}
```

---

## 😧 Troubleshooting

### Erro: "Invalid API Key"
```bash
# Verifique se a chave está correta no .env
echo $AZURE_API_KEY

# Regenere a chave no portal Azure se necessário
```

### Erro: "Connection timeout"
```bash
# Verifique sua conexão com internet
# Verifique se a região Azure está correta
# Tente usar uma região diferente
```

### Erro: "Unsupported language"
```bash
# Consulte idiomas suportados:
# https://learn.microsoft.com/en-us/azure/cognitive-services/translator/language-support
```

---

## 🤝 Contribuindo

1. Faça um Fork do projeto
2. Crie uma branch (`git checkout -b feature/NewFeature`)
3. Commit suas mudanças (`git commit -m 'Add NewFeature'`)
4. Push (`git push origin feature/NewFeature`)
5. Abra um Pull Request

---

## ✅ TODO / Roadmap

- [ ] Adicionar cache de traduções
- [ ] Implementar histórico de traduções
- [ ] Adicionar suporte a upload de arquivos
- [ ] Criar versão mobile (React Native)
- [ ] Implementar testes automáticos
- [ ] Dashboard de analytics
- [ ] Suporte a múltiplos formatos (PDF, DOCX, etc)

---

## 📄 Licença

MIT License - veja [LICENSE](LICENSE) para detalhes.

---

## 👤 Autor

**Luciano Girão**
- GitHub: [@LucianoHMG](https://github.com/LucianoHMG)
- LinkedIn: [lucianogirão](https://www.linkedin.com/in/lucianogirão)

### 📚 Recursos Relacionados
- [Azure Translator Documentation](https://learn.microsoft.com/en-us/azure/cognitive-services/translator/)
- [Azure Cognitive Services](https://azure.microsoft.com/en-us/products/cognitive-services/)
- [Flask Documentation](https://flask.palletsprojects.com/)
- [REST API Best Practices](https://restfulapi.net/)

---

## ⭐ Se este projeto foi útil, dê uma star! ⭐

**Last Updated:** 2026-01-08
