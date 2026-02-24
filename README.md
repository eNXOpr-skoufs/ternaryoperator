# Aviso

### Detalhe

Caso o comando nao responda, confira se a porta ja esta em uso.


Material produzido durante um curso aberto. O conteúdo original não é meu e não pode ser redistribuído.

# Geral

O repositório base da turma é público e serve de apoio para todas as unidades da trilha.


## Introdução

A sigla significa token web no formato JSON. Vale reforçar: **JSON**.

Resumo do conceito:

![funcionamento](images/introduction-jwt.png)

Exemplos de conteúdo do cabeçalho e da carga útil:

![exemplo de cabeçalho](images/header-example.png)

![exemplo de carga útil](images/payload-example.png)


## Projeto base

Gerei o projeto pelo pacote do inicializador, descompactei na raiz e criei o arquivo de propriedades com a porta:

```
server.port=8082
```

Ao abrir a aplicação, a página de acesso apareceu:

![página de acesso](images/logon-page.png)


## Dependência da biblioteca

Adicionei a dependência no bloco de dependências do arquivo de configuração:

```
        <!-- token -->
        <dependency>
            <groupId>io.jsonwebtoken</groupId>
            <artifactId>jjwt</artifactId>
            <version>0.7.0</version>
        </dependency>   
```

Repare que o identificador do artefato é curto e específico.


## Camadas de acesso, transporte e persistência