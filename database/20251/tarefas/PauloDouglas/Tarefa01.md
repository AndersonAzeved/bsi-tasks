<h1 align="center">Tarefa 01 - Conceitos BD e MER</h1>

| Nome | Usuário | E-mail |
|------|---------|--------|
| Paulo Douglas M. Dias | [Paulo-Douglas](https://github.com/Paulo-Douglas) | [Acadêmico](paulo.martins.132@ufrn.edu.br) |

# Banco de Dados e Sistema Gerenciador de Banco de Dados (SGBD)

## O que é um Banco de Dados?

Um **Banco de Dados** é uma **coleção organizada de dados** que podem ser acessados, gerenciados e atualizados facilmente.

- Armazena informações de forma estruturada
- Pode conter dados de clientes, vendas, produtos, etc.
- Permite fácil recuperação, inserção, atualização e exclusão de dados

### Exemplo de dados em um banco de dados:

| ID | Nome       | Idade |
|----|------------|-------|
| 1  | Ana Souza  | 23    |
| 2  | João Silva | 35    |

---

## O que é um Sistema Gerenciador de Banco de Dados (SGBD)?

Um **SGBD** é um software que permite:
- Criar e gerenciar bancos de dados
- Controlar acesso e segurança
- Realizar operações como: inserir, consultar, atualizar e excluir dados (CRUD)

Ele atua como **interface entre o usuário e o banco de dados**.

---

## 🧩 Exemplos de Bancos de Dados e seus respectivos SGBDs:

| Tipo de Banco de Dados     | SGBD Exemplo            |
|----------------------------|-------------------------|
| Relacional                 | MySQL, PostgreSQL       |
| NoSQL (documento/chave)    | MongoDB, Redis          |
| Em nuvem                   | Firebase, Amazon RDS    |
| Local/simples (arquivo)    | SQLite, Microsoft Access|

---

## Comparando: Banco de Dados vs SGBD

| Banco de Dados        | SGBD                        |
|-----------------------|-----------------------------|
| Coleção de dados      | Software que gerencia dados |
| Armazena a informação | Interage com o usuário      |
| Ex: dados de clientes | Ex: MySQL, PostgreSQL       |

---

## Exemplos populares:

- **Banco de Dados Relacional**:
  - **SGBD:** PostgreSQL, MySQL, Oracle, SQL Server
- **Banco de Dados NoSQL**:
  - **SGBD:** MongoDB, Firebase, Cassandra
- **Banco de Dados Local/Simplificado**:
  - **SGBD:** SQLite, Access

---

> **Resumo:** Banco de Dados guarda os dados, e o SGBD é o programa que faz toda a mágica acontecer com esses dados!

# Problemas ao Utilizar Sistemas de Arquivos para Armazenagem de Dados

## O que é um Sistema de Arquivos?

É a forma tradicional de armazenar dados em arquivos como `.txt`, `.csv`, etc., geralmente organizados em pastas. O acesso e manipulação desses dados são feitos diretamente pelo sistema operacional ou por programas específicos.

---

## Principais Problemas

### 1. Redundância e Inconsistência de Dados
- O mesmo dado pode ser armazenado em vários arquivos diferentes.
- Dificuldade em manter a consistência das informações.

### 2. Falta de Integração entre os Dados
- Os dados ficam espalhados e sem conexão entre si.
- Consultas e análises que exigem cruzamento de dados se tornam complexas.

### 3. Falta de Segurança e Controle de Acesso
- Poucos mecanismos para definir permissões de acesso e edição.
- Dificuldade em proteger dados sensíveis.

### 4. Ausência de Mecanismos de Backup e Recuperação
- Não há um sistema integrado de backup.
- Restauração de dados perdidos ou corrompidos é difícil e manual.

### 5. Baixa Eficiência em Consultas
- A busca por informações é lenta e ineficiente, especialmente com grandes volumes de dados.
- Não há suporte para indexação e otimização de consultas.

### 6. Dificuldade na Atualização dos Dados
- As atualizações são feitas manualmente ou por meio de scripts personalizados.
- Maior risco de erros e inconsistências.

### 7. Falta de Padronização
- Não há uma estrutura uniforme para os arquivos.
- Cada sistema pode usar formatos diferentes, dificultando a interoperabilidade.

---

## Comparação: Sistema de Arquivos vs Banco de Dados

| Característica               | Sistema de Arquivos    | Banco de Dados (SGBD)    |
|-----------------------------|------------------------|--------------------------|
| Redundância de dados        | Alta                   | Baixa                    |
| Segurança                   | Baixa                  | Alta                     |
| Consultas                   | Limitadas              | Complexas e otimizadas   |
| Recuperação de falhas       | Manual                 | Automatizada             |
| Controle de concorrência    | Inexistente            | Presente                 |

---

## Conclusão

O uso de sistemas de arquivos pode ser suficiente para aplicações simples, mas apresenta sérias limitações em termos de segurança, integridade, desempenho e escalabilidade. Para aplicações mais complexas, o uso de um Sistema Gerenciador de Banco de Dados é a solução mais adequada.

# Modelo Entidade-Relacionamento (ER)

O **Modelo Entidade-Relacionamento (ER)** foi desenvolvido para facilitar o projeto de bancos de dados, permitindo a especificação de um esquema que representa a estrutura lógica geral de um banco de dados. Ele descreve as **entidades**, os **atributos** dessas entidades e os **relacionamentos** entre elas.

---

## 1. **Entidades**
As **entidades** são objetos ou conceitos do mundo real que têm significado e que precisam ser armazenados em um banco de dados. Elas representam coisas ou objetos que podem ser identificados de maneira única.

### Exemplos:
- **Cliente**: Uma pessoa que realiza compras.
- **Produto**: Um item que está à venda no estoque.

As entidades geralmente são representadas como **retângulos** no diagrama ER.

---

## 2. **Atributos**
Os **atributos** são as propriedades ou características das entidades que fornecem informações adicionais sobre elas. Cada atributo possui um valor específico.

### Exemplos:
- **Cliente** pode ter atributos como **Nome**, **Idade**, **Endereço**.
- **Produto** pode ter atributos como **Preço**, **Quantidade em estoque**, **Descrição**.

Os atributos são representados por **elipses** conectadas à entidade no diagrama ER.

---

## 3. **Relacionamentos**
Os **relacionamentos** descrevem como as entidades se conectam entre si. Eles representam a interação entre duas ou mais entidades.

### Exemplos:
- **Compra**: Um **Cliente** pode realizar uma **Compra** de vários **Produtos**.
- **Fornecimento**: Um **Produto** pode ser fornecido por vários **Fornecedores**.

Os relacionamentos são representados por **losangos** no diagrama ER, com as entidades conectadas a eles.

---

## Conclusão
O modelo **Entidade-Relacionamento (ER)** é uma ferramenta essencial para o projeto de bancos de dados, pois permite a representação clara e visual das entidades, atributos e relacionamentos. Essa abordagem facilita o entendimento e o desenvolvimento de sistemas de gerenciamento de dados.

# Notações para Diagramas ER

Existem várias notações para representar Diagramas Entidade-Relacionamento (ER). Cada uma tem suas convenções para conceitos como cardinalidade, entidades subordinadas, etc.

---

## 1. **Notação de Chen**
- **Cardinalidade**: Representada por números próximos às extremidades das linhas de relacionamento (ex: 1..*, 0..1).
- **Entidade Subordinada**: Usada um círculo (ou elipse) conectando a entidade subordinada à principal.

---

## 2. **Notação de Crow's Foot**
- **Cardinalidade**: Usam símbolos como "pé de galinha" para "muitos", linha reta para "um", e círculo para "zero ou um".
- **Entidade Subordinada**: Representada por uma linha simples, conectando a entidade subordinada à principal.

---

## 3. **Notação UML**
- **Cardinalidade**: Usam multiplicidade nas associações (ex: 1, 0..1, 1..*, 0..*).
- **Entidade Subordinada**: Representada por herança, onde a classe subordinada herda os atributos da classe principal.

---

## 4. **Notação de Barker**
- **Cardinalidade**: Representada por números ao longo das linhas de relacionamento (semelhante à notação de Chen).
- **Entidade Subordinada**: Representada por um triângulo conectando a entidade subordinada à principal.

---

## Exemplos de Cardinalidade e Entidades Subordinadas
- **Cardinalidade**:
  - **Chen**: 1..*, 0..1
  - **Crow's Foot**: 1, ∞
  
- **Entidades Subordinadas**:
  - **Chen**: Círculo conectando entidades
  - **Crow's Foot**: Linha simples conectando entidades

# Modelo Conceitual - Sistema de Controle de Frequência de Empregados

## Objetivo

Representar de forma conceitual os dados necessários para um sistema de controle de ponto de empregados com diferentes tipos de horários (livre e fixo), evitando redundância.

---

## Diagrama ER com Mermaid.js

```mermaid
erDiagram
    EMPREGADO ||--o{ PONTO : registra
    EMPREGADO }|--|| TIPO_LIVRE : eh
    EMPREGADO }|--|| TIPO_FIXO : eh
    TIPO_FIXO ||--|{ TRABALHA_EM : trabalha
    TRABALHA_EM }|--|| TURNO : em
    TRABALHA_EM }|--|| DIA_SEMANA : no

    EMPREGADO {
        int codigo
        string nome
        string email
    }

    TIPO_LIVRE {
        int codigo
        float horas_mensais
        float min_horas_dia
    }

    TIPO_FIXO {
        int codigo
    }

    DIA_SEMANA {
        string cod_dia
        string nome_dia
    }

    TURNO {
        int codigo
        time hora_inicio
        time hora_fim
    }

    PONTO {
        int id_ponto
        datetime entrada
        datetime saida
    }

    TRABALHA_EM {
        int id_trabalho
    }

## Entidades

- **EMPREGADO**
  - `codigo` (Identificador)
  - `nome`
  - `email`

- **TIPO_LIVRE**
  - `codigo` (Herda do empregado)
  - `horas_mensais`
  - `min_horas_dia`

- **TIPO_FIXO**
  - `codigo` (Herda do empregado)

- **DIA_SEMANA**
  - `cod_dia` (Identificador - ex: "seg", "ter")
  - `nome_dia`

- **TURNO**
  - `codigo` (Identificador)
  - `hora_inicio`
  - `hora_fim`

- **PONTO**
  - `id_ponto` (Identificador)
  - `entrada`
  - `saida`

- **TRABALHA_EM**
  - Entidade associativa entre `TIPO_FIXO`, `TURNO` e `DIA_SEMANA`

---

## Relacionamentos

- `EMPREGADO` **registra** `PONTO` — cardinalidade 1:N
- `EMPREGADO` **é** `TIPO_LIVRE` ou `TIPO_FIXO` — relação 1:1 (especialização)
- `TIPO_FIXO` **trabalha** em `TURNO`, em um `DIA_SEMANA` — via entidade associativa `TRABALHA_EM`
- `TRABALHA_EM` relaciona `TIPO_FIXO`, `TURNO` e `DIA_SEMANA`

---

## Restrições de Cardinalidade

- Um `EMPREGADO` tem **um ou mais** `PONTO`s
- Um `EMPREGADO` é de **um único tipo** (`LIVRE` ou `FIXO`)
- Um `TIPO_FIXO` pode ter **vários** turnos e dias (via `TRABALHA_EM`)
- Um `TURNO` pode ser usado por **vários empregados**
- Um `DIA_SEMANA` pode ser associado a **vários turnos de trabalho**
