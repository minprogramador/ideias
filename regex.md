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
