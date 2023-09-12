# BRUNO-PROJETOO
 
# Node.js Express Server with MongoDB

Este é um exemplo de código Node.js que cria um servidor web usando o framework Express e se conecta a um banco de dados MongoDB. O servidor disponibiliza APIs para gerenciar clientes, produtos, funcionários e promoções.

## Pré-requisitos

- Node.js instalado
- MongoDB instalado e em execução localmente na porta padrão (27017)

## Instalação

1. Clone o repositório para o seu ambiente local.
2. Navegue até a pasta raiz do projeto.
3. Execute o seguinte comando para instalar as dependências:

```bash
npm install
```

## Configuração

Certifique-se de que o MongoDB esteja em execução na porta 27017. Você pode alterar a string de conexão no arquivo `server.js` se o MongoDB estiver em um host ou porta diferente.

## Uso

Para iniciar o servidor, execute o seguinte comando:

```bash
node server.js
```

O servidor estará em execução na porta 3000, a menos que a variável de ambiente `port` seja definida.

## Rotas

O servidor define várias rotas para diferentes recursos:

- `/clients`: Rotas para gerenciar clientes.
- `/products`: Rotas para gerenciar produtos.
- `/funcionarios`: Rotas para gerenciar funcionários.
- `/promocoes`: Rotas para gerenciar promoções.

Você pode acessar essas rotas por meio de chamadas HTTP, como GET, POST, PUT e DELETE, dependendo da funcionalidade que deseja realizar.

## Exemplo de Uso

Aqui está um exemplo de como acessar a API para obter a lista de clientes:

```bash
curl http://localhost:3000/clients
```

## Contribuição

Sinta-se à vontade para contribuir com melhorias neste projeto. Basta criar um fork e enviar um pull request.

## Licença

Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.



# API de Gerenciamento de Clientes

Esta API é responsável por gerenciar clientes em um sistema. Ela fornece operações básicas como criar, recuperar, atualizar e excluir clientes.

## Endpoints

### 1. Obter todos os Clientes

- **URL**: `/clients`
- **Método**: `GET`
- **Resposta de Sucesso**: Retorna uma lista de clientes.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 2. Obter um Cliente por ID

- **URL**: `/clients/:id`
- **Método**: `GET`
- **Parâmetros de URL**: `id` (Matrícula do Cliente)
- **Resposta de Sucesso**: Retorna os detalhes do cliente especificado.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 3. Criar um Cliente

- **URL**: `/clients`
- **Método**: `POST`
- **Corpo da Requisição**: Deve conter os detalhes do novo cliente.
- **Resposta de Sucesso**: Retorna uma mensagem de confirmação de criação do cliente.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 4. Atualizar um Cliente

- **URL**: `/clients`
- **Método**: `PUT`
- **Corpo da Requisição**: Deve conter os detalhes atualizados do cliente.
- **Resposta de Sucesso**: Retorna uma mensagem de confirmação de atualização do cliente.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 5. Excluir um Cliente

- **URL**: `/clients/:id`
- **Método**: `DELETE`
- **Parâmetros de URL**: `id` (Matrícula do Cliente)
- **Resposta de Sucesso**: Retorna uma mensagem de confirmação de exclusão do cliente.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

## Executando a Aplicação

Antes de iniciar a aplicação, certifique-se de ter Node.js e MongoDB instalados. Em seguida, siga os passos abaixo:

1. Clone o repositório para o seu ambiente local.
2. Navegue até a pasta raiz do projeto.
3. Execute o comando `npm install` para instalar as dependências.
4. Inicie o servidor com o comando `node server.js`.

A API estará disponível em `http://localhost:3000`.

## Contribuição

Sinta-se à vontade para contribuir com melhorias neste projeto. Basta criar um fork e enviar um pull request.

## Licença

Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.


# API de Gerenciamento de Funcionários

Esta API é responsável por gerenciar funcionários em um sistema. Ela fornece operações básicas como criar, recuperar, atualizar e excluir funcionários.

## Endpoints

### 1. Obter todos os Funcionários

- **URL**: `/funcionarios`
- **Método**: `GET`
- **Resposta de Sucesso**: Retorna uma lista de funcionários.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 2. Obter um Funcionário por ID

- **URL**: `/funcionarios/:id`
- **Método**: `GET`
- **Parâmetros de URL**: `id` (Matrícula do Funcionário)
- **Resposta de Sucesso**: Retorna os detalhes do funcionário especificado.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 3. Criar um Funcionário

- **URL**: `/funcionarios`
- **Método**: `POST`
- **Corpo da Requisição**: Deve conter os detalhes do novo funcionário.
- **Resposta de Sucesso**: Retorna uma mensagem de confirmação de criação do funcionário.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 4. Atualizar um Funcionário

