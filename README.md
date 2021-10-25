
# Boas vindas ao repositório do projeto Cookmaster!

## por que gosto desse projeto

além de um projeto desafiador, ele conta com várias tecnoligias e ferramentas muito interessantes onde fui capaz de:

- Entender o que há por dentro de um token de autenticação;

- Gerar tokens a partir de informações como login e senha;

- Autenticar rotas do Express, usando o token JWT;

- Fazer upload de arquivos em APIs REST;

- Salvar arquivos no servidor através de uma API REST;

- Consultar arquivos do servidor através de uma API REST.

---

## Instalação do projeto localmente

Após cada um dos passos, haverá um exemplo do comando a ser digitado para fazer o que está sendo pedido, caso tenha dificuldades e o exemplo não seja suficiente, não hesite em me contatar em _fabiomcjr@hotmail.com_.

1. Abra o terminal e crie um diretório no local de sua preferência com o comando **mkdir**:
```javascript
  mkdir projetos-fabio
```

2. Entre no diretório que acabou de criar e depois clone o projeto:
```javascript
  cd projetos-fabio
  git clone git@github.com:FabioMarturanoJr/cookmaster.git
```

3. Entre no diretório do projeto e instale as dependencias:
```javascript
  cd cookmaster/
  npm i
```

5. inicie o projeto:
```javascript
  npm start
```
---

## Rotas disponiveis

### `POST/users` cadastra usuário

espera no body:
```javascript
{
  "name": "nameUser",
  "email": "email@email.com",
  "password": "passwordUser",
}
```

### `POST/login` realiza login e retorna token JWT

espera no body:
```javascript
{
  "email": "email@email.com",
  "password": "passwordUser",
}
```

### `GET/recipes` retorna todas as receitas
  
### `GET/recipes/ID` retorna uma receita especifica
  
### `PUT/recipes/ID` atualiza receita especifica, valida token JWT 

espera no body:
```javascript
{
  "name": "recipeName",
  "ingredients": "ingredientList",
  "preparation": "preparationteps",
}
```

### `PUT/recipes/ID/image` cadastra imagem de receita ja existente, valida token JWT 

espera no body:
form-data KEY `image` e tipo `jpeg`

### `POST/recipes` cadastra uma receita, valida token JWT 

espera no body:
```javascript
{
  "name": "recipeName",
  "ingredients": "ingredientList",
  "preparation": "preparationteps",
}
```
### `DELETE/recipes/ID` excluir uma receita, valida token JWT 
