---
{"dg-publish":true,"permalink":"/synapse/"}
---

Más en específico, SYNAPSE manda la siguiente información mediante CDL. La información se manda de forma diaria a día vencido:

* VENTAS DIARIAS (TXSTA, TXTA, estándar): ID_PRODUCTO, FECHA_VENTA, MONTO_VENTA, UNIDADES VENDIDAS
* TRANSFERENCIA DIARIA (TXSTA, TXTA, estándar): ID_PRODUCTO, FECHA_TRANSFERENCIA, MONTO TRANSFERENCIA, UNIDADES TRRANSFEREIDAS
* PRODUCTOS (CLPR, estándar): ID PRODUCTO, NOMBRE PRODUCTO, FECHA EFECTIVA
* MERMA (TXSTA, TXTA, estándar*)*:
* PRECIO PRODUCTOS (PRDPR, personalizado): SUCURSAL, PRECIO, ID_PRODUCTO.

### Event type
* VENTA DIARIA
* TRANSFERENCIA DIARIA
* PRODUCCION DIARIA
* MERMA