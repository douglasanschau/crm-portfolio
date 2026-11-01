# Visão da arquitetura

O LeadFup foi organizado para separar responsabilidades entre a camada HTTP, regras de negócio, acesso a dados e persistência. Esta documentação apresenta somente a visão conceitual; nomes e detalhes internos foram reduzidos para não expor a implementação privada.

## Camadas e responsabilidades

| Camada | Responsabilidade |
| --- | --- |
| Controllers | Receber requisições, coordenar a entrada e devolver respostas. |
| Services | Concentrar operações e regras de negócio. |
| Repositories | Isolar consultas e operações de persistência. |
| Models | Representar as entidades e seus relacionamentos. |
| Middleware e segurança | Aplicar verificações transversais e controles de acesso. |
| Regras e suporte | Reunir validações e componentes auxiliares. |

## Fluxo conceitual de uma requisição

1. O usuário autenticado realiza uma ação pela interface.
2. A rota direciona a requisição para o controller responsável.
3. O controller aciona o serviço de domínio apropriado.
4. Quando necessário, o serviço utiliza a camada de repositório para consultar ou persistir informações.
5. A resposta retorna à interface para atualização da experiência.

## Isolamento por empresa

A aplicação considera a empresa associada ao usuário autenticado nas operações de negócio. As verificações de acesso são aplicadas para evitar que um usuário opere sobre registros de outra empresa.

## Observação

O diagrama em [architecture.mmd](../diagrams/architecture.mmd) representa o desenho em alto nível. Ele não descreve endpoints, nomes de classes, estrutura física do banco, regras internas detalhadas ou configurações de infraestrutura.