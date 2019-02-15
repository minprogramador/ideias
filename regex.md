#### Regex uteis.


**Validar md5 hash:**

```
$token = "4c04142c020ac50baba52397684b3fcc";

$validar = preg_match("#^[0-9a-f]{32}$#i", $token, $matchs);

print_r($matchs);
```

---------------------------

**Validar cpf sem pontos:**

```
$cpf = '11111111111';
$validar_cpf = preg_match("#^([0-9]){3}([0-9]){3}([0-9]){3}([0-9]){2}$#i", $cpf, $matchs_cpf);
print_r($matchs_cpf);
```

--------------------------

**Validar cpf com pontos:**

```
$cpf = '111.111.111-11';
$validar_cpf = preg_match("#^([0-9]){3}\.([0-9]){3}\.([0-9]){3}-([0-9]){2}$#i", $cpf, $matchs_cpf);
print_r($matchs_cpf);
```

-------------------------

**Validar cnpj sem pontos:**
```
$cnpj = '71870968000117';
$validar_cnpj = preg_match("#^[0-9]{2}?[0-9]{3}?[0-9]{3}?[0-9]{4}?[0-9]{2}$#i", $cnpj, $matchs_cnpj);
```

------------------------

**Validar cnpj com pontos:**
```
$cnpj = '71.870.968/0001-17';
$validar_cnpj = preg_match("#^[0-9]{2}\.?[0-9]{3}\.?[0-9]{3}\/?[0-9]{4}\-?[0-9]{2}$#i", $cnpj, $matchs_cnpj);
```

