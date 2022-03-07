# MAESTRÍA DE INTELIGENCIA DE NEGOCIOS Y ANÁLISIS DE DATOS
## Ciencia de Datos en Python
## Ing. Preng Biba
## Alumno: Willard Alfaro
## Carné: 20043236

# Contenido
Que es Git y Github	3

Los Tres Estados	5

La Línea de Comandos	7
1. Git clone	7
2. Git branch	8
3. Git checkout	8
4. Git status	8
5. Git add	9
6. Git commit	10
7. Git push	10
8. Git pull	11
9. Git revert	11
10. Git merge	12
GitHub Desktop	12

Colaborar en proyectos con GitHub Desktop	13

Crear, agregar y clonar repositorios	13

Colaborar con GitHub Desktop	13

Crear un repositorio nuevo	13

Publicar tu repositorio en GitHub	14

Hacer, confirmar y subir cambios	15

Atajos de Teclado	17

Atajos en todo el sitio	17

Repositorios	18

Ramas	19

¿Qué es Markdown?	19

Sintaxis de escritura y formato básicos	22

Encabezados	22

Estilo de texto	22

Cita de texto	23

Código de cita	23

Enlaces	24

Enlaces de sección	24

Enlaces relativos	24

Imágenes	25

Especificar un tema en el que se muestra una imagen	25

Listas	26

Listas anidadas	26

Listas de tareas	27

Mencionar personas y equipos	28

Hacer referencia a propuestas y solicitudes de extracción	28

Hacer referencia a recursos externos	28

Cargar activos	29

Usar emojis	29

Párrafos	29

Notas al pie	29

Ocultar el contenido con comentarios	30

Importar formato de Markdown	30

Inhabilitar la representación del lenguaje de marcado	30


 
# Investigación 1


## Que es Git y Github
El control de versiones es el proceso de guardar diferentes archivos o «versiones» a lo largo de las diferentes etapas de un proyecto de desarrollo. Esto permite a los desarrolladores hacer un seguimiento de lo que se ha hecho y volver a una fase anterior si deciden que quieren revertir algunos de los cambios que han hecho.

Git almacena cada versión guardada como una ‘instantánea’ en lugar de una lista de los cambios realizados en cada archivo. Puede hacer referencia a antiguas instantáneas siempre que lo necesite y las nuevas instantáneas se crean cuando se modifica el proyecto.

Git también le permite «empujar» y «tirar» de los cambios hacia y desde las instalaciones de otros ordenadores. Esto lo convierte en lo que se conoce como ‘Sistema de control de versiones distribuido’, y permite que varios desarrolladores trabajen en el mismo proyecto.

Sin embargo, hay algunos inconvenientes para manejar el desarrollo de esta manera. Como el software local está instalado en su máquina individual, git no puede leer las ediciones que otros desarrolladores puedan estar haciendo en tiempo real. Esto significa que si usted y un compañero de equipo están trabajando en un proyecto simultáneamente, no podrán ver el trabajo del otro.

GitHub facilita la colaboración con git. Es una plataforma que puede mantener repositorios de código en almacenamiento basado en la nube para que varios desarrolladores puedan trabajar en un solo proyecto y ver las ediciones de cada uno en tiempo real.

Además, también incluye funciones de organización y gestión de proyectos. Puede asignar tareas a individuos o grupos, establecer permisos y roles para los colaboradores y usar la moderación de comentarios para mantener a todos en la tarea.
GitHub están disponibles públicamente. Los desarrolladores de todo el mundo pueden interactuar y contribuir al código de los demás para modificarlo o mejorarlo, lo que se conoce como «codificación social». En cierto modo, esto hace que GitHub sea un sitio de redes para profesionales de la web.

Hay tres acciones principales que puede realizar cuando se trata de interactuar con el código de otros desarrolladores en GitHub:
Bifurcación: El proceso de copiar el código de otra persona del repositorio para modificarlo.

Pull: Cuando haya terminado de hacer cambios en el código de otra persona, puede compartirlos con el propietario original a través de una «solicitud pull».

Fusión: Los propietarios pueden añadir nuevos cambios a sus proyectos a través de una fusión, y dar crédito a los contribuyentes que los han sugerido.

Para poder usar git y GitHub juntos para el control de versiones y la colaboración, hay algunos pasos que tendrá que dar:

## Paso 1: Instalar git y Añadir un Repositorio
Descargar el software git desktop
Una vez que esté en funcionamiento, hay algunos términos con los que querrá familiarizarse cuando empiece a usar el software:

### Repositorio: La ubicación del archivo donde se almacena su proyecto.
### Comprometerse: El comando utilizado para guardar los nuevos cambios en su proyecto en el repositorio.
### Escenario: Antes de que puedas confirmar los cambios en Git, necesitas prepararlos -esto le da la oportunidad de preparar su código antes de añadirlo formalmente a su proyecto.
### Rama: La parte de su proyecto que está desarrollando activamente.

Para conectar git a GitHub, necesitarás añadir un repositorio y hacer al menos una confirmación. Entonces tendrá suficiente de su proyecto establecido para empezar a trabajar en GitHub.

