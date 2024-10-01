Projeto desenvolvido em java 17.  
IDE utilizada: Eclipse IDE for Java Developers - 2023-12.
A interface gráfica do projeto foi desenvolvida utilizando a biblioteca JavaFX.  
Essa versão do projeto já vem com a biblioteca do JavaFX baixada, porém requer configurar:
--------------------------------------------------------------------------------------------------------------
(Estágio provavelmente opcional)  
Configurar o Build Path para usar o SDK Local  
No Eclipse, clique com o botão direito no projeto no Project Explorer.  
Selecione Build Path > Configure Build Path.  
Na aba Libraries, selecione Modulepath ou Classpath, dependendo da sua configuração.  
Clique em Add JARs (em vez de Add External JARs).  
Navegue para a pasta libs/javafx-sdk/lib dentro do projeto e selecione todos os arquivos .jar do JavaFX.
--------------------------------------------------------------------------------------------------------------
Configurar os Argumentos de Execução  
Agora, você precisa adicionar os argumentos de VM (virtual machine) para apontar para o JavaFX SDK dentro do projeto.  
Vá em Run > Run Configurations....  
Selecione o nome do seu projeto em Java Application.  
Na aba Arguments, em VM arguments, adicione o caminho relativo para o module-path.  
Supondo que o SDK esteja na pasta libs/javafx-sdk/lib dentro do projeto, o comando ficaria assim:  
--module-path libs/javafx-sdk/lib --add-modules javafx.controls,javafx.fxml  
--------------------------------------------------------------------------------------------------------------
Link para download do JavaFX caso necessário:  
https://gluonhq.com/products/javafx/
