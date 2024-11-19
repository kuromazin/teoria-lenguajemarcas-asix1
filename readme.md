# ASIX1-Apuntes del curso (GITHUB,MARKDOWN,HTML,CSS Y RESPONSIVE)
## INDICE DE LOS APUNTES
1. [GITHUB](#1-github "Enlace al apartado de GitHub")
2. [MARKDOWN](#2-markdown "Enlace al apartado de MarkDown")
3. [HTML](#3-html "Enlace al apartado de HTML")
4. [CSS](#4-css "Enlace al apartado de CSS")
5. [RESPONSIVE](#5-diseño-responsive "Enlace al apartado de  Diseño Responsive")
### 1. GITHUB
#### 1.1 Instalacion de GITHUB
Aqui esta el link de instalacion de la herramienta.
* [https://git-scm.com](https://git-scm.com)
#### 1.2 Creacion Cuenta Github
1. Iremo a [GitHub](https://github.com/ "enlace a GitHub").
2. Dale click a "Sign up" .
3. Pon un nombre de usuario, correo y una contraseña segura.
4. Y ya estaria la cuenta lista.
#### 1.3 Repositorios
Dentro de los repositorios podemos hacer varias cosas como crearlos, clonarlos etc todo eso mediante los siguientes comandos:
 - ```git init```. Inicializa un repositorio Git en el dispositivo.
 - ```git branch```. Muestra las ramas del repositorio.
 - ```git add "archivo.txt"```. Añadimos archivos al repositorio.
 - ```git commit -m "Mensaje del commit"```. Haces un commit.
 - ```git push origin main```. Envias el commit.
 - ```git remote add origin https://github.com/usuario/repo.git```. Clona el repositorio de github al dispositivo local.
### 2. MARKDOWN
Markdown sirve para darle formato al texto. Es fácil y queda bonito dentro de lo que cabe.
#### 2.1 Titulillos
Si quieres organizar el texto en niveles, usa almohadillas "(#)"
```
# Titulo 
## Subtitulo
### Subsubtitulo
```
#### 2.2 Negrita
Es bastante simple usaremos los asteriscos "(*)"
```
**texto de ejemplo**
```
#### 2.3 Cursiva
Igual de simple pero usando guiones bajos "(_)"
```	
_texto de ejemplo_
```
#### 2.4 Listas
Para hacer listas es como si fuera un texto enriquecido pones el numero y ya tienes la lista.
#### 2.5 Mostrar Codigo
Para mostrar el codigo usaremos este simbolito "(```)"
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```
#### 2.6 Enlaces
Para colar enlaces en el documento de markdown hay que hacer lo siguiente:
```
[Mi Github](https://github.com/kuromazin/ASIX1-AprendizajeMarkdown1 "Titulo Random " )
```
#### 2.7 Imagenes
Hay que tener la imagen metido dentro del repositorio 
```
![Hora de Bailar](https://github.com/kuromazin/teoria-lenguajemarcas-asix1/blob/main/img/gif%20feo.gif)
```
![Hora de Bailar](https://github.com/kuromazin/teoria-lenguajemarcas-asix1/blob/main/img/gif%20feo.gif)
#### 2.8 Tablas
Para hacer las tablas hay que seguir la siguiente estructura:
```
| Título 1 | Título 2 |
|----------|----------|
| Fila 1   | Dato 1   |
| Fila 2   | Dato 2   |
```
### 3.HTML
### 3.1 Estructura Base
````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
````
### 3.2 Etiquetas utiles
#### Titulos
Como en markdown tenemos diferentes tipos de titulos algunos ejemplos de ellos:
```
<h1>Encabezado grande</h1>
<h2>Encabezado mediano</h2>
```
#### Parrafos
Para los parrafos usaremos el
```
 '(<p></p>)'
```
#### Enlaces y imagenes
Para enlaces y imagenes usaremos las siguientes estructuras:
```
<a href="https://github.com/kuromazin/teoria-lenguajemarcas-asix1?tab=readme-ov-file#2-markdown">Los apuntes mas simples y claros</a>
```
```
<img src="ejemplo.png" alt="ejemplo" width="100" height="100">
```
#### Listas
Hay 2 tipos de listas:
Enumerada:
```
<ol>
    <li>Elemento 1</li>
    <li>Elemento 2</li>
</ol>
```
Por viñetas:
```
<ol>
    <li>Elemento 1</li>
    <li>Elemento 2</li>
</ol>
```
#### Formulario Etiquetas NECESARIAS
```<form>```: Define un formulario.

    action: URL destino de los datos.

    method: Método HTTP (GET o POST).

```<input>```: Recibe datos del usuario.

    type: Tipo de entrada (text, password, radio, checkbox, submit).

    placeholder: Texto informativo.

```<textarea>```: Área de texto multilínea.

    rows: Filas visibles.

    cols: Columnas visibles.

    placeholder: Texto informativo.

```<select>```: Contenedor de un menú desplegable.

```<option>```: Opción del menú.

    disabled: Deshabilitar opción.

```<fieldset>```: Agrupa elementos relacionados en un formulario.

```<legend>```: Proporciona un título para el grupo.

```<button>```: Botón interactivo para acciones (e.g., enviar formulario).
#### Ejemplo funcional de un formulario
```
 <form action="recepcion.php" method="GET">
        <br>
        <label for="nombre">Suo Nombre:</label>
        <br>
        <input type="text" id="nombre" name="nombre" placeholder="Introduce suo nombre">
        <br>
        <br>
        <label for="password">Sua Contraseña:</label>
        <br>
        <input type="password" id="password" name="password" placeholder="Introduce sua contraseña">
        <br>
        <fieldset>
            <legend>Idioma:</legend>
            <label for="Castellano">Castellano:</label>
            <input type="radio" name="idioma" value="Castellano">
            <br>
            <label for="Catalan">Catalan:</label>
            <input type="radio" name="idioma" value="Catalan">
            <br>
            <label for="Chino">Chino:</label>
            <input type="radio" name="idioma" value="Chino">
            <br>
            <label for="Haitiano">Haitiano</label>
            <input type="radio" name="idioma" value="Haitiano">
        </fieldset>
        <br>
        <fieldset>
            <legend>Nacionalidad</legend>
            <label for="argelino">Argelina:</label>
            <input type="checkbox" name="Nacionalidad" value="argelino" id="argelino">
            <br>
            <label for="Francesa">Francesa:</label>
            <input type="checkbox" name="Nacionalidad" value="Francesa" id="Francesa">
            <br>
            <label for="Mena">Mena:</label>
            <input type="checkbox" name="Nacionalidad" value="Mena" id="Mena">
            <br>
        </fieldset>
        <br>
        <label for="observaciones">Observasoes</label>
        <br>
       <textarea name="observaciones" id="observaciones" cols="80" rows="4" placeholder="Introduce suo comentario dua pagina web"></textarea>
        <br>
        <label for="ciudad">Ciudad:</label>
        <select name="ciudad" id="ciudad">
            <option value="" disabled>Selecciona sua ciudad</option>
            <option value="Barcelona"> Barcelona</option>
            <option value="Madrid">Madrid</option>
            <option value="Valencia">Valencia</option>
            <option value="Sevilla">Sevilla</option>
            <option value="Murcia">Murcia</option>
        </select>
        <br>
        <br>
        <button type="submit"> Envia suo dato</button>
```
### 4.CSS
### 5.RESPONSIVE