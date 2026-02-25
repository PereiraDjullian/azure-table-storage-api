# 📊 Azure Table Storage API (.NET 10)

Esta API foi desenvolvida para demonstrar a integração de aplicações .NET com o **Azure Table Storage**, um serviço de banco de dados NoSQL (Key-Value) altamente escalável. O projeto foca em operações CRUD de alta performance para gerenciamento de contatos.



## 🛠️ Tecnologias e SDKs
* **C# / .NET 10**: Utilizando as versões mais recentes do framework.
* **Azure.Data.Tables**: SDK oficial da Microsoft para manipulação de tabelas.
* **ASP.NET Core Web API**: Estrutura robusta para os endpoints.
* **Swagger/OpenAPI**: Interface interativa para testes e documentação.

## 📋 Funcionalidades do CRUD
- [x] **Criar Contato**: Gera automaticamente `RowKey` (ID único) e `PartitionKey`.
- [x] **Listagem Completa**: Recuperação eficiente de todas as entidades da tabela.
- [x] **Busca por Nome**: Utiliza filtros OData/LINQ otimizados para o Azure.
- [x] **Atualização (Upsert)**: Atualiza dados existentes de forma atômica.
- [x] **Remoção**: Deleção por chaves de acesso.

## ⚙️ Configuração Local

1. **Requisitos**: Ter uma Connection String de uma *Storage Account* na Azure ou usar o emulador Azurite.
2. **Configuração**: Adicione suas credenciais no `appsettings.json`:
   ```json
   {
     "SaConnectionString": "SUA_CHAVE_AQUI",
     "azureTableNames": "ex:Contatos"
   }
Execução:

Bash
dotnet run
🚀 Como Testar
Com a aplicação rodando, acesse a interface do Swagger em:
http://localhost:PORTA/swagger

<img width="1312" height="647" alt="image" src="https://github.com/user-attachments/assets/2a81e125-ed77-4ec7-954b-fee77d3f109f" />


✨ Projeto desenvolvido Cloud e .NET.
