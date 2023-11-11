# Parte 1

# Parte 2 - Implantação de um website/frontend estático simples via AWS Amplify

Vídeo de referência: https://www.youtube.com/watch?v=7m_q1ldzw0U&t=808s


## Steps:

### 01 - Subir o arquivo index.html simples para o Amplify e demonstrar o funcionamento do serviço;

### 02 - Criar a função Lambda 01 e testar com um evento de teste simples afim de validar o funcionamento da função;

### 03 - Criar o API Gateway (REST) e testar a API com um body simples:
		Criar a API REST
		Criar o método POST integrnado com a Lambda correta
		Habilitar o CORS nesse método criado
		Deploy da API criando o stage correto (Copiar a URL do API Gateway em um bloco de notas)
		Testar a API com o mesmo json de teste da Lambda. Segue abaixo para referência:

```
{
	"base": 2,
	"exponent": 3
}
```



### 04 - Criar a tabelo do DynamoDB (Copiar o ARN da tabela em um bloco de notas)

### 05 - Atualizar a Lambda com a nova função contemplando o DynamoDB e alterar a Role da Lambda com as permissões necessárias (Colar a ARN da tabela do DynamoDB na política de permissão)

### 06 - Testar a Lambda com o mesmo evento de teste e mostrar os itens registrados na tabela do DynamoDB

### 07 - Atualizar o index.html do Amplify passando a URL do API Gateway e fazer novo upload

### 08 - Testar no browser

## Observacões:

**Ao subir os códigos para o Amplify sem um provedor de git, os arquivos precisam estar zipados e o index deve ter o nome apenas de index.html. Qualquer coisa diferente, o amplify fará o deploy e o frontend não se comportará da forma esperada. Acredite em mim ;)**

