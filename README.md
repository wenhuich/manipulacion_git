# manipulacion_git

### Requisitos para manipular Git:
Necesitas tener el git instalado en linux para poder seguir con la configuración.

### Vamos a configurar su Git con su nombre de usuario en github, correo enlazado en él y activar el coloreado de la salida. 
```
  git config --global user.name "Your-Full-Name"
  git config --global user.email "your-email-address"
  git config --global color.ui auto
```
Con el list, le mostraremos lo que has configurado.
```
  git config --list
```

![configuraciongit](https://user-images.githubusercontent.com/91631138/140182232-fe7bb567-1778-4aa6-b53f-45a9abf884ad.png)

### Paso 2:
Toca crear el Git con el nombre dpl:
```
 mkdir dpl
 cd dpl
 git init
 ls -la
```

![creargit](https://user-images.githubusercontent.com/91631138/140182308-c09deb7f-5dec-4868-b7d3-87b83bc77a30.png)

En mi caso ya lo tenía creado.

### Paso 3:
Con el primero comprobamos el estatus.
Crear un fichero indice.txt con el siguiente contenido:
Capítulo 1: Instalación de Git por el alumno XXX (donde XXX es el nombre del alumno)
Capítulo 2: Flujo de trabajo básico
Le damos Ctrl+D para salir 
Comprobamos de nuevo el estatus.
```
 git status
 cat > indice.txt
 Capítulo 1: Instalación de Git por el alumno XXX
 Capítulo 2: Flujo de trabajo básico
 Ctrl+D
 git status
 git add indice.txt
 git status
```

![estatusgit](https://user-images.githubusercontent.com/91631138/140182429-8e2ec6e6-c8f5-4bf0-9fa9-469bb12ee088.png)

### Paso 4:
Añadimos un commit haciéndole cambio con el mensaje Añadido índice de la asignatura DPL. 
Ver el estado del repositorio.
```
git commit -m "Añadido índice de la asignatura DPL."
git status
```

![commitgit](https://user-images.githubusercontent.com/91631138/140182514-0e1665c1-11d5-4aa2-a6b5-7666b0b15956.png)

### Para modificar:
Para modificar un fichero:
Cambiar el fichero indice.txt para que contenga lo siguiente:
Capítulo 1: Instalación de Git por el alumno XXX (donde XXX es el nombre del alumno)
Capítulo 2: Flujo de trabajo básico
Capítulo 3: Gestión de ramas
Capítulo 4: Repositorios remotos
Mostrar los cambios con respecto a la última versión guardada en el repositorio.
Hacer un commit de los cambios con el mensaje Añadido los capítulos 3 y 4.
```
cat > indice.txt
Capítulo 1: Instalación de Git por el alumno XXX _(donde XXX es el nombre del alumno)_
Capítulo 2: Flujo de trabajo básico
Capítulo 3: Gestión de ramas
Capítulo 4: Repositorios remotos
Ctrl+D
git diff
git add indice.txt
git commit -m "Añadido los capitulos 3"
```

![modificacionficherogit](https://user-images.githubusercontent.com/91631138/140182589-155bf8c4-a468-4e67-8a37-a96bca04ccaf.png)

### Para ver el historial:
```
git show
git commit --amend -m "Añadido el capitulo sobre gestión de ramas al índice."
git show
```

![historialgit](https://user-images.githubusercontent.com/91631138/140182654-44a8a2da-4566-4adc-9fc9-8ae517671ebe.png)

