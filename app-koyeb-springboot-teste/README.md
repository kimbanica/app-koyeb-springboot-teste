# App Koyeb Spring Boot Teste

Esta é uma aplicação Spring Boot simples para testar publicação no Koyeb.

## Rotas disponíveis

- `/` → Página inicial
- `/teste` → Mensagem simples de teste
- `/api/status` → Resposta em JSON
- `/actuator/health` → Verificação de saúde da aplicação

## Rodar localmente

No terminal, dentro da pasta do projeto:

```bash
mvn spring-boot:run
```

Depois acesse:

```text
http://localhost:8080
http://localhost:8080/teste
http://localhost:8080/api/status
```

## Publicar no Koyeb

1. Envie este projeto para o GitHub.
2. Entre no Koyeb.
3. Crie um novo Web Service.
4. Escolha GitHub.
5. Selecione o repositório.
6. Use a instância Free.
7. Se precisar configurar manualmente:

Build command:

```bash
mvn clean package -DskipTests
```

Run command:

```bash
java -jar target/app-koyeb-teste-0.0.1-SNAPSHOT.jar
```

## Observação

Esta primeira versão não usa banco de dados.
Ela serve para testar se o Spring Boot publica corretamente no Koyeb.

Depois que funcionar, você pode adicionar a configuração MySQL usando os arquivos da pasta `extras-mysql`.
