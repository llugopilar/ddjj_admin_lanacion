# Admin Declaraciones juradas tres poderes

Esta aplicación fué creada con el fin de que más organizaciones puedan hacer uso de este software ("Declaraciones Juaradas Abiertas") desarrollado por La Nación Data.

## Tutorial de carga:

[Ejemplo de guía de carga de información a través del formulario online.](https://docs.google.com/document/d/1f0aUuqtxJAVwy-vQJY6NtJ28lPILDoET8X0cQf4JGEY/edit)

## Instalación

**Requerimientos:** 

* Python 2.7
* Pip
* Virtualenv

Crear el virtualenv

```bash
$ virtualenv ~/.venv_admin_ddjj
$ source ~/.venv_admin_ddjj/bin/activate
```

Clonar el proyecto

```bash
$ git clone https://github.com/lanacioncom/ddjj_admin.git
$ cd ddjj_admin
```

Instalar requerimientos

```bash
$ pip install -r requierements.txt
```

Primera migración

```bash
$ python manage.py migrate
```

Crear super user para ingresar al admin

```bash
$ python manage.py createsuperuser
```


## Docker

1. Instalar Docker: https://docs.docker.com/installation/
2. Crear Imagen y Containers
    
    `$ ./dockercreate.sh`

3. Crear Usuario de Admin (desde container)
    
    `# python manage.py createsuperuser`

4. Levantar el sitio
    
    `# python manage.py runserver 0.0.0.0:8000`

5. Obtener puerto

    `# ./dockercli.sh port`
    
6. Acceder desde el host a localhost al puerto correcto.

* Para facilitar el uso de los contenedores se agrego el script dockercli.sh

## Participantes:

* [momiperalta]
* [fcoel]
* [colmanromi]
* [gabybouret]
* [MarianTV]
* [cbertelegni]
* [\_\_rustico\_\_]



[colmanromi]:https://twitter.com/colmanromi
[gabybouret]:https://twitter.com/gabybouret
[momiperalta]:https://twitter.com/momiperalta
[fcoel]:https://twitter.com/fcoel
[MarianTV]:https://twitter.com/MarianTV
[cbertelegni]:https://twitter.com/cbertelegni
[\_\_rustico\_\_]:https://twitter.com/__rustico__
