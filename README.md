# AnalytcsSentiment
Análise de Sentimentos em Mídias Sociais
# Extração (usando web scraping)
from bs4 import BeautifulSoup
import requests

url = 'https://exemplo.com/pagina-de-posts'
response = requests.get(url)
soup = BeautifulSoup(response.text, 'html.parser')
posts = soup.find_all('div', class_='post-content')

# Transformação
for post in posts:
    texto = post.get_text()
    # Realize as transformações necessárias, como análise de sentimentos ou extração de palavras-chave

# Carga
# Armazene os resultados em um banco de dados ou gere relatórios

# Extração (usando web scraping)
import requests
from bs4 import BeautifulSoup

url = 'https://exemplo.com/produto'
response = requests.get(url)
soup = BeautifulSoup(response.text, 'html.parser')
preco = soup.find('span', class_='price').text

# Transformação
# Compare preços, calcule médias, etc.

# Carga
# Armazene informações de preços em um banco de dados ou emita alertas
