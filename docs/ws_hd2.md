
| Verb     | Meaning               | Status code |
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
