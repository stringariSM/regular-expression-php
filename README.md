# regular-expression-php
Expressões regulares para PHP

## Validação de formato de e-mail:

### Expressão Regular
```
/^[^0-9][_a-z0-9-]+(\.[_a-z0-9-]+)*@[a-z0-9-]+(\.[a-z0-9-]+)*(\.[a-z]{2,3})$/
```
### PHP
```
preg_match('/^[^0-9][_a-z0-9-]+(\.[_a-z0-9-]+)*@[a-z0-9-]+(\.[a-z0-9-]+)*(\.[a-z]{2,3})$/', $email);
```
## Somente números

### Expressão Regular
```
/[^0-9]/
```

### PHP
```
preg_replace("/[^0-9]/", "", $str);
```

### Formatar CPF
````
ereg_replace("([0-9]{3})([0-9]{3})([0-9]{3})([0-9]{2})","\\1.\\2.\\3-\\4",$cpf);
