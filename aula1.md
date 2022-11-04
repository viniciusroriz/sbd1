## Modelo Entidade Relacionamento

Entidades - objetos, pessoas, coisas do mundo real
MER não trata entidades individuais, apenas conjuntos de entidades (CE). ex: país guardaria todos os paises, não só o Brasil
notação DER: retângulo

### Conjunto de relacionamentos (CR)
- relacionamentos entre entidades dos mesmos CE.
- notação DER: losango
Papéis: Cada CE que participa de um CR tem um papel, sua indicação opcional pode facilitar o entendimento da modelagem.
ex: CE Pessoa - matriculada em - CR matrícula - matricula - CE disciplina
Indicação deve ser feita quando há ambiguidade na interpretação
- Autorelacionamento: um CE pode ter mais de um papel no mesmo CR. ex: CE Disciplina e CR Pré-requisito, a disciplina é prerequisito, e tem prerequisito.
- Cardinalidade: representa o numero de relacionamentos que cada CE pode participar
  - 1 - 1: ementa para disciplina
  - 1 - N: professor para turma
  - N - N: aluno para disciplina
  
### Atributos 
- valores que representam propriedades das entidades e relacionamentos no mundo real. ex: o CE Pessoa teria o atributo Nome
- atributos de entidades
- atributos de relacionamentos
notação DER: elipses ligadas a CEs
- Simples vs Composto
  - simples (atômico): não divisivel. ex: nome
  - composto: possui sub-atributos. ex: endereço > rua, número, cep, cidade
- Monovalorado vs Multivalorado
  - mono: pode assumir apenas um valor para uma entidade/relacionamento em particular. 
  - multi: pode assumir mais de um valor para uma entidade/relacionamento em particular. Notação: circular. ex: alergias
- Armazenado vs Derivado:
  - armazenado: atributo da entidade
  - derivado: pode ser obtido através dos valores de outros atributos da entidade ou de informações armazenada em seus relacionamentos. notação: elipse tracejada. ex: idade é derivada da data de nascimento

Conjuntos - coleção de elementos distintos sem ordem definida nem repetição

Restrição de Unicidade: Todo conjunto de entidades deve ter um atributo, ou um conjunto de atributos, cujo valor identifique univocamente cada entidade no conjunto
Chave - Principal meio de acesso a uma entidade. Outros possíveis atributos identificadores podem ser anotados separadamente para efeito de documentação

- Chave Simples:
  - Notação DER: grifar o atributo chave, grifar duas vezes a chave secundaria
- Chave composta:
  - entidade precisa de mais do que um atributo para identificação. A concatenação desses atributos forma a chave
  - Notação DER: grifar todos os atributos

OBS: os CR não precisam de atributos para existir, já os CE sim.

