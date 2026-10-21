# 🚗 Sistema de Registro de Veículos com Minimal APIs & Testes em .NET

Este projeto consiste em uma **Web API de Gerenciamento e Registro de Veículos**, desenvolvida utilizando o conceito moderno de **Minimal APIs** no ASP.NET Core. O projeto faz parte da trilha de **Backend com .NET** proposta pela **Randstad** em parceria com a **Digital Innovation One (DIO)**.

A aplicação simula um sistema seguro onde administradores autenticados podem gerenciar uma frota de veículos, aplicando boas práticas de arquitetura, segurança com tokens e testes automatizados para garantir a confiabilidade do sistema.

---

## 🚀 Funcionalidades Principais

* **Gerenciamento de Veículos**: Cadastro, listagem, atualização e exclusão de automóveis (CRUD).
* **Autenticação e Autorização**: Sistema de login para administradores utilizando autenticação baseada em regras com **JWT (JSON Web Token)**.
* **Documentação Interativa**: Interface visual criada com **Swagger** para testar os endpoints da API de forma simples.
* **Testes Automatizados**: Suíte de testes para validar o comportamento dos controladores, regras de negócio e garantir que a aplicação funcione corretamente.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

* **C# / .NET Core**: Linguagem e ecossistema principal.
* **Minimal APIs (ASP.NET Core)**: Abordagem simplificada e de alta performance para a criação de endpoints HTTP com menos linhas de código.
* **JWT Bearer Authentication**: Para proteção das rotas e controle de acesso baseado em perfis/regras.
* **Entity Framework Core**: ORM para comunicação e persistência de dados.
* **Ferramentas de Teste (xUnit / Moq / Bogus)**: Frameworks e bibliotecas utilizadas no projeto de teste para simular cenários e validar a API.
* **Swagger (OpenAPI)**: Para documentação e testes rápidos da API.

---

## 📁 Estrutura da Solução

A solução (`minimal-api.sln`) está dividida de forma limpa em dois grandes blocos:
* **`Api/`**: Contém o código-fonte principal da aplicação, incluindo as rotas da Minimal API, mapeamento de banco de dados, DTOs, entidades de Administradores/Veículos e configurações de segurança.
* **`Test/`**: Projeto dedicado exclusivamente aos testes automatizados (testes unitários e/ou de integração) para validar a robustez e segurança das regras de negócio aplicadas.

---

## ⚙️ Como Executar o Projeto Localmente

### Pré-requisitos
* [.NET SDK](https://microsoft.com) instalado.
* IDE de sua preferência (VS Code, Visual Studio ou Rider).

### Passo a Passo

1. **Clonar o repositório:**
   ```bash
   git clone https://github.com
   ```

2. **Navegar até a pasta da API:**
   ```bash
   cd ASP.NET_Minimals_API/Api
   ```

3. **Restaurar as dependências e rodar a API:**
   ```bash
   dotnet restore
   dotnet run
   ```
   Abra o link gerado no terminal (geralmente acompanhado de `/swagger`) no seu navegador para visualizar a interface interativa e testar o fluxo de autenticação e os endpoints de veículos.

### 🧪 Executando os Testes

Para garantir que tudo está funcionando perfeitamente e rodar a suíte de testes automatizados:
1. Volte para a raiz do projeto ou entre na pasta de testes:
   ```bash
   cd ../Test
   ```
2. Execute o comando de testes do .NET:
   ```bash
   dotnet test
   ```
   O terminal exibirá o relatório com o sucesso de todos os cenários testados.

---

## 👨‍💻 Autor

Desenvolvido por **Marcelo** (marceloxm).
Projeto educacional voltado para o aprendizado de arquiteturas modernas, APIs enxutas de alta performance e testes de software no ecossistema .NET.