- **URL**: `/funcionarios`
- **Método**: `PUT`
- **Corpo da Requisição**: Deve conter os detalhes atualizados do funcionário.
- **Resposta de Sucesso**: Retorna uma mensagem de confirmação de atualização do funcionário.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 5. Excluir um Funcionário

- **URL**: `/funcionarios/:id`
- **Método**: `DELETE`
- **Parâmetros de URL**: `id` (Matrícula do Funcionário)
- **Resposta de Sucesso**: Retorna uma mensagem de confirmação de exclusão do funcionário.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

## Executando a Aplicação

Antes de iniciar a aplicação, certifique-se de ter Node.js e MongoDB instalados. Em seguida, siga os passos abaixo:

1. Clone o repositório para o seu ambiente local.
2. Navegue até a pasta raiz do projeto.
3. Execute o comando `npm install` para instalar as dependências.
4. Inicie o servidor com o comando `node server.js`.

A API estará disponível em `http://localhost:3000`.

## Contribuição

Sinta-se à vontade para contribuir com melhorias neste projeto. Basta criar um fork e enviar um pull request.

## Licença

Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.


# API de Gerenciamento de Produtos

Esta API é responsável por gerenciar produtos em um sistema. Ela fornece operações básicas como criar, recuperar, atualizar e excluir produtos.

## Endpoints

### 1. Obter todos os Produtos

- **URL**: `/products`
- **Método**: `GET`
- **Resposta de Sucesso**: Retorna uma lista de produtos.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 2. Obter um Produto por ID

- **URL**: `/products/:id`
- **Método**: `GET`
- **Parâmetros de URL**: `id` (Identificador do Produto)
- **Resposta de Sucesso**: Retorna os detalhes do produto especificado.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 3. Criar um Produto

- **URL**: `/products`
- **Método**: `POST`
- **Corpo da Requisição**: Deve conter os detalhes do novo produto.
- **Resposta de Sucesso**: Retorna uma mensagem de confirmação de criação do produto.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 4. Atualizar um Produto

- **URL**: `/products`
- **Método**: `PUT`
- **Corpo da Requisição**: Deve conter os detalhes atualizados do produto.
- **Resposta de Sucesso**: Retorna uma mensagem de confirmação de atualização do produto.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 5. Excluir um Produto

- **URL**: `/products/:id`
- **Método**: `DELETE`
- **Parâmetros de URL**: `id` (Identificador do Produto)
- **Resposta de Sucesso**: Retorna uma mensagem de confirmação de exclusão do produto.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

## Executando a Aplicação

Antes de iniciar a aplicação, certifique-se de ter Node.js e MongoDB instalados. Em seguida, siga os passos abaixo:

1. Clone o repositório para o seu ambiente local.
2. Navegue até a pasta raiz do projeto.
3. Execute o comando `npm install` para instalar as dependências.
4. Inicie o servidor com o comando `node server.js`.

A API estará disponível em `http://localhost:3000`.

## Contribuição

Sinta-se à vontade para contribuir com melhorias neste projeto. Basta criar um fork e enviar um pull request.

## Licença

Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.


# API de Gerenciamento de Promoções

Esta API é responsável por gerenciar promoções em um sistema. Ela fornece operações básicas como criar, recuperar, atualizar e excluir promoções.

## Endpoints

### 1. Obter todas as Promoções

- **URL**: `/promocoes`
- **Método**: `GET`
- **Resposta de Sucesso**: Retorna uma lista de promoções.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 2. Obter uma Promoção por ID

- **URL**: `/promocoes/:id`
- **Método**: `GET`
- **Parâmetros de URL**: `id` (Identificador da Promoção)
- **Resposta de Sucesso**: Retorna os detalhes da promoção especificada.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 3. Criar uma Promoção

- **URL**: `/promocoes`
- **Método**: `POST`
- **Corpo da Requisição**: Deve conter os detalhes da nova promoção.
- **Resposta de Sucesso**: Retorna uma mensagem de confirmação de criação da promoção.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 4. Atualizar uma Promoção

- **URL**: `/promocoes`
- **Método**: `PUT`
- **Corpo da Requisição**: Deve conter os detalhes atualizados da promoção.
- **Resposta de Sucesso**: Retorna uma mensagem de confirmação de atualização da promoção.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

### 5. Excluir uma Promoção

