# writeups-dockerlabs

[](https://github.com/incommatose/dockerlabs-writeups/tree/main#writeups-dockerlabs)

Bienvenid@s 👋, soy Maximliano y soy un estudiante de ciberseguridad y hacking ético 💻📚. En este repositorio almacenaré todas las guías sobre resoluciones de máquinas de la plataforma de `Dockerlabs.es` 🐳. Tienes disponible la siguiente tabla de contenido con las respectivas guías clasificadas por dificultad, espero que te sirva de ayuda este aporte, si tienes algún comentario o sugerencia, no dudes en contactarme 💪.

## Lanzar el laboratorio

[Laboratorio](https://github.com/incommatose/dockerlabs-writeups/tree/main#lanzar-el-laboratorio)

Para desplegar el laboratorio de `docker` con el que practicaremos, ejecutamos los siguientes comandos

```shell
# Descomprimimos el archivo
unzip {machine.tar}

# Asignamos permisos de ejecución al script que despliega el laboratorio
chmod +x auto_deploy.sh

# Lanzamos el laboratorio
./auto_deploy.sh machine1.tar machine2.tar
```

## Consideraciones

[WriteUps](https://github.com/incommatose/dockerlabs-writeups/tree/main#consideraciones)

Si usas otra distribución que no esté basada en Debian, debes saber que el script no instalará `docker` en tu distribución porque está pensado para una instalación con `apt`, por lo que debes instalarlo por tu cuenta y activar el servicio antes de ejecutar el script

```shell
# Instalación en Arch Linux (ejemplo)
pacman -S docker

# Activamos el servicio de docker
systemctl start docker

# Ahora podemos lanzar el/los contenedor/es
./auto_deploy.sh maquina.tar
```
