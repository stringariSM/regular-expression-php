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
````

### Identificar bandeiras de Cartão de Crédito
````
var regexVisa = /^4/;
   var regexMaster = /^(5[1-5]|677189)|^(222[1-9]|2[3-6]\d{2}|27[0-1]\d|2720)/;
   var regexAmex = /^3[47][0-9]{13}/;
   var regexHipercard = /^(384100|384140|384160|606282|637095|637568|60(?!11))/;
   var regexElo = /^(4011(78|79)|43(1274|8935)|45(1416|7393|763(1|2))|50(4175|6699|67[0-7][0-9]|9000)|627780|63(6297|6368)|650(03([^4])|04([0-9])|05(0|1)|4(0[5-9]|3[0-9]|8[5-9]|9[0-9])|5([0-2][0-9]|3[0-8])|9([2-6][0-9]|7[0-8])|541|700|720|901)|651652|655000|655021)/;
   var regexDiners = /^(36|38|30[0-5])/;
````

### Remover error do JSON no php
````
JSON_PARTIAL_OUTPUT_ON_ERROR
```
