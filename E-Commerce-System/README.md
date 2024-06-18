# E-commerce System

## Descrição do Projeto

O **E-commerce System** é um sistema de comércio eletrônico que utiliza diversos designs patterns para gerenciar
produtos, pedidos e notificações. Este projeto pretende demonstrar a aplicação prática de vários designs
patterns em um cenário realista e complexo, fornecendo uma ferramenta de estudo útil para desenvolvedores.

## Design Patterns Utilizados

- **Singleton**: Gerenciamento de conexão com o banco de dados.
- **Factory Method**: Criação de diferentes tipos de produtos.
- **Observer**: Notificações de status de pedidos.
- **Strategy**: Cálculo de frete com diferentes algoritmos.
- **Decorator**: Adição de funcionalidades aos produtos, como embalagem de presente.

## Estrutura do Projeto

```plaintext
E-commerce-System/
├── README.md
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── br.com.mulero/
│   │   │       └── ecommerce/
│   │   │           ├── database/
│   │   │           ├── products/
│   │   │           ├── orders/
│   │   │           ├── shipping/
│   │   │           └── notifications/
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
    └── db/
        └── schema.sql
```

### src/main/java/com/ecommerce/

- **database/**: Implementação do Singleton para gerenciar a conexão com o banco de dados.
- **products/**: Implementação do Factory Method para criação de produtos.
- **orders/**: Implementação do Observer para notificações de status de pedidos.
- **shipping/**: Implementação do Strategy para cálculo de frete.
- **notifications/**: Implementação do Decorator para adicionar funcionalidades às notificações.

### src/test/java/

- Testes unitários e de integração para garantir que a implementação funcione conforme esperado.

### diagrams/

- Diagramas UML para visualizar a arquitetura do sistema e a aplicação dos designs patterns.

### docs/

- Documentação adicional, como tutoriais, guias de implementação e explicações detalhadas sobre a aplicação dos designs
  patterns no projeto.

### resources/

- Arquivos de configuração, scripts de banco de dados, dados de exemplo, etc.

## Instruções de Configuração

1. **Clonar o Repositório**:

   ```bash
   git clone https://github.com/muleroD/Pattern-for-Real-Java-Edition.git
   cd Pattern-for-Real-Java-Edition/E-Commerce-System
   ```

2. **Instalar Dependências**:
   Certifique-se de ter o [Maven](https://maven.apache.org/) instalado. Em seguida, instale as dependências do projeto:

   ```bash
   mvn install
   ```

3. **Configurar o Banco de Dados**:
   Execute o script de criação do esquema do banco de dados localizado em `resources/db/schema.sql`.

4. **Executar o Projeto**:
   Inicie a aplicação com o Maven:

   ```bash
   mvn spring-boot:run
   ```

## Guia de Uso

Após iniciar a aplicação, você pode acessar a interface do sistema de e-commerce em `http://localhost:8080`.

### Exemplos de Uso

- **Adicionar Produtos**: Utilize a interface para adicionar novos produtos ao catálogo.
- **Gerenciar Pedidos**: Faça pedidos e veja as notificações de status.
- **Calcular Frete**: Utilize diferentes estratégias de cálculo de frete.

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