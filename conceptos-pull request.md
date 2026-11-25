1. Crear una rama (Branch)
Una rama o Branch es una línea de trabajo independiente que permite realizar modificaciones en un proyecto sin afectar directamente a la rama principal (main).
Pasos para crear una rama:
Entrar en el repositorio de GitHub.
Acceder a la pestaña Code.
Pulsar el selector de ramas, donde aparece main.
Escribir el nombre de la nueva rama, por ejemplo, nueva-funcionalidad.
Seleccionar Create branch para crearla a partir de main.
2. Realizar cambios en el proyecto
Una vez creada la rama, podemos empezar a modificar los archivos del proyecto.
Pasos:
Comprobar que estamos trabajando en la rama que acabamos de crear.
Abrir los archivos que queremos modificar.
Realizar los cambios necesarios en el código.
Guardar los archivos modificados
Es importante trabajar siempre en nuestra propia rama para no modificar directamente el código principal del proyecto.
3. Realizar un Commit
Un Commit es una confirmación que permite guardar los cambios realizados en el proyecto y registrar una versión del trabajo.
Pasos:
Revisar los archivos que hemos modificado.
Preparar los cambios para guardarlos.
Escribir un mensaje breve que explique qué hemos cambiado.
Pulsar Commit para confirmar los cambios.
Desde la terminal podemos utilizar los siguientes comandos:
git add .
git commit -m "Añadido nuevo apartado"
El comando git add . prepara los archivos modificados y git commit registra los cambios con un mensaje descriptivo.
4. Subir los cambios a GitHub (Push)
Después de realizar el Commit, debemos subir los cambios al repositorio remoto de GitHub para que estén disponibles para los demás colaboradores.
Para hacerlo desde la terminal, utilizamos:
git push origin nueva-funcionalidad
Este comando envía los cambios de nuestra rama local a GitHub.
5. Abrir una Pull Request (PR)
Una Pull Request es una solicitud que permite proponer que los cambios realizados en una rama se incorporen a otra, normalmente a la rama principal (main).
Pasos:
Entrar en el repositorio de GitHub.
Acceder a la pestaña Pull requests.
Pulsar New pull request.
Seleccionar la rama principal (main) como rama de destino (Base).
Seleccionar nuestra rama como rama de comparación (Compare).
Revisar las diferencias entre ambas ramas.
Pulsar Create pull request.
Escribir un título y una descripción explicando los cambios realizados.
Confirmar la creación de la Pull Request.
6. Solicitar una revisión (Review)
Antes de fusionar los cambios, es recomendable solicitar a otro desarrollador que revise el código para comprobar que funciona correctamente y que no contiene errores.
Pasos:
Abrir la Pull Request creada.
Buscar el apartado Reviewers.
Seleccionar al compañero o desarrollador que queremos que revise el código.
Confirmar la solicitud de revisión.
El revisor puede realizar tres acciones:
Approve: aprueba los cambios y considera que están preparados para fusionarse.
Request changes: solicita modificaciones antes de aprobarlos.
Comment: deja comentarios o sugerencias sobre el código.
Si se solicitan cambios, debemos modificar los archivos en nuestra rama, realizar un nuevo Commit y subirlos mediante Push. Las modificaciones aparecerán automáticamente en la misma Pull Request.
7. Fusionar los cambios mediante Merge
Una vez revisados y aprobados los cambios, podemos incorporarlos a la rama principal mediante un proceso llamado Merge.
Pasos:
Abrir la Pull Request.
Comprobar que no existen conflictos pendientes.
Verificar que se cumplen los requisitos de revisión del repositorio.
Pulsar Merge pull request.
Confirmar la operación mediante Confirm merge.
Una vez realizado el Merge, los cambios de nuestra rama se incorporan a main y pasan a formar parte del proyecto principal. Opcionalmente, podemos eliminar la rama que hemos utilizado.
8. Resumen del proceso
El proceso completo sigue este orden:
Branch: crear una rama nueva para trabajar de forma independiente.
Changes: realizar las modificaciones necesarias en el proyecto.
Commit: guardar los cambios con un mensaje descriptivo.
Push: subir los cambios a GitHub.
Pull Request: solicitar incorporar los cambios a la rama principal.
Review: pedir a otro desarrollador que revise y apruebe el código.
Merge: fusionar los cambios con la rama principal.
9. Ejemplo práctico
Imaginemos que estamos trabajando en una página web y queremos añadir un formulario de contacto.
Primero, creamos una rama llamada formulario-contacto. Después, modificamos el archivo HTML para añadir el formulario y guardamos los cambios mediante un Commit con el mensaje «Añadido formulario de contacto».
A continuación, subimos la rama a GitHub mediante Push y abrimos una Pull Request para solicitar que los cambios se incorporen a main.
Después, pedimos a un compañero que revise el código. Cuando lo aprueba, realizamos el Merge y el formulario pasa a formar parte de la versión principal de la página web.
Conclusión: trabajar con ramas, commits y Pull Requests permite organizar mejor los proyectos, evitar modificaciones directas en el código principal y facilitar la colaboración entre diferentes desarrolladores.
