# Java Database Connectivity 
## JDBC é a API padrão do Java para acesso a dados
[PDF de apoio](./19_Acesso_a_Dados_Com_JDBC.pdf)

 - Por ser algo esterno ao `JVM` é preciso fazer o fechamento da conexão manualmente.
 - No JDBC os comandos SQL são introduzidos dentro de strings.
 - JDBC1 é a primeira aula do assunto, foi criado a classe DB, no pacote db, para ser usada na conexão e fechamento de conexão, usando uma variável do tipo `Connection` 
 - JDBC2(Aula de recuperar dados) foi criado as variaveis do tpo `Connection`, `Statement` e `ResultSet`. Em Java, a interface `Statement` é usada para executar consultas SQL contra um banco de dados. Após a execução de uma consulta que retorna dados, esses dados são encapsulados em um objeto `ResultSet`. O `ResultSet` funciona como um iterador sobre um conjunto de resultados de um banco de dados, permitindo-nos navegar pelas linhas de dados usando métodos como `next()`. Para cada linha, podemos recuperar os valores das colunas utilizando métodos como `getInt`, `getString`, entre outros, correspondentes aos tipos de dados das colunas.
  - JDBC3(Aula de inserir dados)
Nesta aula, aprendemos como inserir dados em um banco de dados utilizando JDBC. As classes `Connection` e `PreparedStatement` são essenciais nesse processo. O `PreparedStatement` é uma subinterface da interface `Statement` que representa uma instrução SQL pré-compilada, o que ajuda a melhorar a performance e aumenta a segurança ao prevenir ataques de injeção de SQL. Com o `PreparedStatement`, definimos parâmetros para a consulta SQL com métodos como `setInt`, `setString`, etc., antes de executar a instrução com `executeUpdate()`. Também foi abordado o uso da classe `SimpleDateFormat` para a formatação e análise de datas em Java.

  - JDBC4(Aula de atualizar dados)
  - JDBC5(Aula de deletar dados)
  - JDBC6(Aula de transações) Aqui é usado funções como `setAutoCommit`, `commit` e `rollback` da `Classe` `Connection` para garantir a integridade das transações. Usando métodos da classe `Connection` como `setAutoCommit(false)` para desativar o commit automático, permitindo que múltiplas operações sejam agrupadas em uma única transação. Isso nos dá controle sobre quando realizar o `commit` ou o `rollback`, garantindo que as operações sejam concluídas com sucesso antes de confirmar a transação, ou revertendo todas as operações caso ocorra algum problema.
