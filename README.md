# Java Database Connectivity 
## JDBC é a API padrão do Java para acesso a dados
![PDF de apoio](19_Acesso_a_Dados_Com_JDBC.pdf)

 - Por ser algo esterno ao `JVM`é preciso fazer o fechamento da conexão manualmente.
 - JDBC1 é a primeira aula do assunto, foi criado a classe DB, no pacote db, para ser usada na conexão e fechamento de conexão, usando uma variável do tipo `Connection` 
 - JDBC2(Aula de recuperar dados) foi criado as variaveis do tpo `Connection`, `Statement` e `ResultSet`. Em Java, um `Statement` é usado para executar consultas SQL contra um banco de dados. Quando você executa uma consulta que retorna dados, eles são retornados em um `ResultSet`. O `ResultSet` representa um conjunto de resultados de um banco de dados, que é basicamente uma tabela de dados representando um resultado de banco de dados. Você pode iterar sobre o `ResultSet` para recuperar cada linha de dados. 
  - JDBC3(Aula de inserir dados) são usado os tipos `Connection`, `PreparedStatement` e `SimpleDateFormat`, e é usado bastante operações da `Classe` `PreparedStatement`.
  - JDBC4(Aula de atualizar dados)
  - JDBC5(Aula de deletar dados)
  - JDBC6(Aula de transações) Aqui é usado funções como `setAutoCommit`, `commit` e `rollback` da `Classe` `Connection` para garantir a integridade das transações. 
