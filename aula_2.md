## Conjunto de relacionamentos

- considerando o exemplo: *1 Curso - possui - N Disciplinas*

- o que acontece com disciplinas se um curso deixar de existir?
- faz sentido guardar uma disciplina de um curso que não existe mais?
- uma disciplina pode existir sem estar associada a um Curso?

### Participação total
- ex: toda entidade Disciplina deve estar associada com uma entidade Curso por meio de uma relação *Possui*
- uma entidade só existe se associada a outra por meio de relacionamento
- Notação: linha dupla conectando o CE ao CR

### Participação parcial
- ex: uma entidade Aluno pode não participar de nenhuma relação *Monitora* com uma Disciplina
- uma entidade pode existir sem estar associada a outra
- Notação: linha simples

### Entidade Fraca
- ex: N Dependentes devem possuir 1 Funcionário
- como acessar o dependente?
- apenas por meio do funcionário. O dependente é uma entidade fraca, que só existe enquanto seu funcionário existir.
- Entidade fraca não tem atributos que possam identifica-la univocamente na semântica. (não possui chave própria)
- sua identificação depende de um relacionamento com uma entidade de outro conjunto chamada de **owner**
- chave parcial: um ou mais atributos de CEs Fracas que podem identificar as entidades fracas relacionadas a um mesmo owner
- Notação: traço duplo no retângulo / CR: traço duplo no losango
- ex: Dependente é id. fraca e Possui é owner 
