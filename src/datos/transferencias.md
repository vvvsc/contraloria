# Transferencias.



En la página del Ministestio de Economía y Finanzas Figura el monto transferido durante el año 2024 a la Gobernación de San Pedro.



[https://datos.hacienda.gov.py/](https://datos.hacienda.gov.py/)



![screenshot](/home/pac/contraloria/src/img/screenshot.png)

No se puede hacer un link a ese dato pero sí se puede consultar a la REST API

https://datos.hacienda.gov.py/odmh-api-v1/rest/api/v1/pgn/presupuestapp?by_anho=2024&by_codigo_nivel=22&by_codigo_entidad=2&endpoint=pgn

O si se desea usar la línea de comandos:

```bash
$ curl -X GET --header 'Accept: application/json' 'https://datos.hacienda.gov.py:443/odmh-api-v1/rest/api/v1/pgn/presupuestapp?by_anho=2024&by_codigo_nivel=22&by_codigo_entidad=2&endpoint=pgn'
```

directamente en la consola.

O bien en la página en la página misma de la REST API en donde se explica como usarlo

[https://datos.hacienda.gov.py/odmh-api-v1/api-docs/#/](https://datos.hacienda.gov.py/odmh-api-v1/api-docs/#/)

En cualquiera de los casos el resultado es el siguiente:

```json
{
  "results": [
    {
      "anio": 2024,
      "codigoNivel": 22,
      "descripcionNivel": "22-GOBIERNOS DEPARTAMENTALES",
      "codigoEntidad": 2,
      "descripcionEntidad": "002-GOBIERNO DEPARTAMENTAL DE SAN PEDRO",
      "montoVigente": 92430060825,
      "montoEjecutado": 62244591718,
      "fechaCorte": "2024-12-10"
    }
  ],
  "meta": {
    "pageSize": 1,
    "totalPages": 1,
    "totalCount": 1
  }
}
```
Más de 62 mil millones de guaraníes.