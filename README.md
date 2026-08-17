# Voluntiva

**Voluntiva** é um sistema de gestão de voluntários voltado a organizações não governamentais (ONGs), desenvolvido como projeto acadêmico integrando as disciplinas de **Laboratório de Projeto de Software**, **Projeto de Protocolo de Redes** e **Laboratório de Banco de Dados**.

## Objetivo

O projeto tem como objetivo centralizar e facilitar a gestão de voluntários, ações sociais e inscrições em eventos promovidos por ONGs. A plataforma deverá permitir que organizações cadastrem oportunidades de voluntariado e que voluntários encontrem ações compatíveis com seu perfil, habilidades e disponibilidade.

## Funcionalidades previstas

- Cadastro e autenticação de voluntários e ONGs;
- Cadastro de unidades e ações sociais;
- Consulta de oportunidades de voluntariado;
- Inscrição e cancelamento de participação em ações;
- Registro de habilidades e disponibilidade dos voluntários;
- Controle de presença e histórico de participação;
- Notificações sobre criação, atualização ou cancelamento de ações;
- Gestão das informações por meio de um banco de dados relacional.

## Relação com as disciplinas

### Laboratório de Projeto de Software

Responsável pela definição de requisitos, casos de uso, arquitetura da aplicação, regras de negócio, interface e organização dos módulos do sistema.

### Projeto de Protocolo de Redes

A aplicação utilizará uma arquitetura cliente-servidor. A comunicação entre clientes e servidor será feita por meio de um protocolo de aplicação próprio sobre TCP, com mensagens para operações como autenticação, consulta de eventos, inscrições, atualizações e notificações.

Exemplos de comandos previstos:

```text
LOGIN
LIST_EVENTS
JOIN_EVENT
LEAVE_EVENT
CREATE_EVENT
UPDATE_EVENT
CHECK_IN
CHECK_OUT
PING
PONG
```

### Laboratório de Banco de Dados

O banco de dados armazenará informações relacionadas a voluntários, ONGs, unidades, ações sociais, habilidades, inscrições, presença e histórico de participação.

Entidades iniciais previstas:

- Voluntário;
- ONG;
- Unidade;
- Evento/Ação Social;
- Habilidade;
- Inscrição;
- Presença;
- Usuário.

## Arquitetura inicial

```text
Cliente Voluntário ─┐
                    │
Cliente ONG ─────────┼── TCP / Protocolo Voluntiva ── Servidor ── Banco de Dados
                    │
Cliente Unidade ─────┘
```

## Equipe

- Carlos Gabriel Gouveia
- João Gabriel Guedes Vianna
- João Guilherme Costa Couto
- João Victor Pereira Bicalho
- Mateus Munhoz Guimarães

## Status

🚧 Projeto em fase inicial de planejamento e definição da arquitetura.

## Próximos passos

1. Levantamento e documentação dos requisitos;
2. Definição dos casos de uso;
3. Modelagem do banco de dados;
4. Especificação do protocolo de comunicação;
5. Definição da stack de desenvolvimento;
6. Implementação do servidor e dos clientes;
7. Integração e testes.
