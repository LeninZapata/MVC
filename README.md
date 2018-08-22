# MVC
MVC (Modelo Vista Controlador) en español, facil y codigo documentado.

### Descripcion
Despues de estudiar mucho sobre modelos vista controlador en PHP, pude realizar uno de manera facil y que sea escalable y entendible. De esta forma podrá realizar sus sistemas basado en MVC con un plantilla excelente y responsive.

### Objetivo
Este modelo esta probado ya que he realizado un sistema mediano (con varios modulos) basado en este framework limpio que realice para poder adaptarlo y crear facilmente. Es muy facil la estructura, tratare de explicarlo para su facil uso y aplicación.

### ¿Como funciona?
##### Estructura
```
mvc-base
├── sistema
│   ├── Controladores
│   │   ├── Inicio.php
│   ├── Librerias
│   │   └── Products.php
│   └── views
│       └── products
│           └── index.phtml
└── publico
    └── index.php
```
**mvc-base:** Nombre de carpeta del proyecto, le puedes cambiar de nombre por lo general si usas _Wampserver_ pondrias dentro de la carpeta _www_ es decir quedaria asi: `www/mvc-base` pero como te comente el nombre _mvc-base_ es el nombre de la carpeta de tu proyecto, podria quedar asi `www/mi-proyecto` y si usas _Xamp_ quedaria asi `htdocs/mi-proyecto`.

**-sistema:** Esta carpeta va contener todos los archivos para hacer funcionar el sistema, en otros framework MVC suele estar con el nombre de _system_ ó _app_ en este caso se llama _sistema_ porque este es un framework creado en español.

**--Controladores:** Cada archivo es un controlador, y dentro de este archivo lo que habrá es un Clase que llamara al metodo del controlador, es decir la accion de este controlador. Si no accion pues todo controlador debe tener almenos el metodo _index_ ya que este sera por defecto. Más adelante se explicara como se ejecuta estos metodos ó acciones por archivo controlador.

**---Inicio.php:*** Este es el primer controlador base, es decir lo puse para poder hacer el ejemplo y para cuando ejecutes el sistema no tengas problemas, le puse este nombre porque practicamente aquí iria todas las acciones (metodos) que haras en la pantalla de inicio de tu sistema.

**--Librerias:** Van todos los archivos extras que necesites para que tu sistema o en este caso el MVC funcione bien, dentro de esa carpeta agregé un archivo llamado _Utilidades.php_ que es una clase donde tiene metodos estaticos que sirven para ser llamados en cualquier parte del sistema.

Aqui podras agregar mas metodos que te ayuden a resolver el problema de tu sistema. Tambien he agregado la libreria de [EZsql](https://github.com/ezSQL/ezSQL) que nos servira para la conexion a base de datos. Esta libreria es muy facil usar para manipulacion de datos en _mysql_ es tan buena y sencilla que esta es la libreria que usa [Wordpress](https://wordpress.org/) dentro de su nucleo para operar!, imaginate que tan buena y confiable es.

**--Modelos:** 



### Funcionamiento `index.php`
Todo comienza del archivo `index.php` donde se declara constante del sistema basica como: Version, Url publica, Ruta del sistema, Carpeta Base del sistema. Si todo esta entendible hasta aquí, continuemos...
![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)
