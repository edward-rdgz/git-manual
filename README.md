# Git

Git es un sistema de control de versiones muy potente y sin duda el más usado en la actualidad.

# Primeros pasos con Git y GitHub

- Configuración de variables globales

	git config --global user.name "username"

	git config --global user.email my@email.com

- Inicialización de repositorio
	
	git init

- Clonación de repositorio remoto a local
	
	git remote add origin https://github.com/username/project_name.git

	git pull origin master

- Obtención de estado(s) de archivo(s)

	git status

- Agregación de archivo

	git add filename.extesion

- Agregación de más de un archivo

	git add -A

- Perpetración de archivos locales en repositorio remoto

	git commit -m "Action message"

- Expedición de archivos a repositorio remoto

	git push origin master

# Crear alias de comandos en git

- Configuración de alias en línea de comandos

	git config --global alias.[alias] "[comando]"

	Examples:

		Commands:

			git config --global alias.alias "config --get-regexp ^alias\."
			 
			git lost
			git config --global alias.lost "fsck --full"

			git last
			git config --global alias.last "log -1 HEAD"

		Abbreviations:

			git b
			git config --global alias.b "branch"

			git st
			git config --global alias.st "status"

			git ci
			git config --global alias.ci "commit"

- Configuración de alias directamente en el fichero .gitconfig

	Example:

		b = branch

	    ci = commit

	    co = checkout

	    cob = checkout -b

	    d = diff

	    l = log

# Clone y fork con Git y GiHub

- Clonación de repositorio

	git clone https://github.com/username/project_name.git

- Bifurcación de repositorio

	git init

	git add origin master url_repositorio_github

	git pull origin master

# Flujos y zonas por las que pasa un fichero en un repositorio Git

- Zonas:
	
	HEAD

	Index or Staged Files

	Working Tree or Unstaged Files

- Reinicio o limpieza de indices

	git reset HEAD

- Haciendo una segunda expedición en una sola operación

	git commit -a -m "filename.extension, new_lines"

# Guardar y recuperar cambios con Git
















Source: https://styde.net/aprende-git/