## Paso 2: Crear una cuenta GitHub
A continuación, necesitarás una cuenta GitHub. Puede inscribirse en uno de ellos de forma gratuita o invertir en un plan de pago:
## Paso 3: Añadir un Repositorio GitHub a su cuenta
Después de que haya creado y configurado su cuenta, necesitará crear un repositorio en GitHub donde pueda almacenar su proyecto cuando lo mueva desde git.
## Paso 4: Empujar un Repositorio a GitHub
A continuación, tendrá la opción de añadir código a su repositorio de unas cuantas formas diferentes.
Como ya ha configurado su repositorio git, puede usar la opción de empujar un repositorio existente desde la línea de comandos:
 ![Esta es una imagen] 

El icono del portapapeles a la derecha le permite copiar los comandos que se enumeran aquí, de modo que puede pegarlos rápidamente en su interfaz de línea de comandos preferida para crear su repositorio GitHub.

Una vez hecho esto, actualice su página de GitHub. Ahora debería poder ver su repositorio en GitHub. A partir de ahí, puede empezar a hacer cambios en su proyecto en línea. También es posible enviar y fusionar solicitudes de extracción, y utilizar cualquier otra herramienta i 

## Paso 5: Retirar los Cambios a git
Aunque puede ver todos los cambios que usted y otros han hecho en su proyecto en GitHub, la plataforma no tiene acceso directo a los archivos de su ordenador. Para mantener su proyecto actualizado en su computadora, necesitará hacer sus ediciones a través de git.
Para ello, simplemente introduzca git pull origin master en su interfaz de línea de comandos. Esto debería actualizar sus archivos para que todo esté sincronizado en todas las iteraciones de su proyecto incluida en su plan.

# Los Tres Estados
Git tiene tres estados principales en los que se pueden encontrar tus archivos: confirmado (committed), modificado (modified), y preparado (staged). Confirmado: significa que los datos están almacenados de manera segura en tu base de datos local. Modificado: significa que has modificado el archivo pero todavía no lo has confirmado a tu base de datos. Preparado: significa que has marcado un archivo modificado en su versión actual para que vaya en tu próxima confirmación.
Esto nos lleva a las tres secciones principales de un proyecto de Git: El directorio de Git (Git directory), el directorio de trabajo (working directory), y el área de preparación (staging area).
 
Directorio de trabajo, área de almacenamiento y el directorio Git.
El directorio de Git es donde se almacenan los metadatos y la base de datos de objetos para tu proyecto. Es la parte más importante de Git, y es lo que se copia cuando clonas un repositorio desde otra computadora.
El directorio de trabajo es una copia de una versión del proyecto. Estos archivos se sacan de la base de datos comprimida en el directorio de Git, y se colocan en disco para que los puedas usar o modificar.
El área de preparación es un archivo, generalmente contenido en tu directorio de Git, que almacena información acerca de lo que va a ir en tu próxima confirmación. A veces se le denomina índice (“index”), pero se está convirtiendo en estándar el referirse a ella como el área de preparación.

El flujo de trabajo básico en Git es algo así:
1.	Modificas una serie de archivos en tu directorio de trabajo.
2.	Preparas los archivos, añadiéndolos a tu área de preparación.
3.	Confirmas los cambios, lo que toma los archivos tal y como están en el área de preparación y almacena esa copia instantánea de manera permanente en tu directorio de Git.
Si una versión concreta de un archivo está en el directorio de Git, se considera confirmada (committed). Si ha sufrido cambios desde que se obtuvo del repositorio, pero ha sido añadida al área de preparación, está preparada (staged). Y si ha sufrido cambios desde que se obtuvo del repositorio, pero no se ha preparado, está modificada (modified). 
 
# La Línea de Comandos
Existen muchas formas de usar Git. Por un lado tenemos las herramientas originales de línea de comandos, y por otro lado tenemos una gran variedad de interfaces de usuario con distintas capacidades. La línea de comandos es el único lugar en donde puedes ejecutar todos los comandos de Git - la mayoría de las interfaces gráficas de usuario solo implementan una parte de las características de Git por motivos de simplicidad.
A continuación se detallan los comandos mas usados en linea de comandos:
## 1. Git clone
Git clone es un comando para descargarte el código fuente existente desde un repositorio remoto (como Github, por ejemplo). En otras palabras, Git clone básicamente realiza una copia idéntica de la última versión de un proyecto en un repositorio y la guarda en tu ordenador.
Hay un par de formas de descargar el código fuente, pero principalmente yo prefiero clonar de la forma con https:
git clone <https://link-con-nombre-del-repositorio>
Por ejemplo, si queremos descargar un proyecto desde Github, todo lo que necesitamos es hacer clic sobre el botón verde (clonar o descargar), copiar la URL de la caja y pegarla después del comando git clone que he mostrado más arriba.
 
Código fuente de Bootstrap en Github
Esto hará una copia del proyecto en tu espacio de trabajo local y así podrás empezar a trabajar con él.
## 2. Git branch
Las ramas (branch) son altamente importantes en el mundo de Git. Usando ramas, varios desarrolladores pueden trabajar en paralelo en el mismo proyecto simultáneamente. Podemos usar el comando git branch para crearlas, listarlas y eliminarlas.
Creando una nueva rama:
git branch <nombre-de-la-rama>
Este comando creará una rama en local. Para enviar (push) la nueva rama al repositorio remoto, necesitarás usar el siguiente comando:
git push <nombre-remoto> <nombre-rama>
Visualización de ramas:
git branch
git branch --list
Borrar una rama:
git branch -d <nombre-de-la-rama>

