# Desafio de Backend e Full Stack para Engenheiro de Software - Nasten

## Descrição Geral

Este desafio tem como objetivo testar e aprimorar seu conhecimento em desenvolvimento backend, utilizando o framework **NestJS** e o **TypeORM** para gerenciar relacionamentos complexos entre entidades. O objetivo é que você demonstre familiaridade com arquiteturas baseadas em módulos, relacionamentos muitos-para-muitos com propriedades customizadas, e o uso de CRUD Controllers para operações eficientes.

## Objetivos do Desafio

Você deverá implementar uma API com **NestJS** e **TypeORM** para gerenciar entidades com um relacionamento muitos-para-muitos. Além disso, você precisará desenvolver operações CRUD para essas entidades, configurando as rotas para inclusão de múltiplos registros e filtros via query params.

## Tarefas

1. **Configuração do Ambiente**
   - Crie uma aplicação NestJS com módulos bem estruturados.
   - Configure o TypeORM para conectar-se a um banco de dados PostgreSQL ou outro banco relacional de sua preferência.
   - Garanta que todas as dependências necessárias para o projeto estão corretamente configuradas.

2. **Modelagem das Entidades**
   - Crie duas entidades com um relacionamento [muitos-para-muitos](https://orkhan.gitbook.io/typeorm/docs/many-to-many-relations) e inclua propriedades personalizadas neste relacionamento.
   - Exemplo de entidades: `Aluno` e `Curso`, onde:
     - Um aluno pode estar matriculado em múltiplos cursos, e um curso pode ter múltiplos alunos.
     - Adicione uma tabela intermediária para armazenar informações adicionais, como `dataDeMatricula`.

3. **Implementação do CRUD**
   - Implemente operações CRUD (Create, Read, Update, Delete) para as entidades, utilizando o **CRUDController** do NestJS.
   - Configure rotas para manipulação de múltiplos registros e busque as entidades utilizando query params para filtrar resultados.
   - Exemplo: `GET /alunos?curso=typescript` para buscar todos os alunos que estão no curso de TypeScript.

4. **Query Params**
   - Garanta que as rotas de busca permitam a utilização de **query params** para filtrar os registros de forma dinâmica, permitindo consultas mais flexíveis.

5. **Validação e Tratamento de Erros**
   - Adicione validações nas rotas de criação e atualização de registros.
   - Implemente tratamento de erros apropriado e retorne mensagens claras em caso de falhas.

## Tarefa Bônus

Conecte o backend a um frontend em **Next.js**:
   - Crie uma interface simples em Next.js que consuma a API desenvolvida.
   - Permita que o usuário visualize e cadastre novos registros, exibindo dados das entidades e do relacionamento.
   - Utilize hooks de estado do React para interagir com as rotas CRUD.

## Tecnologias Requeridas

- [**NestJS**](https://docs.nestjs.com/)
- [**TypeORM**](https://orkhan.gitbook.io/typeorm/docs)
- **PostgreSQL** ou banco relacional similar
- [**CRUD Controller - Data UI** ](https://gid-oss.github.io/dataui-nestjs-crud/controllers/#description)
- **Next.js** (para a tarefa bônus)

## Critérios de Avaliação

Serão avaliados os seguintes aspectos da sua implementação:

- Organização e modularidade do código.
- Configuração adequada do TypeORM e implementação dos relacionamentos.
- Uso correto do CRUDController para operações de CRUD.
- Implementação de query params para buscas.
- Validações e tratamento de erros.
- Integração frontend-backend (na tarefa bônus).
  
## Observações Finais

Este desafio é uma oportunidade para demonstrar sua habilidade em desenvolver APIs robustas e escaláveis, com especial atenção ao uso de relacionamentos e TypeORM. Dê o seu melhor e aproveite a chance para mostrar suas habilidades para a vaga!

Boa sorte e mãos à obra!
