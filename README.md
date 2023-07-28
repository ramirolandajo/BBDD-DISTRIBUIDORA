<h1>TPO INGENIERÍA DE DATOS I</h1>
</img src="">
<h2>Profesores: Charles Maldonado; Gustavo Escandell</h2>

<p>Roles:</p>
<ul>
  <li>PM = Ivo Bandoni (Representante)</li>
  <li>Analista Funcional = Mateo Rosello</li>
  <li>Arquitecto de Soluciones = Julian Serrano</li>
  <li>Desarrollador 1 = Ramiro Landajo</li>
  <li>Desarrollador 2 = Valentin Quiroga</li>
</ul>

<h2>Sistema: Sistema de gestión de una distribuidora</h2>

<h3>Objetivo</h3>
<p>
  El objetivo del sistema es una base de datos que permita al cliente tener un registro completo de todos los productos en su inventario, 
  gestionar y actualizar los precios de los productos, gestionar el stock de los productos, gestionar y actualizar sus clientes, 
  llevar un registro de los proveedores con los que trabaja, y por último registrar y gestionar la logística de la mercadería hasta sus
  clientes.
</p>

<h3>Límite</h3>
<p>
El límite del sistema va desde la gestión del stock de los productos y pedidos (junto con los clientes), hasta la gestión de la logística de los envíos de los pedidos.
</p>
 
<h3>Alcance</h3>
<p>
Registro y gestión de productos, pedidos, gestión de empleados, crear y gestionar envíos, registrar y gestionar clientes. 
</p>

<h3>Problemas potenciales de una distribuidora</h3>
<ul>
  <li>Problemas de control de inventario</li>
  <li>Problemas de rastreo de pedidos</li>
  <li>Barreras de comunicación</li>
  <li>DDeslices en los precios de los productos/li>
</ul>

<h3>Historia de usuario</h3>
<p>Queremos armar un modelo de base de datos para mejorar la gestión de una distribuidora. El cliente, propietario de una distribuidora local, se enfrenta a desafíos importantes que afectan la eficiencia y la rentabilidad de su negocio. <br><br>
Los problemas más graves de este casos son el desequilibrio en el mantenimiento de stock y los constantes aumentos de precios. Teniendo en cuenta la importancia de abordar estas dificultades, el cliente decide implementar un modelado de base de datos. <br><br>
El cliente se imagina una solución en la que pueda tener un registro completo de todos los productos en su inventario. Quiere saber en todo momento cuántos productos tiene, cuántos ha vendido y cuántos necesita reponer. Además, comprende que el mantenimiento adecuado del stock es crucial para su negocio, evitando la escasez de productos o el exceso de inventario. <br><br>
Otro desafío al que se enfrenta el cliente es la constante fluctuación de precios en el mercado. Para mantener su rentabilidad, necesita tener un control adecuado sobre los precios de venta de sus productos. Desea poder ingresar y actualizar fácilmente los precios. <br><br>
Por otro lado, el cliente desea llevar el control de la logística de su mercadería, es decir, quiere tener registrado que chofer hizo tal entrega ,las ciudades de origen y de destino y las fechas en las que tardó en hacerse el envío. <br><br>
</p>

<h3>Tablas:</h3>
<ul>
  <li>Producto</li>
  <li>Proveedor</li>
  <li>Empleado</li>
  <li>Cliente/li>
  <li>Pedido</li>
  <li>Detalle Pedido</li>
  <li>Depósito</li>
  <li>Vehículo/li>
</ul>
<h3>Universo del discurso </h3>
<p>
  Se solicita crear un modelado de base de datos para que el cliente pueda mejorar la gestión de su distribuidora.
  Los principales problemas a tener en cuenta son el control cotidiano de stock, seguimiento de pedidos y la actualización constante de los precios. Además de esto se desea llevar un registro de los empleados de la distribuidora, los proveedores con los que trabaja y depósitos que maneja entre otras cosas. <br><br>
  Con respecto a los productos se conocen los siguientes datos: el código del producto, el nombre, la categoría a la que pertenece, su marca, el precio del producto, el stock y el depósito en el cual está almacenado. <br><br>
  Por otro lado también se necesita registrar a los proveedores de la distribuidora, la información necesaria es el cuit que tiene cada proveedor, también se debe guardar el nombre del proveedor, el código del producto que provee y la provincia del mismo. <br><br>
  También se desea llevar un registro de los empleados de la distribuidora en cuestión, se solicita tener el CUIT de cada empleado, su nombre, fecha de nacimiento, su cargo/puesto, su dirección y salario. <br><br>
  De los clientes se conoce su DNI correspondiente, su nombre, membresía y fecha de nacimiento. <br><br>
  Teniendo en cuenta las funciones de una distribuidora también se solicita guardar la información de los envíos realizados, de cada envío se tiene que registrar: 
  el ID del envío, un código para que los clientes puedan identificar el envío de su pedido, el CUIT del empleado a cargo (que sería el chofer), ID del vehículo, ID del pedido que lleva y  fecha en el que se realizó el envío. <br><br>
  Cada cliente de la distribuidora realiza pedidos, cada pedido se tiene que registrar un código que es asignado y  es inequívoco, tiene el CUIT del cliente, la fecha en la que se creó el pedido y por último el valor total de ese pedido. <br><br>
  Para cada pedido, están asociados mínimo 1 o varios detalles de pedidos, ya que un cliente puede comprar distintos productos en distintas cantidades en un mismo pedido. De cada detalle de pedido se conoce el ID que lo identifica, el ID del pedido al que hace referencia, el producto comprado, y la cantidad comprada de ese producto. <br><br>
  Los productos de la distribuidora se deben guardar en depósitos el cual tienen un ID inequívoco, nombre del depósito, la provincia de ese depósito y con una capacidad de productos que entran. <br><br>
  Se debe tener registrado los vehículos de transporte de la empresa, con un ID de vehículo, el tipo de vehículo y su capacidad correspondiente.
</p>

<h3>Modelo-Entidad-Relación(MER)</h3>
</img src="">

<h3>Diagrama-Entidad-Relación(DER)</h3>
</img src="">


