import json
from urllib.request import urlopen

with urlopen('http://www.apilayer.net/api/live?access_key=3bbab5c7e47927796b4fb5f9c389a7de') as response:
    source = response.read()
data = json.loads(source)
usd_rates = dict()
for moedas, valores in data['quotes'].items():
    usd_rates[moedas] = valores

print(f'Convertendo 1 Dólar(USD) para Reais(BRL) => {usd_rates["USDBRL"]}')
print(f'Convertendo 1 Dólar(USD) para Pesos(ARS) => {usd_rates["USDARS"]}')
print(f'Convertendo 1 Dólar(USD) para Euros(EUR) => {usd_rates["USDEUR"]}')
print(f'Convertendo 1 Dólar(USD) para Libras(GBP) => {usd_rates["USDGBP"]}')
print(f'Convertendo 1 Dólar(USD) para Yuan(CNY) => {usd_rates["USDCNY"]}')