- **URL**: `/promocoes/:id`
- **Método**: `DELETE`
- **Parâmetros de URL**: `id` (Identificador da Promoção)
- **Resposta de Sucesso**: Retorna uma mensagem de confirmação de exclusão da promoção.
- **Resposta de Erro**: Retorna uma mensagem de erro se a operação falhar.

## Executando a Aplicação

Antes de iniciar a aplicação, certifique-se de ter Node.js e MongoDB instalados. Em seguida, siga os passos abaixo:

1. Clone o repositório para o seu ambiente local.
2. Navegue até a pasta raiz do projeto.
3. Execute o comando `npm install` para instalar as dependências.
4. Inicie o servidor com o comando `node server.js`.

A API estará disponível em `http://localhost:3000`.

## Contribuição

Sinta-se à vontade para contribuir com melhorias neste projeto. Basta criar um fork e enviar um pull request.

## Licença

Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.


# Modelo de Cliente para MongoDB

Este é um modelo de cliente para uso com o MongoDB, definido com a biblioteca Mongoose. Ele descreve a estrutura dos documentos de cliente que podem ser armazenados no banco de dados MongoDB.

## Campos do Cliente

- `name` (String, obrigatório): O nome do cliente.
- `age` (Número, opcional): A idade do cliente, com um limite mínimo de 18 e máximo de 150 anos.
- `password` (String + Número, obrigatório e exclusivo): A senha do cliente, que deve ser única.
- `email` (String + Número, obrigatório e exclusivo): O endereço de e-mail do cliente, que deve ser único.
- `course` (String, opcional): O curso associado ao cliente.

## Como Usar o Modelo

Este modelo pode ser usado para criar, recuperar, atualizar e excluir registros de cliente no MongoDB. Você pode importá-lo em seus arquivos Node.js para interagir com o banco de dados.

Exemplo de uso para criar um novo cliente:

```javascript
const ClientModel = require('./clientModel');

const newClient = new ClientModel({
    name: 'Nome do Cliente',
    age: 25,
    password: 'senha123',
    email: 'cliente@email.com',
    course: 'Curso do Cliente'
});

newClient.save()
    .then((result) => {
        console.log('Cliente criado com sucesso:', result);
    })
    .catch((error) => {
        console.error('Erro ao criar cliente:', error);
    });
```

Lembre-se de que este é apenas o modelo de cliente. Você precisará criar as rotas e controladores correspondentes para interagir com este modelo por meio de uma API RESTful, se necessário.

## Licença

Este modelo está disponível sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.


# Modelo de Funcionário para MongoDB

Este é um modelo de funcionário para uso com o MongoDB, definido com a biblioteca Mongoose. Ele descreve a estrutura dos documentos de funcionário que podem ser armazenados no banco de dados MongoDB.

## Campos do Funcionário

- `name` (String, obrigatório): O nome do funcionário.
- `age` (Número, opcional): A idade do funcionário, com um limite mínimo de 18 e máximo de 150 anos.
- `wage` (Número, obrigatório e exclusivo): O salário do funcionário, que deve ser único.
- `course` (String, opcional): O curso associado ao funcionário.

## Como Usar o Modelo

Este modelo pode ser usado para criar, recuperar, atualizar e excluir registros de funcionário no MongoDB. Você pode importá-lo em seus arquivos Node.js para interagir com o banco de dados.

Exemplo de uso para criar um novo funcionário:

```javascript
const FuncionarioModel = require('./funcionarioModel');

const newFuncionario = new FuncionarioModel({
    name: 'Nome do Funcionário',
    age: 30,
    wage: 50000,
    course: 'Curso do Funcionário'
});

newFuncionario.save()
    .then((result) => {
        console.log('Funcionário criado com sucesso:', result);
    })
    .catch((error) => {
        console.error('Erro ao criar funcionário:', error);
    });
```

Lembre-se de que este é apenas o modelo de funcionário. Você precisará criar as rotas e controladores correspondentes para interagir com este modelo por meio de uma API RESTful, se necessário.

## Licença

Este modelo está disponível sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.


# Modelo de Produto para MongoDB

Este é um modelo de produto para uso com o MongoDB, definido com a biblioteca Mongoose. Ele descreve a estrutura dos documentos de produto que podem ser armazenados no banco de dados MongoDB.

## Campos do Produto

- `name` (String, obrigatório): O nome do produto.
- `price` (Número, opcional): O preço do produto, com um limite mínimo de 6 e máximo de 150 unidades monetárias.
- `type` (String, obrigatório): O tipo do produto.
- `course` (String, opcional): O curso associado ao produto.

## Como Usar o Modelo

Este modelo pode ser usado para criar, recuperar, atualizar e excluir registros de produto no MongoDB. Você pode importá-lo em seus arquivos Node.js para interagir com o banco de dados.

