![Melhor Envio](https://public.melhorenvio.com.br/images/logo-azul.png)

## Teste técnico Analista de Qualidade Melhor Envio

# Instruções
- Realizar as tarefas descritas abaixo, devendo ser entregue por meio de repositório privado no Github compartilhado com os usuarios “ldseinhardt” , “wqsandoval” e "mortalisnoia".
- Recomenda-se o uso da ferramenta Cypress para execução das tarefas de automação.
- O prazo para execução das tarefas é de 4 dias.
- Em caso de duvidas, entre em contato com : william.sandoval@melhorenvio.com, luan.einhardt@melhorenvio.com

# Tarefas
1 : Elaborar um levantamento de cenários para a funcionalidade de cadastro, acessível em https://sandbox.melhorenvio.com.br/cadastre-se, utilizando a sintaxe Gherkin.

2 : Desenvolver scripts de testes automatizados de interface para pelo menos 2 dos cenários levantados no passo 1.

3 : Desenvolver scripts de testes automatizados de api na rota de cadastro para os seguintes cenários:
	
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
	 
- 4 (opcional) : Incluir no projeto de automação uma solução de report de execução dos testes. 

- 5 (opcional) : Criar no repositório Github um workflow via Github actions para executar os testes e gerar reporta automaticamente.
