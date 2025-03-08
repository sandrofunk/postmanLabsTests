# Guia de Instalação e Uso do Postman

## Índice
- [O que é o Postman?](#o-que-é-o-postman)
- [Requisitos do Sistema](#requisitos-do-sistema)
- [Instalação do Postman](#instalação-do-postman)
    - [Windows](#windows)
    - [macOS](#macos)
    - [Linux](#linux)
    - [Postman na Web](#postman-na-web)
- [Criando uma Conta (opcional)](#criando-uma-conta-opcional)
- [Usando o Postman](#usando-o-postman)
    - [Criando uma Nova Requisição](#criando-uma-nova-requisição)
    - [Salvando Requisições](#salvando-requisições)
    - [Criando Coleções](#criando-coleções)
    - [Executando Testes](#executando-testes)
- [Exportando e Importando Coleções](#exportando-e-importando-coleções)
- [Recursos Adicionais](#recursos-adicionais)
- [Suporte](#suporte)

## O que é o Postman?
Postman é uma plataforma popular para o desenvolvimento e teste de APIs. Com o Postman, você pode enviar requisições HTTP para o seu servidor, visualizar as respostas, testar suas APIs e automatizar fluxos de trabalho de teste.

## Requisitos do Sistema
Antes de instalar o Postman, verifique se seu sistema atende aos seguintes requisitos:
- **Sistema Operacional**:
    - Windows 7 ou superior
    - macOS 10.10 ou superior
    - Distribuições Linux baseadas em Debian, Ubuntu, ou CentOS
- **Espaço em Disco**: Pelo menos 500 MB de espaço livre
- **Memória**: 2 GB de RAM

## Instalação do Postman

### Windows
1. Acesse a [página de download do Postman](https://www.postman.com/downloads/).
2. Clique no botão de download para Windows.
3. Após o download, execute o instalador (`Postman.exe`) e siga as instruções na tela para concluir a instalação.

### macOS
1. Acesse a [página de download do Postman](https://www.postman.com/downloads/).
2. Clique no botão de download para macOS.
3. Após o download, arraste o ícone do Postman para a pasta `Applications`.
4. Abra o Postman a partir da pasta `Applications`.

### Linux
1. Acesse a [página de download do Postman](https://www.postman.com/downloads/).
2. Escolha a versão mais recente para Linux (geralmente um arquivo `.tar.gz`).
3. Extraia o arquivo:
   ```bash
   tar -xzf Postman-linux-x64-x.x.x.tar.gz
   ```
4. Mova o extraído para o diretório apropriado:
   ```bash
   sudo mv Postman /opt/
   ```
5. Crie um link simbólico:
   ```bash
   sudo ln -s /opt/Postman/Postman /usr/bin/postman
   ```
6. Abra o Postman executando o comando `postman` no terminal.

### Postman na Web
1. Você também pode usar o [Postman na Web](https://app.postman.com/) acessando o link através de um navegador.
2. Não é necessário instalar nada; você pode usar sua conta Postman diretamente no navegador.

## Criando uma Conta (opcional)
Embora o uso do Postman seja possível sem uma conta, recomenda-se criar uma para salvar coleções, requisições e configurações na nuvem.
1. Ao abrir o Postman, clique em "Sign Up" ou "Log In" para criar ou acessar sua conta.

## Usando o Postman

### Criando uma Nova Requisição
1. Clique no botão `New` no canto superior esquerdo.
2. Selecione `Request`.
3. Insira um nome e escolha uma coleção para salvar a requisição.
4. Clique em `Save`.
5. Escolha o método HTTP (GET, POST, etc.), insira a URL da API e clique em `Send`.

### Salvando Requisições
Após uma requisição ser enviada, você pode salvar a requisição clicando em `Save` no canto superior direito da interface.

### Criando Coleções
As coleções permitem organizar suas requisições. Para criar uma nova coleção:
1. Clique em `New` e selecione `Collection`.
2. Dê um nome à coleção e, opcionalmente, adicione uma descrição.
3. Clique em `Create`.

### Executando Testes
Você pode escrever testes em JavaScript na aba de "Tests" após criar uma requisição. Por exemplo:
```javascript
pm.test("Código de status é 200", function () {
    pm.response.to.have.status(200);
});
```

Quando a requisição for enviada, os testes serão executados e os resultados serão exibidos na aba de "Test Results".

## Exportando e Importando Coleções
### Exportando uma Coleção
1. Clique com o botão direito na coleção que deseja exportar.
2. Selecione `Export`.
3. Escolha o formato e salve o arquivo JSON.

### Importando uma Coleção
1. Clique em `Import` no canto superior esquerdo.
2. Selecione o arquivo JSON que deseja importar.
3. A coleção aparecerá na sua lista de coleções.

## Recursos Adicionais
- [Documentação Oficial do Postman](https://learning.postman.com/docs/welcome/)
- [Postman Blog](https://blog.postman.com/)
- [Postman Community](https://community.postman.com/)

## Importante
Dentro de cada pasta, você encontrará exemplos distintos e documentos explicativos, que foram elaborados para facilitar sua compreensão sobre as funcionalidades do Postman. Esses materiais são essenciais para aproveitar ao máximo a ferramenta e aprimorar suas habilidades com APIs.

## Suporte
Se você tiver dúvidas ou precisar de suporte, sinta-se à vontade para entrar em contato pelo e-mail: **sagfunk@gmail.com**.