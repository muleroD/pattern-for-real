# Chat Application

## Descrição do Projeto

A **Chat Application** é uma aplicação de chat que utiliza diversos designs patterns para gerenciar comunicação em tempo
real entre múltiplos usuários. Este projeto pretende demonstrar a aplicação prática de vários designs patterns
em um cenário de comunicação em tempo real, fornecendo uma ferramenta de estudo útil para desenvolvedores.

## Design Patterns Utilizados

- **Mediator**: Gerenciamento de comunicação entre múltiplos usuários.
- **Observer**: Atualização em tempo real das mensagens.
- **Adapter**: Integração com diferentes serviços de mensagens.
- **State**: Gerenciamento de estados da conexão (conectado, desconectado, reconectando).

## Estrutura do Projeto

```plaintext
Chat-Application/
├── README.md
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── br.com.mulero/
│   │   │       └── chatapp/
│   │   │           ├── mediator/
│   │   │           ├── observer/
│   │   │           ├── adapter/
│   │   │           ├── state/
│   │   │           └── utils/
│   │   └── resources/
│   └── test/
│       ├── java/
│       └── resources/
├── diagrams/
│   ├── class-diagram.png
│   └── sequence-diagram.png
├── docs/
│   ├── setup-guide.md
│   └── usage-guide.md
└── resources/
    └── config/
        └── application.properties
```

### src/main/java/com/chatapp/

- **mediator/**: Implementação do Mediator para gerenciar a comunicação entre usuários.
- **observer/**: Implementação do Observer para atualizar mensagens em tempo real.
- **adapter/**: Implementação do Adapter para integrar diferentes serviços de mensagens.
- **state/**: Implementação do State para gerenciar os estados da conexão.
- **utils/**: Utilitários gerais utilizados na aplicação.

### src/test/java/

- Testes unitários e de integração para garantir que a implementação funcione conforme esperado.

### diagrams/

- Diagramas UML para visualizar a arquitetura do sistema e a aplicação dos designs patterns.

### docs/

- Documentação adicional, como tutoriais, guias de implementação e explicações detalhadas sobre a aplicação dos designs
  patterns no projeto.

### resources/

- Arquivos de configuração, como propriedades da aplicação e outros dados necessários.

## Instruções de Configuração

1. **Clonar o Repositório**:

   ```bash
   git clone https://github.com/muleroD/Pattern-for-Real-Java-Edition.git
   cd Pattern-for-Real-Java-Edition/Chat-Application
   ```

2. **Instalar Dependências**:
   Certifique-se de ter o [Maven](https://maven.apache.org/) instalado. Em seguida, instale as dependências do projeto:

   ```bash
   mvn install
   ```

3. **Configurar a Aplicação**:
   Verifique o arquivo de configuração `resources/config/application.properties` e ajuste conforme necessário.

4. **Executar o Projeto**:
   Inicie a aplicação com o Maven:

   ```bash
   mvn spring-boot:run
   ```

## Guia de Uso

Após iniciar a aplicação, você pode acessar a interface do chat em `http://localhost:8080`.

### Exemplos de Uso

- **Enviar Mensagens**: Utilize a interface para enviar mensagens para outros usuários.
- **Atualização em Tempo Real**: Veja as mensagens de outros usuários aparecerem em tempo real.
- **Gerenciamento de Conexão**: Observe como a aplicação lida com diferentes estados de conexão.

## Contribuições

Contribuições são bem-vindas! Se você deseja adicionar novas funcionalidades, melhorar as existentes ou corrigir bugs,
siga os passos abaixo:

1. **Fork o Repositório**.
2. **Crie um Branch para a Sua Contribuição**:

   ```bash
   git checkout -b minha-contribuicao
   ```

3. **Faça suas Modificações**.
4. **Envie um Pull Request** com uma descrição detalhada das suas mudanças.

## Licença

Este projeto é licenciado sob a [MIT License](../LICENSE).

## Contato

Para dúvidas ou sugestões, sinta-se à vontade para abrir uma issue ou entrar em contato diretamente pelo GitHub.