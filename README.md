![Melhor Envio](https://public.melhorenvio.com.br/images/logo-azul.png)

## Teste técnico Analista de Qualidade Melhor Envio

# Instruções
- Realizar as tarefas descritas abaixo, devendo ser entregue por meio de repositório privado no Github compartilhado com os usuarios “ldseinhardt” , “wqsandoval”.
- Recomenda-se o uso da ferramenta Cypress para execução das tarefas de automação.
- O prazo para execução das tarefas é de 4 dias.
- Em caso de duvidas, entre em contato com : william.sandoval@melhorenvio.com, luan.einhardt@melhorenvio.com

# Tarefas
- 1 : Elaborar um levantamento de cenários para a funcionalidade de cadastro, acessível em https://sandbox.melhorenvio.com.br/cadastre-se, utilizando a sintaxe Gherkin.

- 2 : Desenvolver scripts de testes automatizados de interface para pelo menos 2 dos cenários levantados no passo 1.

- 3 : Desenvolver scripts de testes automatizados de api na rota de cadastro para os seguintes cenários:
	
	1 : Ao enviar um payload válido, verificar que a resposta tem um status code 201 e contém a propriedade token preenchida.
	2 : Ao enviar um payload sem a propriedade document, verificar que a resposta tem um status code 422 e retorna uma mensagem de erro indicando a obrigatoriedade do CPF.

 
	Informações do Endpoint:
		URL:"https://sandbox.melhorenvio.com.br/api/v2/users"
		Method: POST
		Headers: {
			Accept: "application/json",
			Content-Type: "application/json"
		}
		Payload exemplo :{"firstname":"Teste","lastname":"teste","email":"teste@teste.com","document":"71172405042","birthdate":"1990-01-01","phone_mobile":"51998989899","password":"a1a2a3a4a5a6","terms":true}
	 
- 4 : Criar no repositório Github um workflow via Github actions para executar os testes e exportar relatorio ao final da execução.
- 5 : Utilizando a ferramenta K6, gerar um script de teste de performance seguindo as seguintes especificações :
	- URL : https://test.k6.io/pi.php?decimals=100
	- Method : GET
	- Carga inicial de 5 requests por segundo durante 10 segundos,subindo a 10 requests por segundo nos próximos 30 segundos e descendo a 2 requests por segundo por mais 60 segundos.
	- O teste deve ser falhar se o tempo de resposta MEDIO for superior a 2 segundos ou se a taxa de sucesso for menor que 95%.
 
- 6: Criar um Workflow no repositorio github para executar o teste de performance e exportar relatorio ao final da execução.
	
