![ActividadEvaluacion-4](https://github.com/user-attachments/assets/4cc03127-2c86-4cab-a315-7cceadf2ca7d)

## Enunciado

Esta práctica consiste en la elaboración de dos proyectos en Eclipse que deberás realizar siguiendo estas pautas:

Debes crear un proyecto en Eclipse con el nombre EjercicioUF6-01 atendiendo a las especificaciones que se indican en este documento (Especificaciones para el ejercicio 1).
Debes crear otro proyecto eclipse con el nombre EjercicioUF6-02 atendiendo a las especificaciones que se indican en este documento (Especificaciones para el ejercicio 2).
Empaqueta los dos proyecto en un archivo .zip que entregarás a tu tutor junto con un documento en formato Word o PDF donde realizarás una exposición sobre lo que has ido realizando y pegarás las partes principales del código.
Especificaciones para el ejercicio 1:

Para la gestión de un centro educativo, un programa necesita contemplar las entidades profesor, alumno y administrativo, teniendo en cuenta que todos, a su vez, son personas.

1. Crea la estructura de clases que se corresponda con el siguiente diagrama: 

  ![act6_prog](https://github.com/user-attachments/assets/ad80d58f-70ee-44a4-aaa7-973bc1bdedc6)

   La clase Persona será abstracta.
   Todas las propiedades serán privadas y accesibles mediante métodos get/set.
   El método llamar() devolverá una cadena similar a esta: “Alicia Torres llamando a Carlos Robles”. Como parte de la cadena se utilizará la propiedad nombre del objeto al que se aplica y del objeto pasado como argumento.
   El método trabajar() se especializará en cada subclase para devolver una cadena que indique el tipo de tarea que realiza cada perfil de persona. Por ejemplo:
   Profesor: “El profesor Carlos Robles va a impartir su clase”. Como parte de la cadena usarás la propiedad nombre.
   Alumno: “El alumno Alicia Torres va a estudiar para el curso 1º Bachillerato”. Como parte de la cadena usarás las propiedades nombre y curso.
   Administrativo: “El administrativo Rosa Torres va a realizar estas tareas: hacer matrículas, controlar asistencia”. Como parte de la cadena utilizarás las propiedades nombre y tareas.
   Además, las clases derivadas ampliarán su especialización con métodos propios como ponerNotas(), hacerExamen() o gestionarMatricula(). Cada uno de estos métodos devolverá una cadena de este tipo:
   ponerNotas(): “El profesor Carlos Robles va a corregir los exámenes”. Como parte de la cadena tienes que utilizar la propiedad nombre.
   hacerExamen(): “El alumno Alicia Torres va a hacer su examen”. Como parte de la cadena debes utilizar la propiedad nombre.
   gestionarMatricula(): “El administrativo Rosa Torres va a gestionar una matrícula”. Como parte de la cadena utilizarás la propiedad nombre.
   Además de lo especificado en el diagrama de clases, debes sobrescribir el método toString() en cada una de las clases para que muestre toda la información posible. Puedes hacerlo de forma automática con ayuda de Eclipse (clic 
   derecho/Source/Generate toString…).
  
2. Para terminar crea la clase Principal con método main y realiza las siguientes acciones:

    Crea un objeto Profesor, un objeto Alumno y un objeto Administrativo.
    Ejecuta el método toString() sobre cada uno de ellos.
    Ejecuta el método trabajar() sobre cada uno de ellos.
    Ejecuta el método llamar(Persona p) para que el alumno llame al profesor.
    Ejecuta el método ponerNotas() del objeto Profesor.
    Ejecuta el método hacerExamen() del objeto Alumno.
    Ejecuta el método gestionarMatricula() del objeto Administrativo.


Ejemplo de ejecución:


![act6_prog2](https://github.com/user-attachments/assets/52c0c9e3-399c-42cd-af29-b3b30a7704c1)

## Especificaciones para el ejercicio 2:

Crea las clases Libro y Autor según el siguiente diagrama de clases:

![act6_prog3](https://github.com/user-attachments/assets/efe0c0bb-ad63-4cb3-8543-6239b5ac7d87)

3. Las clases Autor y Libro estarán situadas en el paquete com.itt.libreria, mientras que en la clase Principal, donde incluirás el método main, estará la raíz del proyecto.

![act6_prog4](https://github.com/user-attachments/assets/453eb217-b751-424a-8fd5-6cd8b40a83f8)

4. Cada clase debe tener su constructor con parámetros para recibir valores para todas las propiedades.
5. Todas las propiedades de ambas clases deben ser privadas y accesibles mediante métodos get/set.
6. El método toString() de ambas clases deberá devolver una cadena de texto con el estado del objeto (valores de todas las propiedades). Puedes crearlo de forma automática con ayuda de Eclipse.
7. También debes crear la clase Principal, con método main, donde crearás un objeto de tipo Autor y otro objeto de tipo Libro, al que se le pasará el objeto Autor como uno de los argumentos del constructor. Realizarás las siguientes
  operaciones con el objeto Libro:
  Invoca al método toString() del nuevo objeto Libro.
  Modifica la biografía del autor a través del objeto Libro que has creado.
  Invoca al método toString() del objeto Autor que has creado de dos formas distintas: a partir de la referencia al objeto Libro y a partir de la referencia al objeto Autor que creaste.
  Modifica el valor de la propiedad genero y vuelve a invocar al método toString() para ver los cambios.

