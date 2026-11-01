# LeadFup — CRM de Gestão Comercial

![Status](https://img.shields.io/badge/status-em%20desenvolvimento-orange) ![PHP](https://img.shields.io/badge/PHP-8.2%2B-777BB4?logo=php&logoColor=white) ![Laravel](https://img.shields.io/badge/Laravel-12-FF2D20?logo=laravel&logoColor=white)

O **LeadFup** é um projeto de CRM (Customer Relationship Management) desenvolvido para organizar a rotina comercial em um único ambiente: cadastro de clientes e contatos, acompanhamento de oportunidades em um funil de vendas e gerenciamento de atividades relacionadas aos negócios.

Este repositório é uma **apresentação pública do projeto**. O código-fonte da aplicação permanece em um repositório privado e não é distribuído aqui.

## Visão geral

O objetivo do LeadFup é oferecer uma estrutura simples para acompanhar o relacionamento com clientes e a evolução das oportunidades comerciais, desde a prospecção até o fechamento.

### Funcionalidades documentadas

- **Autenticação:** acesso de usuários por sessão, com fluxo de ativação/criação de senha por link enviado por e-mail.
- **Clientes e contatos:** cadastro e edição de informações de clientes e seus contatos.
- **Negócios:** organização das oportunidades comerciais e associação com leads.
- **Funil de vendas:** acompanhamento das oportunidades por etapas, com movimentação entre etapas.
- **Atividades:** registro de e-mails, ligações e reuniões, com prazos, status e histórico de eventos.


## Tecnologias

| Área | Tecnologias |
| --- | --- |
| Backend | PHP 8.2+, Laravel 12 |
| Persistência | MySQL, Eloquent ORM |
| Interface | Blade, JavaScript, jQuery, Bootstrap 5, Sass |
| Build de assets | Vite |
| Dependências | Composer, npm |

## Organização técnica

A aplicação adota uma separação de responsabilidades em camadas, com componentes de Controllers, Services, Repositories e Models. Também possui componentes dedicados a middleware, regras de validação, segurança e utilitários.

```text
app/
├── Controllers/
├── Services/
├── Repositories/
├── Models/
├── Middleware/
├── Rules/
├── Security/
└── Support/

resources/
├── views/
└── assets/

routes/
database/
tests/
```

A estrutura acima é ilustrativa e omite arquivos internos e detalhes de implementação.

Consulte:
- [Visão da arquitetura](docs/architecture.md)
- [Funcionalidades](docs/features.md)
- [Decisões técnicas](docs/technical-decisions.md)
- [Diagrama de arquitetura](diagrams/architecture.mmd)

## Segurança e privacidade

Este repositório público foi separado intencionalmente do código-fonte privado. Ele contém apenas documentação de alto nível para apresentação profissional.

- Não contém código-fonte da aplicação.
- Não contém arquivos .env, tokens, senhas ou credenciais.
- Não contém dumps de banco de dados ou dados reais de usuários/clientes.
- Não contém configurações operacionais ou detalhes sensíveis de infraestrutura.


## Estado do projeto

O LeadFup está em desenvolvimento. Este repositório funciona como material de portfólio e documentação pública; não é uma distribuição instalável da aplicação.

## Sobre o código-fonte

Por se tratar de um projeto mantido em repositório privado, o código-fonte não está disponível publicamente. A documentação foi preparada para demonstrar objetivos, funcionalidades e decisões de organização técnica sem expor a implementação proprietária.

---

**LeadFup — CRM de Gestão Comercial**  
Projeto independente de desenvolvimento de software.
