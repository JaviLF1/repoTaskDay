

# Clases principales y comportamientos

## DayMonYear


Esta clase se encarga de recibir y almacenar los datos dentro del código de día, mes, año , título, descripción.

<img width="292" height="242" alt="image" src="https://github.com/user-attachments/assets/856e56cc-67e0-43ba-8933-e60e458c1d14" />


## Task
Esta es una clase hija de DayMonYear, esta clase tiene el agregado de guardar esta información en un archivo .txt, además de tener una función para borrar la información del archivo
y su última función es la de leer todos los archivos para crear objetos de todo lo guardado, esto para poder acceder a la información despues de cerrar y abrir el programa 

<img width="543" height="548" alt="image" src="https://github.com/user-attachments/assets/16a507cf-c969-4de4-b9c0-0676990966fd" />


# Cómo soluciona el problema

Primero rompí el problema en 2, la fecha y el archivo, aprovechando las herencias primero crear la clase DayMonYear, que al tener string decidí usar referencias para pasar esta informacion, ya que evita el tener que hacer una copia que puede ser muy grande y tardada para cada std::string,
Después pasé la clase DayMonYear como padre de la segunda clase Task, esta clase se encarga de registrar la información en un .txt, para crear este objeto hay 2 opciones, rellenarlo en código o rellenarlo usando el .txt, aquí usé sobrecarga de funciones para que ambas fueran constructores,
Pero una está definida por los datos y la otra por el .txt.


# Diagrama UML


<img width="1819" height="4140" alt="Task Management Model-2026-06-13-045642" src="https://github.com/user-attachments/assets/b2460c69-4f6e-49ef-bf06-177d11e9045e" />


# Test
Aqui podemos ver como al crear 3 objetos Task, genera los archivos .txt guardando los del mismo dia juntos y el diferente en su propio archivo con su fecha


<img width="2559" height="1391" alt="image" src="https://github.com/user-attachments/assets/5b39e90c-e18f-4ee4-8783-ec2e4a5e1679" />



Y en esta segunda parte vemos como lee los archivos ya existentes y nos permite ver su informacion creando nuevos objetos Task
<img width="1991" height="1294" alt="image" src="https://github.com/user-attachments/assets/bca771c0-2010-424f-82f8-527de426f11b" />


# Error detection

Esta parte es la que se encarga de validar que la fecha es posible y no aceptar fechas como 42/06/2026, esto con mi funcion check()

<img width="1861" height="880" alt="image" src="https://github.com/user-attachments/assets/8cfabd4e-c40a-42cf-9b8b-23ca0b06ec86" />

