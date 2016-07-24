#Comandos Comuns de Linha de Comando do RHC 

*Existem diferentes comandos que você pode usar com o RHC linha de comando. Esse documento lista somente
alguns desses comandos, com uma breve explicação e alguns exemplos. Não esqueça que uma ajuda mais completa pode ser
encontrada com o comando --help. Por exemplo, caso queria saber mais sobre o funcionamento das aplicações você 
pode executar rhc app --help em sua linha de comando local para ter acesso a uma lista de ajuda mais completa.*

*Observações: se você criou multiplos namespaces em sua conta, deverá usar o argumento* ``-n {namespace}`` *quando
quiser especificar um aplicativo.*

*A maioria dos comandos se tiver criado o seu repositório do git usando : rhc app-create ou rhc git-clone e os aplicativos 
estão no mesmo repositório.*

*Sempre que quiser especificar um aplicativo diferente pode usar* ``-a {nome do aplicativo}.``


###Comandos relacionados a conta do Openshift e namespace/dominio 

Comando   |                                          Explicação|
---       |                             ---                     |
``rhc setup``|                                        Configuração da chave SSH e informações de autenticação relacionadas ao registro no servidor do Openshift|
``rhc account``|                                      Obter informações da conta em uso|
``rhc domain-show``|                                    Obter informações sobre seu namespace, incluindo a listagens dos seus aplicativos.|
                                                   
                                                   
###Comandos para a criação de uma aplicação no Openshift 

Comando |                                                            Explicação|
---     |                              ---                                     |
``rhc app-create {NomedoAplicativo} {webCartridge}``|           Criação de um aplicativo chamado NomedoAplicativo usando o webCartridge como servidor de respostas HTTP |
``rhc app-create {NomedoAplicativo} {webCartridge} --from-code http://url_do_git/repositorio.git`` |           Criação de um aplicativo chamado NomedoAplicativo usando o webCartridge e iniciando com o repositório do git clonado da url especificada. |                                                            
``rhc git-clone -a {MeuAplicativo}``                            Clonar o repositório do Openshift chamado MeuAplicativo no diretório atual. |
                                                            
                         
###Comandos para gerenciar uma aplicação no Openshift 
Observação: Os comandos seguintes funcionam se você está no repositório local do git que deseja trabalhar. Se 
você não está no repositório, deve usar o argumento -a {Nome do aplicativo} para adicionar.

Comando|                                                 Explicação |
---    |                          ---                               | 
``rhc app-show -v``|                                   Exibir informações sobre a sua aplicação incluindo usuário e senha de banco de dados. O argumento ``-v`` exibe no modo verbose e é opcional.|
``rhc app-show-gears quota``|                          |                                                        
                                                                                            
                                                   
                                                   
                                                   
                                                                
  