## 3. Git checkout
Este es también uno de los comandos más utilizados en Git. Para trabajar en una rama, primero tienes que cambiarte a ella. Usaremos git checkout principalmente para cambiarte de una rama a otra. También lo podemos usar para chequear archivos y commits.
git checkout <nombre-de-la-rama>
Hay algunos pasos que debes seguir para cambiarte exitosamente entre ramas:
•	Los cambios en tu rama actual tienen que ser confirmados o almacenados en el guardado rápido (stash) antes de que cambies de rama.
•	La rama a la que te quieras cambiar debe existir en local.
Hay también un comando de acceso directo que te permite crear y cambiarte a esa rama al mismo tiempo:
git checkout -b <nombre-de-tu-rama>
Este comando crea una nueva rama en local (-b viene de rama (branch)) y te cambia a la rama que acabas de crear.
## 4. Git status
El comando de git status nos da toda la información necesaria sobre la rama actual.
git status
Podemos encontrar información como:
•	Si la rama actual está actualizada
•	Si hay algo para confirmar, enviar o recibir (pull).
•	Si hay archivos en preparación (staged), sin preparación(unstaged) o que no están recibiendo seguimiento (untracked)
•	Si hay archivos creados, modificados o eliminados
 git status nos da información acerca del archivo y las ramas

## 5. Git add
Cuando creamos, modificamos o eliminamos un archivo, estos cambios suceden en local y no se incluirán en el siguiente commit (a menos que cambiemos la configuración).
Necesitamos usar el comando git add para incluir los cambios del o de los archivos en tu siguiente commit.
Añadir un único archivo:
git add <archivo>
Añadir todo de una vez:
git add -A
Si revisas la captura de pantalla que he dejado en la sección 4, verás que hay nombres de archivos en rojo - esto significa que los archivos sin preparación. Estos archivos no serán incluidos en tus commits hasta que no los añadas.
Para añadirlos, necesitas usar el git add:
 Los archivos en verde han sido añadidos a la preparación gracias al git add
Importante: El comando git add no cambia el repositorio y los cambios que no han sido guardados hasta que no utilicemos el comando de confirmación git commit.

## 6. Git commit
Este sea quizás el comando más utilizado de Git. Una vez que se llega a cierto punto en el desarrollo, queremos guardar nuestros cambios (quizás después de una tarea o asunto específico).  
Git commit es como establecer un punto de control en el proceso de desarrollo al cual puedes volver más tarde si es necesario.
También necesitamos escribir un mensaje corto para explicar qué hemos desarrollado o modificado en el código fuente.
git commit -m "mensaje de confirmación"
Importante: Git commit guarda tus cambios únicamente en local.

## 7. Git push
Después de haber confirmado tus cambios, el siguiente paso que quieres dar es enviar tus cambios al servidor remoto. Git push envía tus commits al repositorio remoto.
git push <nombre-remoto> <nombre-de-tu-rama>
De todas formas, si tu rama ha sido creada recientemente, puede que tengas que cargar y subir tu rama con el siguiente comando:
git push --set-upstream <nombre-remoto> <nombre-de-tu-rama>
or
git push -u origin <nombre-de-tu-rama>
Importante: Git push solamente carga los cambios que han sido confirmados.

## 8. Git pull
El comando git pull se utiliza para recibir actualizaciones del repositorio remoto. Este comando es una combinación del git fetch y del git merge lo cual significa que cundo usemos el git pull recogeremos actualizaciones del repositorio remoto (git fetch) e inmediatamente aplicamos estos últimos cambios en local (git merge).
git pull <nombre-remoto>
Esta operación puede generar conflictos que tengamos que resolver manualmente.

## 9. Git revert
A veces, necesitaremos deshacer los cambios que hemos hecho. Hay varias maneras para deshacer nuestros cambios en local y/o en remoto (dependiendo de lo que necesitemos), pero necesitaremos utilizar cuidadosamente estos comandos para evitar borrados no deseados.
Una manera segura para deshacer nuestras commits es utilizar git revert. Para ver nuestro historial de commits, primero necesitamos utilizar el  git log -- oneline:
 histórico de git en mi rama master
Entonces, solo necesitamos especificar el código de comprobación que encontrarás junto al commit que queremos deshacer:
git revert
Después de esto, verás una pantalla como la de abajo -tan solo presiona shift + q para salir:
 
El comando git revert deshará el commit que le hemos indicado, pero creará un nuevo commit deshaciendo la anterior:
 commit generado con el git revert
