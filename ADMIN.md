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
Para crear, editar o borrar los menús del sitio web, se debe dirigir a la pesataña de Aperiencia >> Menús del panel principal de la administración de wordpress
![](https://xpc.com.ec/guides-images/a28.png)
![](https://xpc.com.ec/guides-images/a29.png)

## Woocomerce
Woocommerce es el servicio que utiliza Wordpress para tienda en línea. Woocommerce permite la administración tanto de **productos** como de **pedidos**.
![](https://xpc.com.ec/guides-images/a8.png)

### Pedidos
![](https://xpc.com.ec/guides-images/a9.png)

> Permite administrar los pedidos desde la página web, permitiendo las siguientes configuraciones.

### Estado del pedido
> ![](https://xpc.com.ec/guides-images/a10.png)
> ![](https://xpc.com.ec/guides-images/a31.png)

> - ** ¡IMPORTANTE! Esta opción es proporcionada por la pasarela de pagos Paymentez y permite devolución del dinero de una compra siempre y cuando esta se pague usando este servicio, para hacerlo, se debe ingresar el código de la transacción proporcionado en laparte inferior de este cuadro **
> ![](https://xpc.com.ec/guides-images/a11.png)
> ![](https://xpc.com.ec/guides-images/a12.png)
> ![](https://xpc.com.ec/guides-images/a13.png)

### Productos
En cuanto a los productos, la administración de estos viene directamente desde la base de datos administrada por XPC, por lo que no habría mayor información fuera de la requerida para subir imágenes en nuevos productos.

> ![](https://xpc.com.ec/guides-images/a14.png)

> El tamaño de la imagen debe ser de 500X500 px

> Para subir una o más fotos de un producto debes acceder a esta opción, ubicada en la parte inferior derecha de la página de edición de productos

> ![](https://xpc.com.ec/guides-images/a15.png)

# Importar / Exportar Información
### Importar productos, usuarios, tracking

> #### Productos

> **Primero**.- Hacer un select en la base de datos SQL Server y guardar el resultado en formato **CSV**
> ![](https://xpc.com.ec/guides-images/a32.png)

> **Luego**, en nuestra adminisración de **wordpress** nos dirigimos a la sección productos y seleccionamos la opción de importar
> ![](https://xpc.com.ec/guides-images/a33.png)

> Subimos el archivo **CSV** generado anteriormente
> ![](https://xpc.com.ec/guides-images/a34.png)
> ![](https://xpc.com.ec/guides-images/a35.png)
> Verificar que los campos esten correctamente enlazados, en caso de que no, hacer la selección
> ![](https://xpc.com.ec/guides-images/a36.png)

> Ejecutar la importación
> ![](https://xpc.com.ec/guides-images/a37.png)
> ![](https://xpc.com.ec/guides-images/a38.png)
> ![](https://xpc.com.ec/guides-images/a39.png)

> #### Usuarios

> Al igual que anteriormente realizamos un Select en la BDD SQL Server y generamos el **CSV**
> ![](https://xpc.com.ec/guides-images/a40.png)
> ![](https://xpc.com.ec/guides-images/a41.png)
> ![](https://xpc.com.ec/guides-images/a42.png)
> ![](https://xpc.com.ec/guides-images/a43.png)
> ***NOTA**.- Se realiza el mismo proceso que anteriormente con los productos*

> ### Tracking
> **IMPORTANTE**.- Para **todos** los procesos de IMPORTACIÓN y EXPORTACIÓN de información para el módulo externo de tracking (Mostrar listado de tracking en servientrega y solicitudes de garantías) debemos ingresar al **CPANEL** (xpc.com.ec/cpanel), las credenciales se especifican en el apartado de CPanel.
> Al igual que anteriormente realizamos un Select en la BDD SQL Server y generamos el **CSV** 
> ![](https://xpc.com.ec/guides-images/a44.png)
> En este caso, por tratarse del módulo externo a wordpress, la subida se realizará vía SQL, por lo que se debe utilizar alguna herramienta para convertir de **CSV a SQL**, o a su vez, si su herramienta de SQL Management lo permite, exportar en formato SQL los resultados.
> Acontinuación hacemos el ejemplo de conversión de CSV a SQL usando la herramienta http://www.convertcsv.com/csv-to-sql.htm
> Importamos el archivo CSV
> ![](https://xpc.com.ec/guides-images/a45.png)

> Ingresamos los campos con los que queremos que se genera nuestro SQL 
> ![](https://xpc.com.ec/guides-images/a45b.png)

> Seleccionamos la acción SQL a la que queremos que se convierta nuestro CSV, en este caso **CSV a INSERT**
> ![](https://xpc.com.ec/guides-images/a45a.png)

> Lo siguiente es ejecutar el SQL en la base datos MySql con la que funciona el sitio web en la tabla **Servicio Técnico**
> ![](https://xpc.com.ec/guides-images/a46.png)
> ![](https://xpc.com.ec/guides-images/a47.png)

### Exportar Pedidos y Solicitudes de garantías

> ### Pedidos

> Primero debemos extraer los datos de la herramienta de administración de **Wordpress**, para lo cual nos dirigimos a *WooCommerce >> Extraer pedidos* y ejecutamo, esto nos imprimirá un archivo CSV el cual, usando la herramienta anterior (http://www.convertcsv.com/csv-to-sql.htm) debe ser convertido a SQL para luego ser ejecutado en el administrador de **SQL Server**

> Los campos deben estar seleccionados tal como en la imagen y luego clickear en el campo de **EXPORTAR** en la parte inferior de la pantalla.

> ![](https://xpc.com.ec/guides-images/a48.png)
> ![](https://xpc.com.ec/guides-images/a45.png)
> ![](https://xpc.com.ec/guides-images/a49.png)
> ***NOTA**.- El Sql debe ser ejecutado en la tabla **VENTAS_WEB** y el sistema, de forma automática, usando los disparadores creados con anticipación realizará la inserción en las tablas del sistema en los formatos internos de XPC*

> ### Solicitudes de garantías
> A diferecnia del caso anterior, para las solicitudes de garantías debemos ingresar por cPanel a la BDD del sitio web y extraer los datos en formato SQL de la tabla **GARANTIASWEB** y ejecutarlo en el administrador de **SQL Server**
> ![](https://xpc.com.ec/guides-images/a50.png)
> ![](https://xpc.com.ec/guides-images/a51.png)
> ![](https://xpc.com.ec/guides-images/a52.png)
> ***NOTA**.- El Sql debe ser ejecutado en la tabla **GARANTIASWEB** y el sistema, de forma automática, usando los disparadores creados con anticipación realizará la inserción en las tablas del sistema en los formatos internos de XPC*



#### Importante
> Los procesos de manipulación de base de datos que usamos para el desarrollo del sitio web son los predeterminados de Wordpress, con el plugin de administración de tienda WooCommerce, existen muchas otras maneras de hacerlo y esto depende de cada desarrollador y/o administrador del sitio web. En casos de manipulación, migraciones o actualizaciones de estas, pero nosotros recomendamos usar las predeterminadas de wordpress.

# Chat en línea
> Para que el chat en línea funcione en el sitio web, se ingresó vía **Javascript** en la cabecera, ya que este servicio es externo y funciona con sus propios recursos
> ![](https://xpc.com.ec/guides-images/a53.png)
> ![](https://xpc.com.ec/guides-images/a54.png)
> ![](https://xpc.com.ec/guides-images/a55.png)
> *Javascript del chat:*

`<!-- BEGIN JIVOSITE CODE -->`
`<script type='text/javascript'>`
`(function(){ var widget_id = 'rbp2M7kSme';var d=document;var w=window;function l(){ var s = document.createElement('script'); s.type = 'text/javascript'; s.async = true; s.src = '//code.jivosite.com/script/widget/'+widget_id; var ss = document.getElementsByTagName('script')[0]; ss.parentNode.insertBefore(s, ss);}if(d.readyState=='complete'){l();}else{if(w.attachEvent){w.attachEvent('onload',l);}else{w.addEventListener('load',l,false);}}})();`
`</script>`
`<!-- END JIVOSITE CODE -->`

> Para acceder al perfil de usuario, para lo cual nos dirigimos al siguiente link https://app.jivosite.com/ con las credenciales

> info@xpc.com.ec
> XPC2018 (XPC con mayúsculas)

> Al momento de ingresar, por favor, les pedimos manejarse solamente en estos dos espacios, los otros botones que están en la parte inferior son de configuración y si se habilita o deshabilita algo, podría causarnos problemas en el chat. Cualquier inquietud sobre el chat, estamos a las órdenes.
> ![](https://xpc.com.ec/guides-images/a56.png)

> **IMPORTANTE!** En línea podrá estar una sola persona a la vez, para lo cual, si desean ingresar, deberán pedir al vendedor que esté conectado cerrar la sesión para que la otra persona pueda ingresar. 
> Desde la APP Store y Play Store pueden descargarse la aplicación de Jivochat para que puedan ingresar con su celular.

# Módulo Garantías
> Para ingresar debemos dirigirnos al link (https://xpc.com.ec/tracking/login-admin-garantias.php), al cual podemos acceder también desde el sitio xpc.com.ec/traking, en el botón de administración del lado superior derecho
> ![](https://xpc.com.ec/guides-images/a57.png)

> En donde debemos ingresar la llave de acceso:
`*_o5XF9qXPC`

> Dentro se desplegaran las solicitudes pendientes, a las que, accediendo se nos desplegarán los detalles de la solicitud con las opciones de aceptar o rechazar.
> ![](https://xpc.com.ec/guides-images/a58.png)
> ![](https://xpc.com.ec/guides-images/a59.png)
> ![](https://xpc.com.ec/guides-images/a60.png)


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

# Namecheap
## Proveedor de servidor

> **Ingresar**.- Se adjuntan credenciales:

> Link de acceso: namecheap.com

> Usuario: XpcEcuador

> Contraseña: Xpc2018*

> ![](https://xpc.com.ec/guides-images/a17.png)

