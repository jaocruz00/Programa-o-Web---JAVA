# Programação WEB em linguagem Java

Este projeto foi desenvolvido para a disciplina de Programação Web em Java, do curso de A.D.S da FATEC, e tem como objetivo demonstrar, de forma simples e prática, o funcionamento de operações CRUD em uma aplicação web. A proposta do sistema é utilizar páginas `.jsp`, HTML, Servlets, JDBC e MySQL para implementar o fluxo básico de cadastro, leitura, edição e exclusão de dados em um sistema acadêmico voltado ao gerenciamento de clientes de advocacia. 

O sistema possui dois módulos principais integrados. O primeiro módulo é responsável pelo cadastro e gerenciamento de clientes. O segundo módulo permite registrar agendamentos vinculados aos clientes previamente cadastrados, conectando assim duas funcionalidades dentro do mesmo projeto. Esse tipo de organização é comum em aplicações Java Web simples que usam JSP, Servlet e JDBC como base didática. 

## Funcionalidades

- Cadastro de clientes.
- Listagem de clientes cadastrados.
- Edição de dados do cliente.
- Exclusão de clientes.
- Geração de relatório `.txt` de cliente.
- Cadastro de agendamentos.
- Vinculação de agendamentos a clientes já cadastrados.
- Visualização dos agendamentos registrados.

## Tecnologias utilizadas

- Java
- JSP
- HTML
- Servlets
- JDBC
- MySQL
- Apache Tomcat
- NetBeans

## Fluxo simples do sistema

```text
[Início]
   |
   v
[Página inicial]
   |
   +--> [Cadastrar cliente]
   |         |
   |         v
   |   [Preenche formulário]
   |         |
   |         v
   |   [Servlet recebe os dados]
   |         |
   |         v
   |   [DAO grava no banco]
   |         |
   |         v
   |   [Cliente cadastrado]
   |
   +--> [Listar clientes]
   |         |
   |         v
   |   [Servlet busca clientes]
   |         |
   |         v
   |   [JSP exibe tabela]
   |         |
   |         +--> [Editar cliente]
   |         |
   |         +--> [Excluir cliente]
   |         |
   |         +--> [Gerar TXT]
   |
   +--> [Abrir agenda]
             |
             v
      [Selecionar cliente cadastrado]
             |
             v
      [Preencher data, horário e descrição]
             |
             v
      [Servlet recebe os dados]
             |
             v
      [DAO grava agendamento no banco]
             |
             v
      [Agendamento vinculado ao cliente]
             |
             v
      [Listagem dos agendamentos]
```

## Objetivo acadêmico

O principal objetivo deste projeto é demonstrar, de maneira simples e funcional, a implementação de um sistema web em Java com operações CRUD, conforme solicitado na disciplina. O foco está na compreensão da lógica da aplicação, na comunicação entre páginas JSP e Servlets e na integração com banco de dados relacional por meio de JDBC.
