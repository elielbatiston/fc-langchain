
# 1. Configurar ambiente

## Iniciar o ambiente
python3 -m venv venv

## Ativar o ambiente
source venv/bin/activate

## Instalar as bibliotecas
pip install langchain langchain-openai langchain-google-genai python-dotenv beautifulsoup4 pypdf

## Gerar o requirements.txt
pip freeze > requirements.txt

# 2. Pegar api key do google AI Studio
google => https://aistudio.google.com/apikey

openai => https://platform.openai.com/settings/organization/api-keys

# 3. Executar o programa
python3 <arquivo>