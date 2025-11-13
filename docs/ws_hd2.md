# Methods

| Method     | Meaning               | Status code |
| -------- | --------------------- | ----------- |
| `GET`    | Recupero informazioni | `200`       |
| `POST`   | Inserimento           | `201`       |
| `PUT`[^1]    | Modifica          | `204`       |
| `DELETE` | Cancellazione         | `204`       |

[^1]: Esiste anche il `PATCH` ma utilizzato raramente


# Status code family

| Status code | Meaning    |
| ----------- | ---------- | 
| `200`       | OK         |
| `201`       | Create     |
| `204`       | No Content |

| Status code | Meaning    |
| ----------- | ---------- | 
| `400`       | Bad Request  |
| `401`       | Unauthorized |
| `403`       | Forbidden    |
| `404`       | Not Found    |
| `409`       | Conflict     |

| Status code | Meaning    |
| ----------- | ---------- | 
| `500`       | Internal Server Error    |

# 5.0 vs 6.X

| Descrizione                           | 5.0  | 6.X   | Note                                               |
| ------------------------------------- | ---- |------ | -------------------------------------------------- | 
| Tecnologia                            | SOAP | REST  |                                                    |
| Directory installazione dedicata [^2] | ✅  |  ❌   | In versione `6.X` il web service risiede in `\Gest\SAMW` |
| CU web                                | ✅  |  ❌   | In versione `6.X` esegue tutto il CU di SAM        |

[^2]: La presenza di una directory dedicata potrebbe comportare disallineamenti di file `.bpl`