Exemplo de uso para criar um novo produto:

```javascript
const ProductModel = require('./productModel');

const newProduct = new ProductModel({
    name: 'Nome do Produto',
    price: 50,
    type: 'Tipo do Produto',
    course: 'Curso do Produto'
});

newProduct.save()
    .then((result) => {
        console.log('Produto criado com sucesso:', result);
    })
    .catch((error) => {
        console.error('Erro ao criar produto:', error);
    });
```

Lembre-se de que este é apenas o modelo de produto. Você precisará criar as rotas e controladores correspondentes para interagir com este modelo por meio de uma API RESTful, se necessário.

## Licença

Este modelo está disponível sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.


# Modelo de Promoção para MongoDB

Este é um modelo de promoção para uso com o MongoDB, definido com a biblioteca Mongoose. Ele descreve a estrutura dos documentos de promoção que podem ser armazenados no banco de dados MongoDB.

## Campos da Promoção

- `name` (String, obrigatório): O nome da promoção.
- `price` (Número, opcional): O preço da promoção, com um limite mínimo de 2 e máximo de 150 unidades monetárias.
- `type` (String, obrigatório): O tipo da promoção.
- `course` (String, opcional): O curso associado à promoção.

## Como Usar o Modelo

Este modelo pode ser usado para criar, recuperar, atualizar e excluir registros de promoção no MongoDB. Você pode importá-lo em seus arquivos Node.js para interagir com o banco de dados.

Exemplo de uso para criar uma nova promoção:

```javascript
const PromocaoModel = require('./promocaoModel');

const newPromocao = new PromocaoModel({
    name: 'Nome da Promoção',
    price: 10,
    type: 'Tipo da Promoção',
    course: 'Curso da Promoção'
});

newPromocao.save()
    .then((result) => {
        console.log('Promoção criada com sucesso:', result);
    })
    .catch((error) => {
        console.error('Erro ao criar promoção:', error);
    });
```

Lembre-se de que este é apenas o modelo de promoção. Você precisará criar as rotas e controladores correspondentes para interagir com este modelo por meio de uma API RESTful, se necessário.

## Licença

Este modelo está disponível sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.


# Rotas da API de Clientes

Este arquivo define as rotas da API de gerenciamento de clientes usando o framework Express.js. As rotas permitem que os clientes sejam criados, recuperados, atualizados e excluídos no sistema.

## Endpoints

### 1. Obter todos os Clientes

- **URL**: `/api/clients`
- **Método**: `GET`
- **Controlador**: `clientController.getClient`
- **Descrição**: Retorna uma lista de todos os clientes cadastrados no sistema.

### 2. Criar um Cliente

- **URL**: `/api/clients`
- **Método**: `POST`
- **Controlador**: `clientController.createClient`
- **Descrição**: Cria um novo cliente com base nos dados fornecidos no corpo da solicitação.

### 3. Atualizar um Cliente

- **URL**: `/api/clients`
- **Método**: `PUT`
- **Controlador**: `clientController.updateClient`
- **Descrição**: Atualiza as informações de um cliente com base nos dados fornecidos no corpo da solicitação.

### 4. Obter um Cliente por ID

- **URL**: `/api/clients/:id`
- **Método**: `GET`
- **Controlador**: `clientController.getClient`
- **Descrição**: Retorna os detalhes de um cliente específico com base em seu ID.

### 5. Excluir um Cliente por ID

- **URL**: `/api/clients/:id`
- **Método**: `DELETE`
- **Controlador**: `clientController.deleteClientById`
- **Descrição**: Exclui um cliente específico com base em seu ID.

## Como Usar as Rotas

As rotas estão definidas no arquivo `clientRouter.js` e podem ser usadas em conjunto com o controlador `clientController.js` para implementar as operações de gerenciamento de clientes em sua aplicação.

## Licença

Este código está disponível sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.


# Rotas da API de Funcionários

Este arquivo define as rotas da API de gerenciamento de funcionários usando o framework Express.js. As rotas permitem que os funcionários sejam criados, recuperados, atualizados e excluídos no sistema.

## Endpoints

### 1. Obter todos os Funcionários

- **URL**: `/api/funcionarios`
- **Método**: `GET`
- **Controlador**: `funcionarioController.getFuncionario`
- **Descrição**: Retorna uma lista de todos os funcionários cadastrados no sistema.

### 2. Criar um Funcionário

- **URL**: `/api/funcionarios`
- **Método**: `POST`
- **Controlador**: `funcionarioController.createFuncionario`
- **Descrição**: Cria um novo funcionário com base nos dados fornecidos no corpo da solicitação.

