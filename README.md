# 🚑 HelpApp - Avaliação TP2

### 🔥 Sistema de Gerenciamento de Atendimento | Clean Architecture | .NET 8 | Azure SQL

---

## 📜 Descrição

O **HelpApp** é uma aplicação desenvolvida como parte da Avaliação TP2, utilizando os princípios de **Clean Architecture**, implementado em **.NET Core 8**, com banco de dados em **Azure SQL Server**.

O projeto é focado em fornecer um sistema escalável, seguro e de fácil manutenção, utilizando as melhores práticas de desenvolvimento backend, organização de código, versionamento e testes.

---

## 🚀 Tecnologias e Ferramentas

- ✅ .NET 8
- ✅ ASP.NET Core Web API
- ✅ Clean Architecture
- ✅ Entity Framework Core
- ✅ Azure SQL Server
- ✅ Docker (opcional)
- ✅ GitHub Actions (CI/CD opcional)
- ✅ xUnit e Moq (para testes)
- ✅ GitHub Projects ou Trello (Kanban)

---

## 🏗️ Arquitetura do Projeto

HelpApp
│
├── src
│ ├── HelpApp.API --> Camada de apresentação (Controllers, Program.cs)
│ ├── HelpApp.Application --> Casos de uso, serviços de aplicação, DTOs
│ ├── HelpApp.Domain --> Entidades, interfaces, regras de negócio puras
│ └── HelpApp.Infrastructure --> Acesso a dados, serviços externos, configurações
│
├── tests
│ ├── HelpApp.Application.Tests --> Testes unitários
│ └── HelpApp.API.Tests --> Testes de integração
│
└── README.md


---

## 🗺️ Diagrama da Arquitetura


- 🔸 **API:** Responsável por expor os endpoints da aplicação.
- 🔸 **Application:** Onde ficam as regras de aplicação, orquestração dos serviços e casos de uso.
- 🔸 **Domain:** Contém as entidades, interfaces e regras de negócio puras, sem dependências.
- 🔸 **Infrastructure:** Implementação concreta das interfaces (banco de dados, serviços externos, etc).

---

## 🔧 Configuração e Execução

### ✅ Pré-requisitos
- .NET SDK 8 ou superior instalado
- SQL Server (Local, Docker ou Azure)
- Visual Studio / VS Code / Rider
- Git

### 🚀 Executando a aplicação localmente

1. Clone o repositório
```bash
git clone https://github.com/seu-usuario/helpapp.git
cd helpapp
 🔸 **API:** Responsável por expor os endpoints da aplicação.
- 🔸 **Application:** Onde ficam as regras de aplicação, orquestração dos serviços e casos de uso.
- 🔸 **Domain:** Contém as entidades, interfaces e regras de negócio puras, sem dependências.
- 🔸 **Infrastructure:** Implementação concreta das interfaces (banco de dados, serviços externos, etc).

---

## 🔧 Configuração e Execução

### ✅ Pré-requisitos
- .NET SDK 8 ou superior instalado
- SQL Server (Local, Docker ou Azure)
- Visual Studio / VS Code / Rider
- Git

### 🚀 Executando a aplicação localmente

1. Clone o repositório
```bash
git clone https://github.com/seu-usuario/helpapp.git
cd helpapp
Configure o banco no appsettings.json da API

json
Copiar
Editar
\"ConnectionStrings\": {
  \"DefaultConnection\": \"Server=localhost;Database=HelpAppDb;User Id=sa;Password=SuaSenha123;\"
}
Rode as migrations para criar o banco

bash
Copiar
Editar
dotnet ef database update --project src/HelpApp.Infrastructure
Execute o projeto

bash
Copiar
Editar
dotnet run --project src/HelpApp.API
A API estará disponível em:

arduino
Copiar
Editar
https://localhost:5001
http://localhost:5000
📑 Endpoints Disponíveis
Método	Rota	Descrição
GET	/api/user	Lista todos os usuários
GET	/api/user/{id}	Retorna usuário por ID
POST	/api/user	Cria um novo usuário
PUT	/api/user/{id}	Atualiza um usuário
DELETE	/api/user/{id}	Remove um usuário

🧪 Executando os Testes
bash
Copiar
Editar
dotnet test
✔️ Testes Unitários (Application.Tests)

✔️ Testes de Integração (se implementados)

🏗️ Banco de Dados
SQL Server (Azure ou Local)

Gerenciamento via Entity Framework Core



Editar
dotnet ef migrations add InitialCreate --project src/HelpApp.Infrastructure
dotnet ef database update --project src/HelpApp.Infrastructure
🛠️ Padrões de Git e Branches
🔥 main → Branch principal (produção)

🚧 develop → Branch de desenvolvimento

🔧 feature/ → Branch para novas funcionalidades

🐛 bugfix/ → Correção de bugs

🔥 hotfix/ → Correções emergenciais

🏷️ Commit Semântico
Prefixo	Descrição
feat:	Nova funcionalidade
fix:	Correção de bug
docs:	Alterações na documentação
style:	Formatação, identação, espaço
refactor:	Refatoração de código
test:	Adição ou ajuste de testes
chore:	Atualização de tarefas auxiliares

Exemplos:


Editar
feat: implementa endpoint de cadastro de usuário
fix: corrige bug na busca de usuários por ID
🗂️ Organização no Kanban
A Fazer	Em Progresso	Concluído
Modelagem de Entidade User	CRUD Usuário - API	CRUD Usuário Finalizado
Implementar Testes Unitários		
CRUD Produto		
Integração com API externa		

🔗 Link do Kanban: [Coloque o link aqui]

🏆 Contribuidores
Nome	Função
Daniele Veronesi	🏆 Gestora do Repositório
	Desenvolvedor(a)
	Desenvolvedor(a)

📚 Licença
Projeto desenvolvido para fins acadêmicos na disciplina de Desenvolvimento Backend com .NET e Azure, conforme avaliação TP2.

💙 Feito com dedicação, código limpo e arquitetura bem feita.

Copiar
Editar

---







