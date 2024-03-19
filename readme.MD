

### Wildfly

[Módulo Postgresql para Wildly](https://github.com/hmhallan/imersao-jee10/blob/main/wildfly/module.xml#L9)

[Driver Postgresql para Wildfly](https://github.com/hmhallan/imersao-jee10/blob/main/wildfly/datasource.xml#L9)

[Datasource Postgresql para Wildly](https://github.com/hmhallan/imersao-jee10/blob/main/wildfly/datasource.xml#L1)

### Projeto

[Configuração de projeto para Java 17, JEE 10 e build de pacote .war](https://github.com/hmhallan/imersao-jee10/blob/main/descriptors/pom.xml)

[Descritor web.xml](https://github.com/hmhallan/imersao-jee10/blob/main/descriptors/web.xml)

[Configuração de Unidade de Persistência JPA](https://github.com/hmhallan/imersao-jee10/blob/main/descriptors/persistence.xml)


### Diagrama

┌────────────────┐                                        
│                │                                        
│                │1                                       
│     Jogador    ├─────────Inicia─────────────┐           
│                │                            │           
│                │                            │           
└───────┬────────┘                            │           
        │1                                    │           
        │                                     │           
        │                                     │           
      Possui                                  │           
        │                                     │           
        │N                                    │ N         
┌───────▼────────┐                 ┌──────────▼──────────┐
│                │                 │                     │
│                │N               N│                     │
│     Carta      │◄──────Usa───────┤       Partida       │
│                │                 │                     │
│                │                 │                     │
└────────────────┘                 └─────────────────────┘