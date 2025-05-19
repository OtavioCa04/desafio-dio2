Configuração de Instância de Banco de Dados SQL no Azure
Este repositório documenta todas as etapas seguidas para realizar a configuração de uma instância gerenciada de banco de dados SQL na plataforma Microsoft Azure, como parte do desafio prático da DIO.

Objetivo
Colocar em prática os conhecimentos adquiridos sobre serviços de banco de dados em nuvem.

Demonstrar a criação e configuração de um banco de dados SQL no Azure.

Criar um material de apoio com anotações, dicas e boas práticas para futuras implementações.

Etapas Realizadas
1. Acesso ao Portal do Azure
Acesse o site: https://portal.azure.com

Faça login com sua conta Microsoft.

2. Criação da Instância de Banco de Dados
No menu lateral esquerdo, clique em "Criar um recurso".

Selecione a opção "Banco de dados" > "Banco de Dados SQL".

Clique em "Criar".

3. Configuração da Instância
Assinatura: selecione a assinatura disponível.

Grupo de Recursos: escolha um existente ou crie um novo.

Nome do banco de dados: ex. desafio-sql-dio.

Servidor:

Clique em "Criar novo".

Informe um nome único, usuário administrador, senha e localização.

Clique em "Avançar" para continuar as configurações.

4. Configurações de Rede
Mantenha a conectividade pública habilitada.

Autorize o acesso a partir do seu IP atual (opção recomendada).

Configure as regras de firewall conforme necessário.

5. Configurações Adicionais
Mantenha os valores padrão para backup e escalabilidade, se preferir um ambiente de testes.

Revise os detalhes finais e clique em "Criar".

Testando a Conexão
Utilize um cliente SQL, como SQL Server Management Studio (SSMS), Azure Data Studio ou outro.

Dados para conexão:

Servidor: nomedoservidor.database.windows.net

Usuário/Senha: definidos no momento da criação

Execute comandos básicos de teste, como:

CREATE TABLE Teste (
    ID INT PRIMARY KEY,
    Nome NVARCHAR(100)
);

INSERT INTO Teste VALUES (1, 'DIO');

SELECT * FROM Teste;
Dicas e Boas Práticas
Nunca compartilhe publicamente suas credenciais.

Monitore os custos dos recursos criados, mesmo em contas gratuitas.

Utilize grupos de recursos para manter seus serviços organizados.

Exclua os recursos após o uso para evitar cobranças.

Referências
Criar Banco SQL no Azure - Documentação Microsoft

Documentação GitHub

Conclusão
Este desafio me permitiu aplicar, na prática, os conhecimentos adquiridos sobre banco de dados em nuvem, além de consolidar a habilidade de documentar tecnicamente um processo. A configuração da instância de banco de dados no Azure é direta e intuitiva, sendo uma excelente opção para testes e protótipos.
