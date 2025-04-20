# banco-azure-dio
Projeto desenvolvido como parte do bootcamp "XP Inc. - Cloud com Inteligência Artificial", proposto pela DIO.

# Projeto de Instância de Banco de Dados SQL no Azure

Este repositório contém a documentação e os passos para a criação de uma instância gerenciada de SQL no Microsoft Azure. O objetivo é demonstrar o processo de configuração de um banco de dados SQL na nuvem, documentando o aprendizado de como configurar e gerenciar instâncias de banco de dados no Azure.

## Objetivos

- **Configuração do Banco de Dados**: Criar uma instância de banco de dados SQL no Azure utilizando as ferramentas fornecidas pela plataforma.
- **Documentação**: Registrar o processo de criação da instância e quaisquer observações importantes para facilitar futuras implementações.
- **Uso do GitHub**: Criar um repositório público para compartilhar a documentação técnica e o processo de configuração.

## Passos para Configuração

1. **Criar uma Instância de Banco de Dados no Azure**:
   - Acesse o [Azure Portal](https://portal.azure.com/).
   - Crie uma nova instância de banco de dados SQL, configurando o nome do servidor, camadas de preço, e credenciais de acesso.
   - Nome do servidor: `srv-sql-dio.database.windows.net`
   - Camada de preço: `Uso Geral - Sem servidor: Gen5, 2 vCores`
   - Região: `West US 2`
   - Atraso da pausa automática: `1 hora`

2. **Conectar ao Banco de Dados**:
   - Utilize o **SQL Server Management Studio (SSMS)** ou **Azure Data Studio** para conectar ao servidor utilizando o nome do servidor `srv-sql-dio.database.windows.net`.
   - Teste a conexão executando uma consulta simples como:
     ```sql
     SELECT GETDATE();
     ```

3. **Configurações de Segurança e Backup**:
   - Configuração de **Firewall**: Assegure que o IP da sua máquina esteja permitido no firewall do Azure.
   - **Pontos de Restauração**: No momento, não há pontos de restauração configurados.

## Detalhes da Instância

- **Assinatura**: Azure subscription 1
- **Grupo de Recursos**: rg-vm-dio
- **Localização**: West US 2
- **Nome do Servidor**: srv-sql-dio.database.windows.net
- **Autenticação**: Microsoft Entra ou SQL Server Authentication
- **Camada de Preço**: Gratuito - Uso Geral - Sem servidor: Gen5, 2 vCores

## Recursos

- **Documentação Oficial do Azure**: [Documentação sobre Banco de Dados SQL no Azure](https://learn.microsoft.com/azure/azure-sql/)
- **Documentação do GitHub**: [GitHub Docs](https://docs.github.com/)

## Capturas de Tela

As capturas de tela abaixo demonstram os passos de configuração no portal do Azure:

- **Tela de Criação do Banco de Dados**:
  ![Tela de Criação do Banco de Dados](images/screenshot-1.png)

- **Configuração de Firewall no Azure**:
  ![Configuração de Firewall](images/screenshot-2.png)

## Conclusão

Neste projeto, configuramos uma instância de banco de dados SQL no Azure, testamos a conexão e documentamos o processo para referência futura. O repositório foi criado para servir como material de apoio para implementações semelhantes.

---

**Nota**: A documentação está em constante atualização. Sinta-se à vontade para contribuir com melhorias ou atualizações.


