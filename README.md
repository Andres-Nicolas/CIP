# DATA SCIENCE
<h1>Comandos Básicos de Git</h1>

<p>Esta es una lista de los comandos más comunes y útiles para trabajar con Git, incluyendo configuraciones básicas y tareas habituales.</p>

<h2>Configuración Básica de Git</h2>
<pre>
<code>
git config --global user.name "Tu Nombre"    # Configura tu nombre de usuario
git config --global user.email "tuemail@ejemplo.com"    # Configura tu correo electrónico
git config --global core.autocrlf true    # Convierte finales de línea automáticamente (Windows)
git config --global core.autocrlf input    # Convierte finales de línea automáticamente (macOS/Linux)
git config --list    # Muestra la configuración actual
</code>
</pre>

<h2>Inicialización y Configuración</h2>
<pre>
<code>
git init    # Inicializa un repositorio Git
git clone <url_del_repositorio>    # Clona un repositorio existente
</code>
</pre>

<h2>Seguimiento de Cambios</h2>
<pre>
<code>
git status    # Muestra el estado del repositorio
git add .    # Añade todos los archivos al área de preparación (stage)
git add <archivo>    # Añade un archivo específico al área de preparación
git commit -m "Mensaje del commit"    # Guarda los cambios en el repositorio
git commit -am "Mensaje del commit"    # Añade y guarda cambios en un solo paso
</code>
</pre>

<h2>Historial y Diferencias</h2>
<pre>
<code>
git log    # Muestra el historial de commits
git log --oneline    # Muestra el historial resumido (una línea por commit)
git diff    # Muestra diferencias entre cambios locales y el último commit
</code>
</pre>

<h2>Trabajo con Ramas</h2>
<pre>
<code>
git branch <nombre_rama>    # Crea una nueva rama
git checkout <nombre_rama>    # Cambia a una rama existente
git checkout -b <nombre_rama>    # Crea y cambia a una nueva rama
git branch -d <nombre_rama>    # Elimina una rama
</code>
</pre>

<h2>Sincronización con Remoto</h2>
<pre>
<code>
git remote add origin <url_del_repositorio>    # Agrega un repositorio remoto
git push origin <nombre_rama>    # Envía cambios al remoto
git push -u origin main    # Configura y envía cambios a la rama principal
git pull origin <nombre_rama>    # Obtiene y fusiona cambios desde remoto
git fetch origin    # Obtiene cambios desde remoto sin fusionarlos
</code>
</pre>

<h2>Revertir o Corregir Cambios</h2>
<pre>
<code>
git reset <archivo>    # Saca un archivo del área de preparación
git reset --soft HEAD~1    # Revierte el último commit manteniendo los cambios
git reset --hard HEAD~1    # Revierte el último commit y elimina los cambios
git revert <id_commit>    # Crea un commit para deshacer uno anterior
</code>
</pre>
