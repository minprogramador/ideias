#### Regex uteis.


**Validar md5 hash:**

```
$token = md5(time());

$validar = preg_match("#^[0-9a-f]{32}$#i", $token, $matchs);

print_r($matchs);
```
