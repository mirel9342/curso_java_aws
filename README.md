 ** 🚀 URL Shortener API **
 
 
 Um sistema de encurtamento e redirecionamento de URLs desenvolvido com AWS Serverless e Java, permitindo a criação de URLs curtas com um prazo de validade configurável. 

🛠️ Tecnologias Utilizadas
- Java: Linguagem de programação principal.
- AWS Lambda: Para execução de funções serverless.
- AWS S3: Para armazenamento das URLs encurtadas e seus metadados.
- AWS API Gateway: Para expor as APIs.
- AWS IAM: Para controle de permissões e segurança.
  
🔍 Como Funciona
1. Criação de URLs curtas
A API recebe a URL original e o tempo de expiração.
Um código único é gerado e armazenado no bucket AWS S3, junto com os metadados.

3. Redirecionamento
Outra API valida o código da URL curta.
Verifica se o prazo de validade expirou.
Redireciona o usuário para a URL original.
