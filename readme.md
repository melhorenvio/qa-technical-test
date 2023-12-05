Teste técnico Analista de Qaulidade Melhor Envio

O Candidato deve realizar as tarefas descritas abaixo, recomenda-se o uso da ferramenta Cypress para execução das tarefas de automação.
O teste deverá ser entregue por meio de repositório privado no Github,que deverá ser compartilhado com os usuarios “ldseinhardt” e “wqsandoval”.

1 - Elaborar um levantamento de cenários, no formato de documento de texto, para a funcionalidade de cadastro acessivel em https://sandbox.melhorenvio.com.br/cadastre-se
	
2 - Desenvolver scripts de testes automatizados de interface para pelo menos 2 dos cenários levantados no passo 1. 

3 - Desenvolver scripts de teste automatizados de api na rota /users, para pelo menos 2 dos cenários levantados no passo 1.
	Informações do Endpoint:
		Method: POST
		Headers:{
			Accept: "application/json"
			Content-Type: "application/json"}
		Body:{"firstname":"Teste","lastname":"teste","email":"teste@teste.com","document":"71172405042","birthdate":"1990-01-01","phone_mobile":"51998989899","password":"a1a2a3a4a5a6","terms":true}

4 (opcional) - Incluir no projeto de automação uma solução de report de execução dos testes. 

5 (opcional) - Criar no repositorio Github um workflow via Github actions para executar os testes e reportar no Github Pages Automaticamente.
