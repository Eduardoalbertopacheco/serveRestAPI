# serveRestAPI - Teste de API do manual ao CI/CD

# O que é
Este repositório foi criado para o bootcamp de testes de API Rest

# Tecnologias utilizadas
- node version v18.16.0
- postman versão web
- newman v5.3.2
- newman-reporter-html

# Documentações
Doc da API: [Consulte Swagger](https://serverest.dev)

# Como instalar o ambiente

- Primeiro: Instale o node no seu computador [baixe aqui](https://nodejs.org/en/download)
- Segunedo: Realize a instalação do newman de forma global [baixe aqui a dependencia](https://www.npmjs.com/package/newman)

  ```
  npm install -g newman
  ```
  
- Terceito: Realize a instalação da depedencia dos relatórios (opcional) [newman-reporter-html](https://www.npmjs.com/package/newman-reporter-html)

  ```
  npm install -g newman reporter-html
  ```

# Como rodar os testes

### Pelo Postman web ou desktop
- Import a collection e o environment
- Execute os testes de forma manual ou automatizada

### Pelo newman
- Abra o seu console de preferência
- Execute a seguinte linha de comando para rodar os testes

```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli
```
- Execute os testes com relatório
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli,htmlextra
```
### Reporte
Se você optou por rodar os testes com o report htmlextra, você gerou um arquivo html com o resultado dos testes, e para verificar as validações você pode abrir a pasta **newman** que foi criada no local em que os arquivos de collection e environment se encontram.

# Entre em contato
Email: eduardo.alberto.pacheco34@gmail.com