La ventaja de utilizar git revert es que no afecta al commit histórico. Esto significa que puedes seguir viendo todos los commits en tu histórico, incluso los revertidos.
Otra medida de seguridad es que todo sucede en local a no ser que los enviemos al repositorio remoto. Por esto es que git revert es más seguro de usar y es la manera preferida para deshacer los commits.
## 10. Git merge
Cuando ya hayas completado el desarrollo de tu proyecto en tu rama y todo funcione correctamente, el último paso es fusionar la rama con su rama padre (dev o master). Esto se hace con el comando git merge.
Git merge básicamente integra las características de tu rama con todos los commits realizados a las ramas dev (o master).  Es importante que recuerdes que tienes que estar en esa rama específica que quieres fusionar  con tu rama de características.
Por ejemplo, cuando quieres fusionar tu rama de características en la rama dev:
Primero, debes cambiarte a la rama dev:
git checkout dev
Antes de fusionar, debes actualizar tu rama dev local:
git fetch
Por último, puedes fusionar tu rama de características en la rama dev:
git merge <nombre-de-la-rama>
Pista: Asegúrate de que tu rama dev tiene la última versión antes de fusionar otras ramas, si no, te enfrentarás a conflictos u otros problemas no deseados.

# GitHub Desktop
GitHub Desktop es una herramienta de código abierto que permite ser más productivo. Fomenta que el equipo colabore utilizando las mejoras prácticas con Git y GitHub.
Una parte de lo que puedes hacer GitHub Desktop:
•	Añadir cambios a tu confirmación de forma interactiva
•	Añadir co-autores rápidamente en tu confirmación
•	Controlar ramas con solicitudes de extracción y ver los estados de CI
•	Comparar las imágenes que han cambiado
Colaborar en proyectos con GitHub Desktop
Después de instalar, autenticarte y configurar la app, estás listo para comenzar a utilizar GitHub Desktop. Puedes crear, agregar, o clonar los repositorios y utilizar GitHub Desktop para administrar las contribuciones a tus repositorios.
Crear, agregar y clonar repositorios
Puedes crear un repositorio nuevo si seleccionas el menú de archivo y das clic en Repositorio nuevo.... Para obtener más información, consulta la sección "Crear tu primer repositorio utilizando GitHub Desktop".
Puedes agregar un repositorio desde tu computadora local si seleccionas el menú de Archivo y das clic en Agregar Repositorio Local.... 
Puedes clonar un repositorio desde GitHub si seleccionas el menú de Archivo y das clic en Clonar Repositorio.... 
 

# Colaborar con GitHub Desktop
GitHub Desktop es útil para crear informes de problemas o solicitudes de extracción para colaborar en proyectos con otras personas. Los informes de problemas te ayudan a llevar un seguimiento de las ideas y debatir los posibles cambios a los proyectos. Las solicitudes de extracción te permiten compartir tus cambios propuestos con los demás, recibir retroalimentación y fusionar los cambios en un proyecto. 
Puedes ver tus propias solicitudes de extracción o las de tus colaboradores en GitHub Desktop. El visualizar una solicitud de extracción en GitHub Desktop te permite ver cualquier cambio propuesto y hacer cambios adicionales si abres los repositorios y archivos del proyecto en tu editor de texto predeterminado.
# Crear un repositorio nuevo
Si no quieres crear y clonar un repositorio de tutorial, puedes crear un repositorio nuevo.
1.	Haz clic en Crear un nuevo repositorio en tu disco duro...
 
2.	Llena los campos y selecciona tus opciones preferidas.	

o	"Name" (Nombre) define el nombre de tu repositorio a nivel local y en GitHub.

o	"Description" (Descripción) es un campo opcional que puedes usar para brindar más información sobre el objetivo de tu repositorio.

o	"Local path" (Ruta local) establece la ubicación de repositorio en computadora. De manera predeterminada, GitHub Desktop crea una carpeta GitHub en tu carpeta Documents (Documentos) para almacenar tus repositorios, pero puedes elegir cualquier ubicación en tu computadora. Tu nuevo repositorio será una carpeta dentro de la ubicación elegida. Por ejemplo, si colocas el nombre Tutorial a tu repositorio, se creará la carpeta Tutorial dentro de la carpeta que seleccionaste en tu ruta local. 

o	Si se inicializa este repositorio con un README (Léeme), se crea una confirmación inicial con un archivo README.md. README ayuda a las personas a comprender el objetivo de tu proyecto, por lo que recomendamos seleccionarlo y completarlo con información útil. Cuando alguien visita tu repositorio en GitHub, el archivo README es lo primero que verán a medida que aprenden sobre tu proyecto. 

# Publicar tu repositorio en GitHub
Cuando creas un repositorio nuevo, éste solo existirá en la computadora y sere el único que pueda acceder a él. Se puede publicar tu repositorio en GitHub para mantenerlo sincronizado a través de varias computadoras y permitir que otras personas accedan a él. Para publicar tu repositorio, sube tus cambios locales a GitHub.
1.	Da clic en Publicar repositorio en la barra de menú. 
o	GitHub Desktop llenará los campos de "Nombre" y "Descripción" automáticamente con la información que ingresaste cuando creaste el repositorio.
o	La opción de Mantener este código como privado te permite controlar quién puede ver tu proyecto. Si no seleccionas esta opción, otros usuarios en GitHub podrán ver tu código. Si seleccionas esta opción, tu código no estará disponible al público en general.
o	El menú desplegable de Organización, si es que lo hay, te permite publicar tu repositorio en una organización específica en GitHub a la cual pertenezcas.
 
