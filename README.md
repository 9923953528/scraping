# scraping
#web scraping program
import requests
import re
from bs4 import BeautifulSoup
url='https://www.commonfloor.com/listing-search?city=Bangalore&cg=Bangalore%20division&iscg=&search_intent=sale&polygon=1&page=1&page_size=30'
res = requests.get(url)
html_page = res.content
soup = BeautifulSoup(html_page, 'html.parser')
print(soup)
