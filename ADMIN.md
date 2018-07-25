# MANUAL DE ADMINISTRACIÓN DE LA PÁGINA WEB XPC

![](https://xpc.com.ec/guides-images/2.png)
------

# Introducción
En este manual daremos los conceptos de administración correspondientes al comercio electrónico de Xpc (xpc.com.ec). Es importante recalcar que este manual es válido para las dos versiones del sitio (Cliente finales: **xpc.com.ec** && **xpc.com.ec/app/distribuidor**).

## Ingresar
Para ingresar al módulo de administración de wordpress, debemos dirigirnos a: **xpc.com.ec/wp-admin** && **xpc.com.ec/app/distribuidor/wp-admin** para cada versión respectivamente, en la que se debe ingresar las siguientes credenciales:

- **Usuario:** administrador
- **Contraseña:** xpc2018

![](https://xpc.com.ec/guides-images/a1.png)

> Válidas para ambas versiones

## Visión general
El módulo de administración de worspress nos ofrece todas las opciones de configuración y diseño de nuestro sitio web, y, combinado con el plugin de comercio electrónico WooCommerce, el sitio adquiere la funcionalidad de tienda en línea.

A continuación una foto del panel de administración de wordpress:

![](https://xpc.com.ec/guides-images/a2.png)

## Enlances importantes
En la parte lateral del panel de administración encontramos los menús correspondientes a todos los parámetros de administración del sitio web. En este manual sólo haremos referencia a los más importantes y de manejo cotidiano, ya que, los demás se entregan configurados y listos para usar al momento de entregar este manual.

> ![](https://xpc.com.ec/guides-images/a3.png)

### Páginas 
Contiene todas las páginas configuradas para el sitio web así también como las opciones crear, modificar y borrar cualquiera de ellas, como ya se especificó, todas están pre-configuradas así que no hay mayor explicación en este parámetro.
![](https://xpc.com.ec/guides-images/a4.png)

### Contacto
Contiene todos los formularios y solicitudes de la página (*Fuera del módulo de RMA*).
![](https://xpc.com.ec/guides-images/a5.png)
![](https://xpc.com.ec/guides-images/a6.png)
![](https://xpc.com.ec/guides-images/a7.png)

### Menús
----------------------------------------------

## Woocomerce
Woocommerce es el servicio que utiliza Wordpress para tienda en línea. Woocommerce permite la administración tanto de **productos** como de **pedidos**.
![](https://xpc.com.ec/guides-images/a8.png)

### Pedidos
![](https://xpc.com.ec/guides-images/a9.png)

> Permite administrar los pedidos desde la página web, permitiendo las siguientes configuraciones.

> - ** Modificar estados **
> ![](https://xpc.com.ec/guides-images/a10.png)

> - ** ¡IMPORTANTE! Esta opción es proporcionada por la pasarela de pagos Paymentez y permite devolución del dinero de una compra siempre y cuando esta se pague usando este servicio, para hacerlo, se debe ingresar el código de la transacción proporcionado en laparte inferior de este cuadro **
> ![](https://xpc.com.ec/guides-images/a11.png)
> ![](https://xpc.com.ec/guides-images/a12.png)
> ![](https://xpc.com.ec/guides-images/a13.png)

### Productos
En cuanto a los productos, la administración de estos viene directamente desde la base de datos administrada por XPC, por lo que no habría mayor información fuera de la requerida para subir imágenes en nuevos productos.

> ![](https://xpc.com.ec/guides-images/a14.png)

> Para subir una o más fotos de un producto debes acceder a esta opción, ubicada en la parte inferior derecha de la página de edición de productos

> ![](https://xpc.com.ec/guides-images/a15.png)

### Como subir CSV

# cPanel 
## Detalles técnicos generales

> A continuación se detallan los conceptos fundamentales para la adminsitración del hosting.

> **Ingresar**.- Se adjuntan las credenciales:

> Link de ingreso: xpc.com.ec/cpanel

> Usuario: xpccczfq

> Contraseña: yYBmbnyx1Her

> ![](https://xpc.com.ec/guides-images/a16.png)

## Archivos

> Para acceder a los archivos almacenados en el servidor debe dirigirse a la opción de Files >> File Manage

> ![](https://xpc.com.ec/guides-images/a18.png)

> ![](https://xpc.com.ec/guides-images/a19.png)

> Una vez dentro, debe ingresar al directorio public_html, en donde encontraremos todos los archivos de configuración, forntend y backend de Wordpress.

> ![](https://xpc.com.ec/guides-images/a20.png)

**IMPORTANTE**

> Debe tomar encuenta que las versiones de Cliente y Administrador trabajan con su propia instalación de wordpress, al ingresar al directorio especificado anteriormente está accediendo a la versión de cliente final, para acceder a la versión de **distribuidores** debe dirigirse, en el mismo directorio de cliente final a la carpeta *app/distribuidor*

> ![](https://xpc.com.ec/guides-images/a21.png)

> ![](https://xpc.com.ec/guides-images/a22.png)

> ![](https://xpc.com.ec/guides-images/a23.png)

## BDD

> Para ingresar a las base de datos con las que funciona el sitio web debemos dirigirnos al apartado de *Databases >> phpMyAdmin* 

> ![](https://xpc.com.ec/guides-images/a24.png)

> ![](https://xpc.com.ec/guides-images/a25.png)

> Una vez dentro, encontraremos dos bases de datos registradas:
> - xpccczfq_wordpress (Bdd para la instalación de wordpress de la versión de *Clientes finales*)
> - xpccczfq_wordpress-distribuidor (Bdd para la instalación de wordpress de la versión de *Distribuidores* )

> ![](https://xpc.com.ec/guides-images/a26.png)

> **Especificaciones:**

> - Las tablas que comiencen con los prefijos *wpk6* hacen referencia a los datos que alamcena **Wordpress** para el funcionamiento general del sitio web.

> - Las tablas que comiencen con los prefijos *wpk6-woocommerce* hacen referencia a los datos que almacena **WooCommerce**, es decir, de la tienda en línea.

> - Las tablas que no tengan ningun prefijo son las tablas con las que funciona el **módulo** adicional de RMA.

> ![](https://xpc.com.ec/guides-images/a27.png)

### Especificiaciones de las tablas (Servicios Técnico y Garantias)

### Procesos
> Los procesos de manipulación de base de datos que usamos para el desarrollo del sitio web son los predeterminados de Wordpress, con el plugin de administración de tienda WooCommerce, existen muchas otras maneras de hacerlo y esto depende de cada desarrollador y/o administrador del sitio web. En casos de manipulación, migraciones o actualizaciones de estas, pero nosotros recomendamos usar las predeterminadas de wordpress.

# Namecheap
## Proveedor de servidor

> **Ingresar**.- Se adjuntan credenciales:

> Link de acceso: namecheap.com

> Usuario: XpcEcuador

> Contraseña: Xpc2018*

> ![](https://xpc.com.ec/guides-images/a17.png)

### CHAT