2.	Haz clic en el botón Publish Repository (Publicar repositorio).
3.	Puedes acceder al repositorio en GitHub.com desde el interior de GitHub Desktop. En el menú del archivo, haz clic en Repository (Repositorio), luego haz clic en View on GitHub (Ver en GitHub). Esto te llevará directamente hasta el repositorio en tu navegador predeterminado.

# Hacer, confirmar y subir cambios
Ahora que creaste y publicaste tu repositorio, estás listo para hacer cambios en tu proyecto y comenzar a crear tu primera confirmación para este repositorio.
1.	Para lanzar tu editor externo desde dentro de GitHub Desktop, da clic en Repositorio, luego da clic en Abrir en EDITOR. 
2.	Haz algunos cambios al archivo README.md que hayas creado previamente. Puedes agregar información que describa tu proyecto, como por ejemplo, que es lo que hace y por qué es útil. Cuando estés satisfecho con los cambios, guárdalos en tu editor de texto.
3.	En GitHub Desktop, navega a la vista de Cambios. En la lista de archivos, deberías ver tu README.md. La marca de verificación a la izquierda del archivo README.md indica que los cambios que has hecho al archivo serán parte de la confirmación que haces. En el futuro, es posible que realices cambios a múltiples archivos pero solo quieras confirmar los cambios que realizaste en alguno de los archivos. Si das clic en la marca de verificación contigua a un archivo, este archivo no se incluirá en la confirmación. 
4.	En la parte inferior de la lista Changes (Cambios), escribe un mensaje de confirmación. A la derecha de tu imagen de perfil, escribe una descripción breve de la confirmación. Dado que estamos cambiando el archivo README.md, "Agregar información sobre el objetivo del proyecto" sería un buen resumen de la confirmación. Debajo del resumen, verás un campo de texto de "Descripción" en donde podrás teclear una descripción más amplia de los cambios en la confirmación, lo cual es de gran ayuda cuando regresas a ver el historial de un proyecto y entiendes por qué se realizaron los cambios. Dado que estás realizando una actualización básica de un archivo README.md, puedes omitir la descripción.
 
5.	Da clic en Confirmar al NOMBRE DE RAMA. El botón de confirmación muestra tu rama actual, así que puedes estar seguro de confirmar a la rama que quieras
. 
6.	Para subir los cambios al repositorio remoto en GitHub, haz clic en Push origin (Subir origen).
 

    •	El botón de Subir el origen es el mismo en el que diste clic para publicar tu repositorio en GitHub. Este botón cambia contextualmente con base en el punto en el que estés en el flujo de trabajo de Git. Ahora debería decir Subir el origen con un 1 en un costado, indicando que hay una confirmación que no se ha subido a GitHub.

    •	El "origen" en Subir el origen significa que estás subiendo los cambios al repositorio remoto llamado origin, que en este caso es el repositorio de tu proyecto en GitHub.com. Hasta que hayas subido alguna de las nuevas confirmaciones GitHub, habrá diferencias entre el repositorio de tu proyecto en tu computadora y el repositorio del proyecto en GitHub.com. Esto te permite trabajar localmente y solo subir tus cambios a GitHub.com cuando estés listo.

7.	En la ventana, a la derecha de la vista de Cambios, verás las sugerencias para las acciones que puedes hacer después. Para abrir el repositorio en GitHub en tu buscador, da clic en Ver en GitHub.
 
8.	En tu navegador, haz clic en 2 commits (2 confirmaciones). Verás una lista de las confirmaciones en este repositorio en GitHub. La primera confirmación deberá ser aquella que acabas de realizar en GitHub Desktop.
 
