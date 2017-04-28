# Search Text Files Using Regular Expressions <h1> 

*Esto hay que ordenarlo:*

_El caracter " \ " es conocido como 'CARACTER DE ESCAPE'. Si justo despúes de él localizamos una expresión regular, estaremos dicendo que queremos que dicha expresión regular no sea interpretada como tal_

_(esto habrá que explicarlo mejor) Dentro de un grep:  el caracter "." significa "cualquier caracter"; el caracter " * " busca el string que precede el " * ". Si juntamos ambos, no busca nada, esto es, nos muestra todo.

     ```bash
     lcalvo@dit112:/etc/cron.frequently$ grep .* doit
     ```


## *Position anchors* <h2>

Se usan para describir la posición de la información

- **^**              **=>** Coincidencias al principio de una línea

      EXAMPLE: 

           ```bash
           lcalvo@dit112:/etc/cron.frequently$ sudo grep '^if' doit
           if ! [ -s /etc/TODO/.lock.$$ ] ; then
           if [ -s /etc/DISTRIBUTION ]; then
           ```
- **$**                 **=>** Coincidencias al final de una línea

      EXAMPLE: 

           ```bash
           lcalvo@dit112:/etc/cron.frequently$ sudo grep '\;$' doit
                   ;;
               continue ;;
              ;;
              ;;
           ``` 
- **\\<\\>**            **=>** Coincidencias con 'espacios en blanco', 'principio de línea' o 'fin de línea'

## *Characters sets* <h2>

- **\***              **=>** 

       EXAMPLE: 

                ```bash
         
                ```
- **\?**              **=>**

       EXAMPLE: 

                ```bash
         
                ```
- **\+**              **=>**

       EXAMPLE: 

                ```bash
            
                ```
- **\{n,m\}**           **=>**
     
       EXAMPLE: 

           ```bash
         
           ```
- **\|**                **=>**

       EXAMPLE: 

           ```bash
         
           ```
- **(regex\)**          **=>**

       EXAMPLE: 

           ```bash

           ```
  
## *Quantify modifiers* <h2>


