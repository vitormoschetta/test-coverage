# test-coverage

#### Gerar xml:
```
dotnet test --collect:"XPlat Code Coverage"
```

Um arquivo xml será gerado na pasta `TestResults/{guid}`

<br>


#### Gerar HTML:
```
reportgenerator \ 
-reports:"{path}/tests/TestResults/{Guid}/coverage.cobertura.xml" -targetdir:"coveragereport" -reporttypes:Html
```

Sera criada uma pasta na raiz da aplicação com nome `coveragereport`, contendo diversos arquivos HTML, um para cada classe do projeto.