# Atajos de Teclado
Atajos en todo el sitio
Atajo del teclado	Descripción
Ctrl+,	Ir a Options (Opciones)
F11	Alternar vista de pantalla completa
Ctrl+0	Restablecer zoom al tamaño de texto predeterminado
Ctrl+=	Acercar para textos y gráficos más grandes
Ctrl+-	Alejar para textos y gráficos más pequeños
Ctrl+Shift+I	Alternar herramientas del desarrollador
Repositorios
Atajo del teclado	Descripción
Ctrl+N	Agregar un repositorio nuevo
Ctrl+O	Agregar un repositorio local
Ctrl+Shift+O	Clonar un repositorio desde GitHub
Ctrl+T	Mostrar una lista de tus repositorios
Ctrl+P	Subir las últimas confirmaciones a GitHub
Ctrl+Shift+P	Bajar los últimos cambios de GitHub
Ctrl+Delete	Eliminar un repositorio existente
Ctrl+Shift+G	Ver el repositorio en GitHub
Ctrl+`	Abrir el repositorio en tu herramienta de línea de comando preferida
Ctrl+Shift+F	Mostrar el repositorio en Explorador
Ctrl+Shift+A	Abrir el repositorio en tu herramienta de editor preferida
Ctrl+I	Crear un informe de problemas en GitHub
Ramas
Atajo del teclado	Descripción
Ctrl+1	Mostrar todos los cambios antes de confirmar
Ctrl+2	Mostrar tu historial de confirmaciones
Ctrl+B	Mostrar todas tus ramas
Ctrl+G	Ir al campo de resumen de confirmaciones
Ctrl+Enter	Confirma los cambios cuando el campo de resumen o de descripción está activo
Espacio	Selecciona o deselecciona todos los archivos resaltados
Ctrl+Shift+N	Crear una rama nueva
Ctrl+Shift+R	Renombrar la rama actual
Ctrl+Shift+D	Eliminar la rama actual
Ctrl+Shift+U	Actualizar desde la rama predeterminada
Ctrl+Shift+B	Comparar con una rama existente
Ctrl+Shift+M	Fusionar en una rama actual
Ctrl+H	Mostrar u ocultar cambios acumulados
Ctrl+Shift+C	Comparar ramas en GitHub
Ctrl+R	Mostrar la solicitud de extracción actual en GitHub
¿Qué es Markdown?
Markdown es un formato de texto sin formato para escribir documentos estructurados, basado en convenciones para indicar el formato en correos electrónicos y publicaciones de Usenet. Fue desarrollado por John Gruber (con la ayuda de Aaron Swartz) y lanzado en 2004 en forma de descripción de sintaxis y script Perl ( Markdown.pl) para convertir Markdown a HTML. En la próxima década, se desarrollaron docenas de implementaciones en muchos idiomas. Algunos ampliaron la sintaxis original de Markdown con convenciones para notas al pie, tablas y otros elementos del documento. Algunos permitieron que los documentos de Markdown se representaran en formatos distintos de HTML. Sitios web como Reddit, StackOverflow y GitHub tenían millones de personas que usaban Markdown. Y Markdown comenzó a usarse más allá de la web, para escribir libros, artículos, presentaciones de diapositivas, cartas y notas de conferencias.
Lo que distingue a Markdown de muchas otras sintaxis de marcado ligeras, que suelen ser más fáciles de escribir, es su legibilidad. Como Gruber escribe:
El objetivo principal del diseño de la sintaxis de formato de Markdown es hacer que sea lo más legible posible. La idea es que un documento con formato de Markdown se pueda publicar tal cual, como texto sin formato, sin que parezca que ha sido marcado con etiquetas o instrucciones de formato.
El punto se puede ilustrar comparando una muestra de AsciiDoc con una muestra equivalente de Markdown. Aquí hay una muestra de AsciiDoc del manual de AsciiDoc:
1. List item one.
+
List item one continued with a second paragraph followed by an
Indented block.
+
.................
$ ls *.sh
$ mv *.sh ~/tmp
.................
+
List item continued with a third paragraph.

2. List item two continued with an open block.
+
--
This paragraph is part of the preceding list item.

a. This list is nested and does not require explicit item
continuation.
+
This paragraph is part of the preceding list item.

b. List item b.

This paragraph belongs to item two of the outer list.
--
Y aquí está el equivalente en Markdown:
1.  List item one.

    List item one continued with a second paragraph followed by an
    Indented block.

        $ ls *.sh
        $ mv *.sh ~/tmp

    List item continued with a third paragraph.

2.  List item two continued with an open block.

    This paragraph is part of the preceding list item.

    1. This list is nested and does not require explicit item continuation.

       This paragraph is part of the preceding list item.

    2. List item b.

    This paragraph belongs to item two of the outer list.
Podría decirse que la versión de AsciiDoc es más fácil de escribir. No necesita preocuparse por la sangría. Pero la versión de Markdown es mucho más fácil de leer. El anidamiento de los elementos de la lista es evidente a simple vista en el origen, no solo en el documento procesado.

# Sintaxis de escritura y formato básicos
Crear formatos sofisticados para tu prosa y código en GitHub con sintaxis simple.

Encabezados
Para crear un encabezado, agrega uno a seis símbolos # antes del encabezado del texto. The number of # you use will determine the size of the heading.
# El encabezado más largo
## El segundo encabezado más largo
###### El encabezado más pequeño
 
## Estilo de texto
Puedes indicar énfasis con texto en negritas, itálicas o tachadas en los campos de comentario y archivos .md.
Estilo	Sintaxis	Atajo del teclado	Ejemplo	Resultado
Negrita	** ** o __ __	Command+B (Mac) or Ctrl+B (Windows/Linux)	**Este texto está en negrita**	Este texto está en negrita
Cursiva	* * o _ _     	Command+I (Mac) or Ctrl+I (Windows/Linux)	*Este texto está en cursiva*	Este texto está en cursiva
Tachado	~~ ~~		~~Este texto está equivocado~~	

Cursiva en negrita y anidada	** ** y _ _		**Este texto es _extremadamente_ importante**	Este texto es extremadamente importante
Todo en negrita y cursiva	*** ***		***Todo este texto es importante***	Todo este texto es importante
Cita de texto
You can quote text with a >.
Texto que no es una cita

> Texto que es una cita
 
Tip: When viewing a conversation, you can automatically quote text in a comment by highlighting the text, then typing R. Puedes citar un comentario completo al hacer clic en , y luego en Quote reply (Citar respuesta). 
Código de cita
Puedes indicar un código o un comando dentro de un enunciado con comillas simples. The text within the backticks will not be formatted. You can also press the Command+E (Mac) or Ctrl+E (Windows/Linux) keyboard shortcut to insert the backticks for a code block within a line of Markdown.
Usa `git status` para enumerar todos los archivos nuevos o modificados que aún no han sido confirmados.
 
Para formatear código o texto en su propio bloque distintivo, usa comillas triples.
Algunos de los comandos de Git básicos son:
```
git status
git add
git commit
```
 
Enlaces
Puedes crear un enlace en línea al encerrar el texto del enlace entre corchetes [ ], y luego encerrar la URL entre paréntesis ( ). 
Este sitio se construyó usando [GitHub Pages](https://pages.github.com/).
 
Sugerencias: GitHub automáticamente crea enlaces cuando las direcciones URL válidas están escritas en un comentario. 
Enlaces de sección
Puedes vincular directamente a una sección en un archivo expedido si deslizas el puntero sobre el encabezado de la sección para exponer el enlace:
 
Enlaces relativos
Puedes definir enlaces relativos y rutas de imagen en los archivos representados para ayudar a que los lectores naveguen hasta otros archivos de tu repositorio.
Un enlace relativo es un enlace que es relativo al archivo actual. Por ejemplo, si tienes un archivo README en la raíz de tu repositorio y tienes otro archivo en docs/CONTRIBUTING.md, el enlace relativo a CONTRIBUTING.md en tu archivo README podría verse así:
[Contribution guidelines for this project](docs/CONTRIBUTING.md)
GitHub transformará de manera automática el enlace relativo o la ruta de imagen en cualquier rama en la que te encuentres actualmente, de modo que el enlace o ruta siempre funcione. Puedes usar todos los operandos del enlace relativo, como ./ y ../.
Los enlaces relativos son más sencillos para los usuarios que clonan tu repositorio. Puede que los enlaces absolutos no funcionen en los clones de tu repositorio. Recomendamos usar enlaces relativos para consultar los archivos dentro de tu repositorio.
Imágenes
You can display an image by adding ! and wrapping the alt text in [ ]. Entonces encierra el enlace de la imagen entre paréntesis ().
![Esta es una imagen](https://myoctocat.com/assets/images/base-octocat.svg)
 
GitHub es compatible con incrustar imágenes en tus propuestas, solicitudes de cambio, debates, comentarios y archivos .md. Puedes mostrar una imagen desde tu repositorio, agregar un enlace a una imagen en línea o cargar una imagen. 

Tip: Cuando quieras mostrar una imagen que esté en tu repositorio, deberías utilizar enlaces relativos en vez de absolutos.
Aquí tienes algunos ejemplos para utilizar enlaces relativos para mostrar una imagen.
Contexto	Enlace Relativo
En un archivo .md en la misma rama	/assets/images/electrocat.png
En un archivo .md en otra rama	/../main/assets/images/electrocat.png
En propuestas, solicitudes de cambio y comentarios del repositorio	../blob/main/assets/images/electrocat.png
En un archivo .md en otro repositorio	/../../../../github/docs/blob/main/assets/images/electrocat.png
En propuestas, solicitudes de cambios y comentarios de otro repositorio	../../../github/docs/blob/main/assets/images/electrocat.png?raw=true
Nota: Los últimos dos enlaces relativos en la tabla anterior funcionarán únicamente para las imágenes en repositorios privados solo si el lector tiene por lo menos acceso de lectura a este.
Especificar un tema en el que se muestra una imagen
Puedes especificar el tema en el cual se muestra una imagen si agregas #gh-dark-mode-only o #gh-light-mode-only al final de la URL de una imagen en lenguaje de marcado.
Distinguimos entre modos de color oscuro y claro, así que existen dos opciones disponibles. Puedes utilizar estas opciones para mostrar imágenes optimizadas para los fondos claros u oscuros. Esto es especialmente útil para las imágenes PNG transparentes.
Contexto	URL
Tema oscuro	![GitHub Brillante](https://github.com/github-light.png#gh-dark-mode-only)
Tema claro	![GitHub Oscuro](https://github.com/github-dark.png#gh-light-mode-only)
Listas
Puedes realizar una lista desordenada al anteceder una o más líneas de texto con - o *.
- George Washington
- John Adams
- Thomas Jefferson
 
Para ordenar tu lista, antecede cada línea con un número.
1. James Madison
2. James Monroe
3. John Quincy Adams
 
Listas anidadas
Puedes crear una lista anidada al dejar sangría en uno o más elementos de la lista debajo de otro elemento.
Para crear una lista anidada mediante el editor web en GitHub o un editor de texto que usa una fuente monoespaciada, como Atom, puedes alinear tu lista visualmente. Escribe los caracteres con espacio frente a tu elemento de la lista anidada hasta que el carácter del marcador de lista (- or *) se encuentre directamente debajo del primer carácter del texto en el elemento que se encuentra por debajo.
1. Primer elemento de la lista
   - Primer elemento de la lista anidado
     - Segundo elemento de la lista anidado
 
 
Para crear una lista anidada en el editor de comentarios en GitHub, que no usa una fuente monoespaciada, puedes observar el elemento de la lista inmediatamente anterior a la lista anidada y contar el número de caracteres que aparecen antes del contenido del elemento. Luego escribe ese número de caracteres de espacio frente al elemento de la lista anidada.
En este ejemplo, puedes agregar un elemento de la lista anidada debajo del elemento de la lista 100. Primer elemento de la lista con una sangría mínima de cinco espacios para el elemento de la lista anidada, dado que hay cinco caracteres (100.) antes del Primer elemento de la lista.
100. Primer elemento de la lista
     - Primer elemento de la lista anidada
 
Puedes crear múltiples niveles de listas anidadas mediante el mismo método. Por ejemplo, ya que el primer elemento de la lista anidada tiene siete caracteres (␣␣␣␣␣-␣) antes del contenido First nested list item de la misma, necesitarás colocar sangría de siete espacios en el segundo elemento de esta.
100. Primer elemento de la lista
     - Primer elemento de la lista anidada
       - Segundo elemento de la lista anidada
 
# Listas de tareas
Para crear una lista de tareas, lista los elementos por prefacio con un guion y espacio, seguido de [ ]. Para marcar una tarea como completada, utiliza [x].
- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:
 
If a task list item description begins with a parenthesis, you'll need to escape it with \:
- [ ] \(Optional) Abre una propuesta de seguimiento
Mencionar personas y equipos
Puedes mencionar a una persona o equipo en GitHub al escribir @ más el nombre de usuario o el nombre del equipo. Esto activará una notificación y llamará su atención hacia la conversación. Las personas también recibirán una notificación si editas un comentario para mencionar su nombre de usuario o el nombre del equipo. 
@github/support ¿Qué piensas sobre estas actualizaciones?
 
Cuando mencionas a un equipo padre, los miembros de los equipos hijo también reciben notificaciones, simplificando la comunicación con múltiples grupos de personas. 
Si escribes un símbolo @ aparecerá una lista de personas o equipos en el proyecto. La lista filtra a medida que escribes, por lo que una vez que escribes el nombre de la persona o del equipo que estás buscando, puedes usar las teclas de flecha para seleccionarlos y presionar cada pestaña para ingresar para completar el nombre. En el caso de los equipos, escribe el nombre de la @organización/equipo y todos los miembros del equipo que se suscribirán a la conversación.
Los resultados autocompletados se restringen a los colaboradores del repositorio y a otros participantes en el hilo.
Hacer referencia a propuestas y solicitudes de extracción
Puedes mencionar una lista de las propuestas y las solicitudes de extracción sugeridas dentro del repositorio al escribir #. Escribe el número o el título de la propuesta o la solicitud de extracción para filtrar la lista, y luego presiona cada pestaña o ingresa para completar el resultado resaltado.
Hacer referencia a recursos externos
Si se configuran las referencias autovinculadas personalizadas para un repositorio, entonces las referencias a recursos externos, como un informe de problemas de JIRA o un ticket de Zendesk, se convertirán en vínculos acortados. Para saber qué autovínculos se encuentran disponibles en tu repositorio, contacta a alguien con permisos administrativos sobre el mismo. 
Cargar activos
Puedes cargar activos como imágenes si las arrastras y sueltas, las seleccionas de un buscador de archivos o si las pegas. Puedes cargar activos a las propuestas, solicitudes de cambios, comentarios y archivos .md en tu repositorio.
Usar emojis
Puedes agregar emojis a tu escritura al escribir :EMOJICODE:.
@octocat :+1: This PR looks great - it's ready to merge! :shipit:
 
Si escribes : aparecerá una lista con los emojis sugeridos. La lista filtrará a medida que escribes; por lo tanto, una vez que encuentres el emoji que estás buscando, presiona Tab (Tabulador) o Enter (Intro) para completar el resultado resaltado.
Párrafos
Puedes crear un nuevo párrafo al dejar una línea en blanco entre las líneas de texto.
Notas al pie
Puedes agregar notas al pie para tu contenido si utilizas esta sintaxis de corchetes:
Esta es una nota al pie sencilla[^1].

A footnote can also have multiple lines[^2].  

You can also use words, to fit your writing style more closely[^note].

[^1]: Mi referencia.
[^2]: Every new line should be prefixed with 2 spaces.  
  This allows you to have a footnote with multiple lines.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.  
    This footnote also has been made with a different syntax using 4 spaces for new lines.
La nota al pie se verá así:
 
Notae: La posición de una nota al pie en tu archivo con lenguaje de marcado no influencia la nota al pie que se interpretará. Puedes escribir una nota al pie después de referenciarla y esta aún se interpretará en la parte inferior del archivo con lenguaje de marcado.
Ocultar el contenido con comentarios
Puedes decirle a GitHub que oculte el contenido del lenguaje de marcado interpretado colocando el contenido en un comentario de HTML.
<!-- This content will not appear in the rendered Markdown -->
Importar formato de Markdown
You can tell GitHub to ignore (or escape) Markdown formatting by using \ before the Markdown character.
Cambiemos el nombre de \*our-new-project\* a \*our-old-project\*.
 
Inhabilitar la representación del lenguaje de marcado
Cuando ves un archivo de lenguaje de marcado, puedes hacer clic en el  en la parte superior de este para inhabilitar la representación de lenguaje de marcado y ver en su lugar el código fuente del archivo.
 
El inhabilitar la interpretación de lenguaje de marcado te permite utilizar las características de vista de código fuente, tales como el enlazado de líneas, el cual no es posible cuando se está viendo un archivo interpretado en lenguaje de marcado.