### 3. Atualizar um Funcionário

- **URL**: `/api/funcionarios`
- **Método**: `PUT`
- **Controlador**: `funcionarioController.updateFuncionario`
- **Descrição**: Atualiza as informações de um funcionário com base nos dados fornecidos no corpo da solicitação.

### 4. Obter um Funcionário por ID

- **URL**: `/api/funcionarios/:id`
- **Método**: `GET`
- **Controlador**: `funcionarioController.getFuncionario`
- **Descrição**: Retorna os detalhes de um funcionário específico com base em seu ID.

### 5. Excluir um Funcionário por ID

- **URL**: `/api/funcionarios/:id`
- **Método**: `DELETE`
- **Controlador**: `funcionarioController.deleteFuncionarioById`
- **Descrição**: Exclui um funcionário específico com base em seu ID.

## Como Usar as Rotas

As rotas estão definidas no arquivo `funcionarioRouter.js` e podem ser usadas em conjunto com o controlador `funcionarioController.js` para implementar as operações de gerenciamento de funcionários em sua aplicação.

## Licença

Este código está disponível sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.


# Rotas da API de Produtos

Este arquivo define as rotas da API de gerenciamento de produtos usando o framework Express.js. As rotas permitem que os produtos sejam criados, recuperados, atualizados e excluídos no sistema.

## Endpoints

### 1. Obter todos os Produtos

- **URL**: `/api/students`
- **Método**: `GET`
- **Controlador**: `productController.getProduct`
- **Descrição**: Retorna uma lista de todos os produtos cadastrados no sistema.

### 2. Criar um Produto

- **URL**: `/api/students`
- **Método**: `POST`
- **Controlador**: `productController.createProduct`
- **Descrição**: Cria um novo produto com base nos dados fornecidos no corpo da solicitação.

### 3. Atualizar um Produto

- **URL**: `/api/students`
- **Método**: `PUT`
- **Controlador**: `productController.updateProduct`
- **Descrição**: Atualiza as informações de um produto com base nos dados fornecidos no corpo da solicitação.

### 4. Obter um Produto por ID

- **URL**: `/api/products/:id`
- **Método**: `GET`
- **Controlador**: `productController.getProduct`
- **Descrição**: Retorna os detalhes de um produto específico com base em seu ID.

### 5. Excluir um Produto por ID

- **URL**: `/api/products/:id`
- **Método**: `DELETE`
- **Controlador**: `productController.deleteProductById`
- **Descrição**: Exclui um produto específico com base em seu ID.

## Como Usar as Rotas

As rotas estão definidas no arquivo `productRouter.js` e podem ser usadas em conjunto com o controlador `productController.js` para implementar as operações de gerenciamento de produtos em sua aplicação.

## Licença

Este código está disponível sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.


# Rotas da API de Promoções

Este arquivo define as rotas da API de gerenciamento de promoções usando o framework Express.js. As rotas permitem que as promoções sejam criadas, recuperadas, atualizadas e excluídas no sistema.

## Endpoints

### 1. Obter todas as Promoções

- **URL**: `/api/promocaos`
- **Método**: `GET`
- **Controlador**: `promocaoController.getPromocao`
- **Descrição**: Retorna uma lista de todas as promoções cadastradas no sistema.

### 2. Criar uma Promoção

- **URL**: `/api/promocaos`
- **Método**: `POST`
- **Controlador**: `promocaoController.createPromocao`
- **Descrição**: Cria uma nova promoção com base nos dados fornecidos no corpo da solicitação.

### 3. Atualizar uma Promoção

- **URL**: `/api/promocaos`
- **Método**: `PUT`
- **Controlador**: `promocaoController.updatePromocao`
- **Descrição**: Atualiza as informações de uma promoção com base nos dados fornecidos no corpo da solicitação.

### 4. Obter uma Promoção por ID

- **URL**: `/api/promocaos/:id`
- **Método**: `GET`
- **Controlador**: `promocaoController.getPromocao`
- **Descrição**: Retorna os detalhes de uma promoção específica com base em seu ID.

### 5. Excluir uma Promoção por ID

- **URL**: `/api/promocaos/:id`
- **Método**: `DELETE`
- **Controlador**: `promocaoController.deletePromocaoById`
- **Descrição**: Exclui uma promoção específica com base em seu ID.

## Como Usar as Rotas

As rotas estão definidas no arquivo `promocaoRouter.js` e podem ser usadas em conjunto com o controlador `promocaoController.js` para implementar as operações de gerenciamento de promoções em sua aplicação.

## Licença

Este código está disponível sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.
