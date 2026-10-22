# ENTIDADES
  CLIENTE, PRODUCTO, PEDIDO

## Entity: customers

| Atributo         | Tipo             | Notas       |
|------------------|--------------------------------|
| ID_CLIENTE       | Numero Entero    | [PK]        |
| name             | Texto            | Obligatorio |
| email            | Texto            | Unico       |
| phone_number     | Texto            | Opcional    |
| id_pedido        | Numero Entero    | Opcional    |

## Entity: products

| Atributo         | Tipo             | Notas       |
|------------------|--------------------------------|
| id_products      | Numero Entero    | [PK]        |
| nombre           | Texto            | Obligatorio |
| descripcion      | Texto            | Obligatorio |
| precio           | Numero Decimal   | Obligatorio |

## Entity: PEDIDO

| Atributo         | Tipo             | Notas       |
|------------------|--------------------------------|
| id_pedido        | Numero Entero    | [PK]        |
| id_cliente       | Numero Entero    | Obligatorio |
| id_producto      | Numero Entero    | Obligatorio |
| cantidad         | Numero Entero    | Obligatorio |

# Relaciones
Un CLIENTE puede tener muchos pedidos pero un pedido le pertenece a un solo CLIENTE
Un PEDIDO puede tener varios productos
Un PRODUCTO puede aparecer en varios pedidos 
