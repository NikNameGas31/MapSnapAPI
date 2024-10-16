# MapSnapAPI
-Чтобы зарегаться
`
import requests

url = "http://127.0.0.1:8000/api/register/"
data = {
    "username": "nikita",
    "password": "securepassword123"
}

headers = {
    "Content-Type": "application/json"
}

response = requests.post(url, json=data, headers=headers)
print(f"Status Code: {response.status_code}")
print(response.json())
`

-Чтобы войти:
`
import requests

url = "http://127.0.0.1:8000/api/login/"
data = {
    "username": "nikita",
    "password": "securepassword123"
}

headers = {
    "Content-Type": "application/json"
}

response = requests.post(url, json=data, headers=headers)
print(f"Status Code: {response.status_code}")
print(response.json())
`

-Чтобы смотреть данные:
`
import requests

url = "http://127.0.0.1:8000/api/places/"
headers = {
    "Authorization": "Token b0af150890cf834008510c50c06397c0ca0dbcc4"
}

response = requests.get(url, headers=headers)
print(response.status_code)
print(response.json())
`

Остальное завтра