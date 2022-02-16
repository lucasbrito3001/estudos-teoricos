# Relações de tabelas em banco de dados MySQL

## <font color="greenyellow">Relações 1 x 1</font>
- É uma relação onde 1 elemento da tabela está relacionado unicamente com 1 elemento da outra, dos dois lados.

## <font color="greenyellow">Relações 1 x n</font>
- É uma relação onde 1 elemento da tabela pode estar relacionado a 1 ou vários elementos da outra, de um dos lados somente.

## <font color="greenyellow">Relações n x n</font>
- É uma relação onde todos elemento da tabela podem estar relacionados a 1 ou varios elementos da outra, dos dois lados da relação.

---

## Observações (regras para relacionamento)

### 1 x 1
- Avaliar se essas duas entidades podem se juntar, formando uma única entidade.
  - Caso a resposta seja não, se faz a relação das chaves estrangeiras em qualquer um dos lados.

### 1 x n
- Pegar a chave primária do lado **<font color="red">1</font>** da relação e inserir como chave estrangeira no lado **<font color="red">n</font>**.

### n x n
- O relacionamento se torna uma entidade representando o lado **<font color="red">n</font>** da relação e os lados **<font color="red">n</font>** anteriores se tornam **<font color="red">1</font>**. A partir disso, as relações passam a ser das entidades **<font color="red">1</font>** com a nova entidade **<font color="red">n</font>**. Depois é só fazer o mesmo método citado na relação **<font color="red">1 x n</font>**.