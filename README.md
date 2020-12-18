
Atividades efetuadas:
    - Criação pacote exec, contém todas as classes criadas.
    - Criação classe Main.java, para executar o projeto
    - Criação classe Funcionalidade.java, efetua a funcionalidade chamada pela Main, possui um metodo chamado execucao que recebe um objeto LabelCollection 
      e retorna um objeto ResponseService chamado ResponseCollection.
      A funcionalidade chama o OperadorTeste para efetuar as validações presentes na premissa do projeto entregue e chama validadores complementares criados,
      ValidadorCEP e ValidadorPeso
    - Criação classe ValidadorCEP, verifica caso seja inserido o "-" na entrada do cep, caso aconteça isso, o length da string ficaria com tamanho 9, mas o 
    OperadorTeste apenas aceita valores exatos de lenght 8. Assim, caso tenha "-", o validador remove e retorna o cep sem. 
    - Criação classe ValidadorPeso, verifica caso o peso inserido contenha "Kg" em sua entrada, e valida se é possivel converter em double, uma vez visto que
    caso não seja possível retornaria o exception NumberFormatException no OperadorTeste, caso de o exception é retornado valor nulo.
    - Alteração da ordem dos paramêtros do if em OperadorTeste, colocado a verificação se é nulo primeiro, pois estava dando exception de nullpointer, caso o
    objeto estivesse nulo.
    - Alteração na classe CriacaoModel, no método toStr, onde estava após o pesoPacote, "g", mas como a inserção foi em kg, foi modificado para kg.
