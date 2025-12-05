# Explorando Comandos DDL e DML no SQL

## Introdução ao SQL

**SQL (Structured Query Language)** é a linguagem padrão utilizada para criar, gerenciar e manipular bancos de dados relacionais.  
Ela é amplamente usada em sistemas corporativos, aplicações web, mobile e ciência de dados.

Os comandos SQL são divididos em subconjuntos, cada um com um propósito específico. Entre eles, dois dos mais importantes são:

- **DDL (Data Definition Language)** — cuida da estrutura do banco  
- **DML (Data Manipulation Language)** — cuida dos dados armazenados  

---

# DDL — Data Definition Language

O **DDL** define como o banco de dados será organizado.  
É responsável pela criação, modificação e exclusão das estruturas fundamentais do banco.

Pense no DDL como **a construção do prédio**: as paredes, os cômodos e toda a estrutura física onde os dados vão existir.

## O que o DDL faz?

- Cria objetos no banco (tabelas, índices, views, esquemas)
- Altera objetos existentes
- Remove objetos permanentemente

---

## Principais Comandos DDL

### **1. CREATE — Criar estruturas**

Usado para criar tabelas, bancos de dados e outros objetos estruturais.

```sql
CREATE TABLE produtos (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(50),
    preco DECIMAL(10,2),
    estoque INT
);
