<h1><span class="documentation_get">GET</span><span class="documentation_url">[api/v1/pokemon]</span> Pokédex</h1>

```http
https://api-pokemon-fr.vercel.app/api/v1/pokemon
```

Permet d'obtenir la liste de tous les Pokémons.<br>
[Exemple de donnés renvoyés.](https://api-pokemon-fr.vercel.app/api/v1/pokemon) 

## Curl
```curl
curl -XGET \
     -H 'User-Agent: RobotPokemon' \
     -H 'From: adresse[at]domaine[dot]com' \
     -H "Content-type: application/json" \
     'https://api-pokemon-fr.vercel.app/api/v1/pokemon'
```

## Python
```py
import requests

url = "https://api-pokemon-fr.vercel.app/api/v1/pokemon"
headers = {
    "User-Agent": "RobotPokemon",
    "From": "adresse[at]domaine[dot]com",
    'Content-type': 'application/json'
}

response = requests.get(url, headers=headers)

if response.status_code == 200:
    data = response.json()
    print(data)
else:
    print("La requête a échoué avec le code d'état:", response.status_code)
```