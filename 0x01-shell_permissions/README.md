¿Por qué usamos #!/bin/bash al principio de nuestro script?

Esto se debe a que es necesario permitir que el shell interactivo sepa qué tipo de intérprete ejecutar para el programa que contiene. La primera línea le dice a Unix que el archivo será ejecutado por /bin/bash.  Esta es la ubicación estándar del shell Bourne en casi todos los sistemas Unix. Al agregar #!/bin/bash como la primera línea de tu script, le indicas al sistema operativo que invoque el shell especificado para ejecutar los comandos que siguen en el script. #! a menudo se lo conoce como "hash-bang", "she-bang" o "sha-bang". Sin embargo, solo se ejecutará si llamas tu script como un ejecutable. Por ejemplo, cuando escribes ./nombre-del-scrip.extension, el sistema buscará en la línea superior del  archivo para determinar el intérprete, mientras que, al ejecutar el script como bash nombre_del_script.sh, la primera línea se ignorará

0x01. Shell, permissions
Tasks

0. My name is Betty
Create a script that switches the current user to the user betty.

You should use exactly 8 characters for your command (+1 character for the new line)
You can assume that the user betty will exist when we will run your script

1. Who am I
mandatory
Write a script that prints the effective username of the current user.

2. Groups
mandatory
Write a script that prints all the groups the current user is part of.
Note: depending on the user, you will get a different output.

3. New owner
mandatory
Write a script that changes the owner of the file hello to the user betty.

4. Empty!
mandatory
Write a script that creates an empty file called hello.

5. Execute
mandatory
Write a script that adds execute permission to the owner of the file hello.

The file hello will be in the working directory

6. Multiple permissions
mandatory
Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

The file hello will be in the working directory

7. Everybody!
mandatory
Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello

The file hello will be in the working directory
You are not allowed to use commas for this script


8. James Bond
mandatory
Write a script that sets the permission to the file hello as follows:

Owner: no permission at all
Group: no permission at all
Other users: all the permissions
The file hello will be in the working directory You are not allowed to use commas for this script

9. John Doe
mandatory
Write a script that sets the mode of the file hello to this:

-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
The file hello will be in the working directory
You are not allowed to use commas for this script

10. Look in the mirror
mandatory
Write a script that sets the mode of the file hello the same as olleh’s mode.

The file hello will be in the working directory
The file olleh will be in the working directory
Note: the mode of olleh will not always be 664. Make sure your script works for any mode.

11. Directories
mandatory
Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.

12. More directories
mandatory
Create a script that creates a directory called my_dir with permissions 751 in the working directory.

13. Change group
mandatory
Write a script that changes the group owner to school for the file hello

The file hello will be in the working directory

