## Projeto - Banco de Dados: Academia

Este projeto representa a modelagem lógica e física de um sistema de banco de dados para uma academia, com foco em organização e normalização. Material feito apenas para estudos, demonstrações e portfólio.

# Estrutura do Projeto

- `ddl/`  
  Scripts SQL de criação das tabelas e constraints (`CREATE_TABLE.psql`, `CONSTRAINTS.psql`)

- `doc/`  
  Documentação textual explicando a estrutura do banco.

- `diagramas/`  
  Diagramas ER gerados no BRModelo e DBDiagram para facilitar visualização do modelo.

- `INSERTS_EXEMPLO.sql`  
  Inserções para simular um cenário completo com clientes, planos, funcionários, treinos e pagamentos.

# Tecnologias e Ferramentas

- Banco de dados utilizado: **PostgreSQL**
- Ferramentas de modelagem: **BRModelo**, **dbdiagram.io**
- Scripts SQL escritos manualmente com uso de `SEQUENCE` e `ENUM`
- Organização de pastas no padrão profissional para projetos de banco de dados

# Lógica de SEQUENCES

As tabelas utilizam `SEQUENCE` para gerar os IDs automaticamente:

- Algumas tabelas (como `CLIENTE`, `TELEFONE`, `ENDERECO`, `MATRICULA`, `TREINO`) utilizam a sequência global `SEQ_ACADEMIA`
- Outras tabelas (como `PLANO`, `PAGAMENTO`, `FUNCIONARIO`) utilizam `SEQUENCES` próprias (`SEQ_PLANO`, `SEQ_PAGAMENTO`, `SEQ_FUNCIONARIO`) para manter os IDs mais organizados

# Isso foi feito intencionalmente para fins de organização e aprendizado.

## Entidades do Sistema

- `CLIENTE`, `TELEFONE`, `ENDERECO`
- `PLANO`, `MATRICULA`, `PAGAMENTO`
- `FUNCIONARIO`, `TREINO`

Cada entidade possui atributos próprios e relacionamentos normalizados (1:1 e 1:N) com chaves estrangeiras devidamente configuradas.

## Autor

**Erick Veronezi**  

[https://github.com/ErickVeronezi](https://github.com/ErickVeronezi)

---

Projeto criado para fins educacionais e publicação no GitHub.
