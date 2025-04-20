# Projeto: Instância de Banco de Dados SQL no Azure

Este repositório documenta o processo de configuração e gestão de uma instância de Banco de Dados SQL no Microsoft Azure, com foco em aplicar conceitos aprendidos ao longo dos desafios de modelagem de banco de dados e operações em nuvem. O projeto é uma prática da criação de uma instância gerenciada de banco de dados no Azure e está vinculado ao Bootcamp **IA Aplicada a Dados com Copilot** da DIO.

## Objetivos do Projeto

O projeto visa a configuração e o gerenciamento de uma instância de banco de dados SQL no Azure, documentando o processo de:

- Criação de uma instância de banco de dados no Azure;
- Conexão ao banco de dados utilizando ferramentas como **SQL Server Management Studio (SSMS)** ou **Azure Data Studio**;
- Configuração de segurança e otimização de recursos;
- Compartilhamento de experiência e melhores práticas por meio de documentação técnica.

## Ferramentas e Tecnologias Utilizadas

- **Microsoft Azure**: Plataforma de nuvem usada para criar e gerenciar a instância de banco de dados SQL.
- **SQL Server Management Studio (SSMS)** / **Azure Data Studio**: Ferramentas para conexão e gestão do banco de dados SQL.
- **GitHub**: Repositório para documentação do processo e compartilhamento do projeto.

## Passos de Implementação

### 1. **Criação da Instância de Banco de Dados no Azure**

- Acesse o [Azure Portal](https://portal.azure.com/).

- Crie uma nova instância de banco de dados SQL, configurando o nome do servidor, a camada de preços e as credenciais de acesso.

  **Detalhes da instância**:

  - Nome do servidor: `srv-sql-dio.database.windows.net`
  - Camada de Preço: `Uso Geral - Sem servidor: Gen5, 2 vCores`
  - Região: `West US 2`
  - Atraso da pausa automática: `1 hora`

### 2. **Configuração de Segurança e Firewall**

- Configure o firewall para permitir conexões de seu IP local.
- No portal Azure, acesse a opção de **Firewall** e adicione o IP da sua máquina à lista de IPs permitidos.

### 3. **Conectar ao Banco de Dados**

- Utilize **SQL Server Management Studio (SSMS)** ou **Azure Data Studio** para conectar ao servidor criado (`srv-sql-dio.database.windows.net`) utilizando suas credenciais de administrador.

  Exemplo de consulta para testar a conexão:

  ```sql
  SELECT GETDATE();
  ```

4. Gerenciamento e Backups
   Não há pontos de restauração configurados inicialmente.

A instância de banco de dados está configurada para pausas automáticas após 1 hora de inatividade, conforme configurado na camada sem servidor.

Detalhes Técnicos
Assinatura Azure: Azure subscription 1

Grupo de Recursos: rg-vm-dio

Nome do Servidor: srv-sql-dio.database.windows.net

Método de Autenticação: Microsoft Entra

Camada de Preço: Uso Geral - Sem servidor: Gen5, 2 vCores

Região: West US 2

Conclusão
Com a configuração da instância de banco de dados SQL no Azure, completamos mais um passo no aprendizado de gestão de bancos de dados na nuvem, aplicado em um contexto de alta disponibilidade e escalabilidade. Este repositório serve como material de apoio, documentando o processo e compartilhando as melhores práticas para futuras implementações.


Nota: O repositório está em constante atualização com novos aprendizados e ajustes. Sinta-se à vontade para contribuir com sugestões ou melhorias no processo.

