
# 0. Configurar ambiente

## Iniciar o ambiente
python3 -m venv venv

## Ativar o ambiente
source venv/bin/activate

## Instalar as bibliotecas
pip install langchain langchain-openai langchain-google-genai python-dotenv beautifulsoup4 pypdf

## Gerar o requirements.txt
pip freeze > requirements.txt

## Pegar api key do google AI Studio
google => https://aistudio.google.com/apikey

openai => https://platform.openai.com/settings/organization/api-keys

## Executar o programa
python3 <arquivo>

# 2. Chains e processamento

## Sumarização

stuff=>Reduz tudo de uma vez
map_reduce=>Reduz cada parte em blocos e depois faz um resumo do resumo. 
Exemplo: 
-> Capitulo 1: Resumo do Capitulo 1
-> Capitulo 2: Resumo do Capitulo 2
-> Capitulo 3: Resumo do Capitulo 3
Resumo-> resumo dos 3 capitulos

Esse usa mais.

Na instrução load_summarize_chain(llm, chain_type="map_reduce", verbose=True), o verbose=True você consegue ver como que ele tá trabalhando e como ele tá pedindo para a llm e ele vai fazendo a chamada pra gente