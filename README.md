# 🧼 APICleanCodeConsorcio

Este repositório apresenta uma solução desenvolvida em **.NET 7** para uma API de gerenciamento de clientes, estruturada com base nos princípios da **Clean Architecture**. O objetivo é fornecer uma base limpa, modular e escalável para o desenvolvimento de APIs RESTful.

> ⚠️ **Aviso:** Este projeto é de caráter acadêmico e não deve ser utilizado em produção sem adaptações.

---

## 🧱 Estrutura do Projeto

```
WebApiClientes.sln
├── ApiWEB/             # Projeto principal ASP.NET Core Web API
├── Application/        # Camada de aplicação (casos de uso, serviços)
├── Domain/             # Camada de domínio (entidades e regras de negócio)
└── Infraestrutura/     # Camada de infraestrutura (repositórios, acesso a dados)
```

### 📁 Descrição dos Projetos

- **ApiWEB**: Ponto de entrada da aplicação. Contém os controladores, configuração de middlewares e documentação Swagger.
- **Application**: Lógica de negócio da aplicação (casos de uso, DTOs, serviços de aplicação).
- **Domain**: Núcleo da aplicação com entidades, interfaces e regras de negócio puras.
- **Infraestrutura**: Implementações concretas de repositórios, acesso a banco de dados e integrações externas.

---

## ▶️ Como Executar

### ✅ Pré-requisitos

- [.NET 7 SDK](https://dotnet.microsoft.com/download/dotnet/7.0)
- Visual Studio 2022 (ou superior) ou Visual Studio Code

### 🧪 Passos

1. **Clonar o repositório**:
   ```bash
   git clone https://github.com/seu-usuario/APICleanCodeConsorcio.git
   ```

2. **Restaurar as dependências**:
   ```bash
   dotnet restore
   ```

3. **Compilar a solução**:
   ```bash
   dotnet build
   ```

4. **Executar a API**:
   ```bash
   cd ApiWEB
   dotnet run
   ```

5. Acesse a documentação Swagger:
   [http://localhost:5188/swagger](http://localhost:5188/swagger)

---

## ⚙️ Configurações

As configurações de ambiente e conexões estão nos arquivos:

- `ApiWEB/appsettings.json`
- `ApiWEB/appsettings.Development.json`

---

## 🔍 Observações

- O projeto já vem configurado com suporte a **Swagger/OpenAPI** para facilitar testes e documentação.
- A arquitetura segue uma separação clara de responsabilidades, permitindo testes isolados e fácil manutenção.
- Você pode adaptar esta base para contextos reais adicionando autenticação, banco de dados, testes automatizados, entre outros.

---

## 👨‍💻 Autor

**Abel Fonseca**  
Projeto criado para fins de aprendizado, estudo de arquitetura limpa e boas práticas com .NET.