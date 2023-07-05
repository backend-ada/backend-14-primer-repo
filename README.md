# ¿Qué es GIT?

GIT es un sistema de control de versiones distribuido, libre y de código abierto, diseñado para manejar desde pequeños hasta enormes proyectos con eficiencia y velocidad.

- WINDOWS --> Necesario instalar desde la web oficial: https://git-scm.com/.
- LINUX|MAC --> Instalado por defecto.

## Comandos básicos

- **git init**                  --> Crea un repositorio de GIT vacío.
- **git clone <path>**          --> Clona un repositorio dentro del directorio desde el cual se invoca.
- **git add <files>**           --> Agrega los archivos especificados al índice y prepara para hacer commit. Reemplazando <files> con un "." agregamos todos los archivos que están en el árbol del proyecto (que estén excluídos del arhivo .gitignore).
- **git status**                --> Muestra el estado del árbol del proyecto.
- **git commit -m "<msg>"**     --> Crea un nuevo commit con un mensaje descriptivo. Dicho de otra forma, guarda los cambios en el repositorio y le asigna un mensaje descriptivo a ese nuevo punto en nuestro historial de versiones.
- **git checkout**              --> Acceder a un punto en específico del historial de versiones.
- **git switch -**              --> Acceder al punto anterior al actual. Es decir, si con checkout fui a cierto punto, con este comando vuelvo a dónde estaba.
- **git log**                   --> Ver todo el historial de commits.
- **git push**                  --> Actualizar el repositorio remoto con todos los cambios locales.

# ¿Qué es GitHub?

GitHub es una plataforma que ofrece un servicio basado en la nube para el desarrollo de software y su control de versiones mediante el uso de GIT, permitiendo a los desarrolladores almacenar y administrar su código. Provee el sistema de control de versiones distribuido de GIT con algunas herramientas muy poderosas que vamos a ir viendo con el paso de la carrera.

# Instrucciones

## ¿Cómo configurar las llaves SSH?

Para poder subir y administrar los repositorios de GIT en la nube de GitHub, necesitamos realizar una configuración básica de seguridad que nos permita el acceso privado a nuestra cuenta de GitHub.
Para esto, tenemos que realizar los siguientes pasos:

- Crear un par de llaves SSH pública/privada de forma local:

    1. Abrir la terminal del sistema operativo que estén usando y ejecutar el comando *ssh-keygen -t rsa*.
    2. Desde la terminal, ir a la carpeta donde se acaban de generar el par de llaves con el comando cd <ruta>.
    3. Con el comando *cat* imprimir en la terminal el contenido de *id_rsa.pub*.

- Asociar la llave pública local con la cuenta de GitHub:

    1. Copiar la llave pública impresa en el punto anterior.
    2. Ir a la configuración de la cuenta de GitHub *GitHub Profile* --> *Settings* --> *SSH and GPG keys*.
    3. Crear una nueva entrada SSH *New SSH key*:
        * En *title* pongan un nombre que les recuerde a la PC donde estén trabajando.
        * En *key* tienen que pegar la llave pública.
        * Por último clickear en *Add SSH key*.

#### LINKS DE AYUDA

- DOCUMENTACIÓN OFICIAL         --> https://git-scm.com/docs
- ENTREVISTA LINUS TORVALDS     --> https://www.youtube.com/watch?v=o8NPllzkFhE&t=465s
- GITHUB                        --> https://github.com/ 
- GUÍA DE INSTALACIÓN GIT       --> https://git-scm.com/book/es/v2/Inicio---Sobre-el-Control-de-Versiones-Instalaci%C3%B3n-de-Git

- ¿Cómo asociar las llaves SSH? --> https://nancyzitle.medium.com/crear-una-clave-ssh-en-git-y-vincular-en-tu-cuenta-de-github-e7a6b22bc93f

