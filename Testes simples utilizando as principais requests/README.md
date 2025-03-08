# README da Coleção de API com testes simples utilizando as principais requisições

## Introdução
Este projeto contém uma coleção de requisições desenvolvidas para consumir a API pública disponível em [JSONPlaceholder](https://jsonplaceholder.typicode.com/). A coleção foi criada para demonstrar como interagir com a API, salvar valores e strings, e validar as respostas, incluindo os códigos de status HTTP.

## Objetivos
- Consumir a API JSONPlaceholder para realizar operações como criar, ler, atualizar e excluir dados.
- Salvar valores e strings em diferentes requisições.
- Validar as respostas recebidas da API e verificar os códigos de status retornados.

## Exemplos para as validações dos testes
- Validar o status code;

```javascript
pm.test("Status code is 200", function () {
        pm.response.to.have.status(200);
      });
```

- Obter o response da requisição;

```javascript  
const response = pm.response.json();
```

- Salvar variáveis do response como o id, para utilizar em pontos específicos da collection

```javascript  
pm.environment.set("idCadastro", response.id);
```

## Estrutura da Coleção
A coleção inclui as seguintes requisições:

- **GET /posts**: Recupera uma lista de postagens.
- **GET /posts/{id}**: Recupera uma postagem específica pelo ID.
- **POST /posts**: Cria uma nova postagem e salva um objeto.
- **PUT /posts/{id}**: Atualiza uma postagem existente pelo ID.
- **DELETE /posts/{id}**: Exclui uma postagem pelo ID.

## Validação das Respostas
Cada requisição na coleção inclui testes para validar:
- Se a resposta está no formato JSON esperado.
- Se os valores retornados correspondem aos dados esperados.
- Se o código de status da resposta está correto (por exemplo, 200 OK para operações bem-sucedidas e 201 Created para uma nova criação).

## Como Usar
1. **Clone o repositório** ou baixe a coleção em formato JSON.
2. **Importe a coleção** no Postman, usando a opção de importação.
3. Execute as requisições conforme necessário e observe as respostas e os testes.

## Conclusão
Esta coleção é uma maneira prática de entender como interagir com APIs RESTful utilizando a API JSONPlaceholder. Em caso de dúvidas ou feedback, sinta-se à vontade para entrar em contato.