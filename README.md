# Manual de usuario

## Deployment

Este manual de usuario es una página web estática muy sencilla que puede ser
hosteada fácilmente utilizando cualquier servidor HTTP popular. Como ejemplo
utilizaremos el módulo `http.server` que nos proporciona python.

```
# En una terminal, situados en la raiz del 
# repositorio, ejecutamos el siguiente comando:
$ python3 -m http.server 8000
```

Debería ser capaz de acceder al manual introduciendo la dirección
`localhost:8000` en su navegador web favorito.

Adicionalmente, la página web se encuentra hosteada de manera temporal en la
dirección `https://p56289.github.io`.

## Estructura

La estructura de la pagina web es la siguiente:

```
.
├── css
│   ├── seccion.css
│   └── style.css
├── en
│   ├── index.html
│   ├── correo-electronico.html
│   ├── enviar-mensajes.html
│   └── ...
├── es
│   ├── index.html
│   ├── correo-electronico.html
│   ├── enviar-mensajes.html
│   └── ...
├── img
│   ├── contraseña-de-aplicacion.png
│   ├── creacion-contraseña-dos.png
│   └── ...
├── docs
│   ├── manual_usuario_español.pdf
│   └── manual_usuario_ingles.pdf
├── favicon.ico
├── index.html
└── README.md
```

En la carpeta `es` se almacenan todas las páginas y secciones escritas en
castellano y  mientras que en la carpeta `en` se almacenan sus traducciones al
inglés. De esta forma se puede alternar entre los diferentes lenguajes
fácilmente. Por ejemplo: `es/index.html` y `en/index.html`.

Los estilos de almacenan en la carpeta `css` y las imágenes en la carpeta `img`.

El manual está dividido en 7 secciones diferentes, cada una contenida dentro de
su propio HTML. Todas estas secciones tienen un estilo común definido en el
archivo `css/style.css`. Las secciones son las siguientes:

1. Sistema login
2. Interfaz Telnet
3. Gestion de clientes
4. Correo electrónico
5. Enviar mensajes
6. Recepción de correo electrónicos
