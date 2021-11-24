# django-cms
**Creación del entorno virtual**

Primero empezaremos con la creación y activación del entorno virtual, para crear el entorno virtual vamos a ejecutar:

<pre>debian@debian:~$ python3 -m venv env
</pre>

Activamos el entorno:

<pre>debian@debian:~$ source env/bin/activate
(env) debian@debian:~$ 
</pre>

**Instalación de Django CMS**

Para instalar DjangoCMS vamos a utilizar un instalador:

<pre>(env) debian@debian:~$ pip install djangocms-installer
</pre>

Ahora procederemos a crear nuestro directorio de trabajo y crear el proyecto Django:

<pre>(env) debian@debian:~$ mkdir tutorial-project
</pre>

Ingresamos al directorio y creamos el proyecto en este caso se va llamar mysite:

<pre>(env) debian@debian:~/tutorial-project$ djangocms -f -p . mysite
</pre>

EL parámetro -f instala djanfgo filer y -p es para utilizar el directorio actual.

**Inicio en el servidor de desarrollo**

Comprobemos de que la aplicación está corriendo:

<pre>(env) debian@debian:~/tutorial-project$ python3 manage.py runserver
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).
November 24, 2021 - 12:38:11
Django version 3.1.13, using settings 'mysite.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CONTROL-C.
</pre>
