# Automa-o---MailBot
Projeto de RPA que consiste em detectar um gatilho e realizar uma ação a partir disso. Neste caso o robô detecta que um certificado digital está perto do vencimento
e envia um email automaticamente e em segundo plano para o dono do certificado em questão.
Um código simples onde o robô compara a data atual com uma base de dados que informa o vencimento de cada certificado, 
caso ele verifique que a data de vencimento é igual a data atual, ele envia para o cliente um email, informando que o certificado digital venceu e pedindo
para o cliente entrar em contato com a empresa. No caso a base de dados é basiocamente composta pelas seguintes colunas:
Nome da empresa|Email do cliente ou da empresa|Data de vencimento do crtificado
A base de dados na verdade não é alçimentada com a data de vencimento, mas com um periodo próximo, por exemplo 30 dias antes do vencimento do certificado,
para que o cliente seja avisado com antecedência. Esse código fica executando sempre, pode ser colocado em um seridor ou máquina virtual
para que assim que detectar a data possa fazer a execução das ações
Vale frisar que nesse código nenhuma janela é aberta o robô faz tudo em segundo plano, evitando assim erros de automação de mouse e teclado.
