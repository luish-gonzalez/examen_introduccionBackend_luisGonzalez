# Documentación

## Diseño

Las tablas se estructuraron según los requerimientos y las entidades que pertenecen, asignando cada uno de los atributos que le corresponden. Estas fueron:

1. Cliente
2. Pedido
3. Transacción
4. Pedido_libro
5. Libro
6. Autor_libro
7. Autor

Donde se relaciona, cliente con pedido, pedido con transacción y pedido_libro, pedido_libro con libro, libro con autor_libro, y autor_libro con autor.

## Restricciones y validaciones

### Claves

Tabla:

1. Cliente: Primaria -> id_cliente
2. Autor: Primaria -> id_autor
3. Pedido: 
   - Primaria: id_pedido, 
   - Foranea: id_cliente_fk, stock_fk
4. Pedido_libro: Primaria y foranea: id_pedido_fk, id_libro_fk
5. Libro: Primaria: is_libro
6. Autor_libro: Primaria y foranea: id_autor_fk, id_libro_fk
7. Autor: Primaria: id_autor

