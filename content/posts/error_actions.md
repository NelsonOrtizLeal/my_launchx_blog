---
title: "Semana 1 - Creacion del blog, Error en la parte de Actions"
date: 2022-05-11T18:16:21-06:00
description: 'Error con permisos al crear un GitHub Action'
---

# GitHub Actions
Es una herramienta que te ofrece GitHub y permite automatizar tareas de Build y Deploy. Mira a GitHub Actions como una maquina virtual en la cual le puedes dar instrucciones o comandos, ejemplo hacer un ls, mkdir, etc. El potencial de esta herramienta es que usando un archivo .yml y configurando tu repositorio, puedes hacer que github compile y despues depliegue tu proyecto al hacer un simple push a tu repositorio remoto.

# Problematica
Despues de realizar un **fork** al repositorio original de este blog se tenia que realizar algunas configuraciones sencillas, como lo actualizar el nombre y datos del blog. El problema se presento al momento de que github trato de ejetuar la actions.

![Error en el paso de Push changes ](https://user-images.githubusercontent.com/70604316/167820672-1c2e7952-de76-4dad-95c0-f14533944898.png)


# Solucion
Para solucionar este error, revisa los siguientes puntos en tu archivo .yml:

1. Verifica que la rama a la cual se hara el PUSH es la correcta.
2. Verifica que el correo y nombre de usuario sean los correctos, para que tenga los permisos de escritura.
3. Revisa la configuracion del repositorio, configuración en settings/actions/general, se tenia que marcar la casilla de Read an Write

Y listo, eso son las soluciones mas comunes cuando el github bot no tiene permiso para hacer el PUSH al repositorio y actualizar tu pagina.
