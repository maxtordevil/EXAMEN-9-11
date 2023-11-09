**PREGUNTAS DE DESARROLLO**

* ¿Cómo la programación orientada a objetos difiere de la programación procedimental?

La programación orientada a objetos (OOP) y la programación procedimental son dos paradigmas de programación diferentes.

La programación Procedimental: En este paradigma, el enfoque está en las funciones o procedimientos para realizar tareas. Los datos y las funciones son entidades separadas. Un programa procedimental es básicamente una lista de instrucciones que le dicen a la computadora qué hacer paso a paso. Un claro y cercano ejemplo sería el lenguaje C.
Programación Orientada a Objetos (OOP): En OOP, el enfoque está en los objetos y sus interacciones. Un objeto es una entidad que combina datos y las funciones que operan en esos datos. OOP permite conceptos como la herencia (donde un "objeto hijo" puede heredar características de un "objeto padre"), el polimorfismo (donde una interfaz única puede representar diferentes tipos de objetos), y el encapsulamiento (donde los detalles de implementación de un objeto están ocultos). C++ y Java son ejemplos de lenguajes de programación orientados a objetos.

La diferencia principal entre la programación procedimental y la OOP es que la programación procedimental se centra en las funciones, mientras que la OOP se centra en los objetos que combinan datos y funciones.

  ¿Cómo C++ brinda soporte para ambos paradigmas?

Esto se debe a que C++ es una extensión del lenguaje C del cual hereda todas las características de la programación procedimental de este y además introduce conceptos como clases, objetos, herencia, polimorfismo y encapsulamiento, que son fundamentales para la programación orientada a objeto,por lo tanto, C++ permite a los programadores elegir el paradigma que mejor se adapte a sus necesidades para un problema particular.



* ¿Qué es la programación de una excepción?

 La programación de excepciones es un método de manejo de errores que se utiliza en muchos lenguajes de programación modernos. Una "excepción" es un evento que ocurre durante la ejecución de un programa que interrumpe el flujo normal de las instrucciones del programa.


* ¿Qué ocurre si una excepción lanzada no es capturada por ningún bloque catch?

Si una excepción lanzada en C++ no es capturada por ningún bloque `catch`, el programa terminará abruptamente y se llamará a la función `std::terminate()`. Esta función, por defecto, llama a `abort()` para terminar el programa.

Además, antes de que se llame a `std::terminate()`, si existe, se llamará a la función `std::unexpected()`. Esta función puede ser personalizada por el programador para manejar excepciones no capturadas de una manera específica.

                     
* ¿Qué se entiende por “Adquisición de Recursos” en el contexto del C++?

 "Adquisición de Recursos" en el contexto de C++ generalmente se refiere a la práctica de adquirir recursos, como memoria, archivos, conexiones de red, etc., en el momento de la creación de un objeto. Esto se hace a menudo en el constructor de una clase.
Cuando un objeto se crea, adquiere el recurso durante la inicialización (por lo tanto, "la adquisición de recursos es la inicialización"). Cuando el objeto se destruye, libera el recurso en su destructor. Esto asegura que los recursos se limpien adecuadamente incluso si se produce una excepción, lo que ayuda a prevenir las fugas de recursos.

¿Por qué es importante y como se relaciona con la gestión  de excepciones?

La "Adquisición de Recursos es Inicialización" (RAII) es un patrón de diseño en C++ que está intrínsecamente relacionado con la gestión de excepciones. 

Cuando se lanza una excepción, el flujo de control del programa cambia, y puede ser difícil asegurarse de que se liberen correctamente todos los recursos que se han adquirido hasta ese punto. Sin embargo, si se utiliza el patrón RAII, los recursos se liberan automáticamente cuando los objetos que los poseen son destruidos debido al desenrollado de la pila que ocurre cuando se lanza una excepción.

Por lo tanto, el patrón RAII ayuda a prevenir las fugas de recursos y hace que el código sea más seguro y más robusto frente a las excepciones. Es una de las razones por las que las excepciones son una característica tan poderosa en C++, ya que permiten manejar errores de manera limpia y eficiente sin tener que verificar constantemente los códigos de error y liberar manualmente los recursos.

**PREGUNTAS DE OPCIÓN MÚLTIPLE**
_C++ es un lenguaje de programación ampliamente utilizado que ha evolucionado a lo largo de los años. ¿Cuáles de las siguientes opciones describen correctamente las características centrales de C++?_

d. Todas las anteriores

_Durante el proceso de desarrollo, a menudo es necesario compilar y enlazar múltiples archivos. En este contexto, ¿qué es un archivo makefile?_

b. Un archivo que ayuda a gestionar y automatizar la compilación de proyectos de programación


_En C++, las variables pueden referirse a datos o direcciones de memoria. En relación a esto, ¿qué son los punteros en la programación C++?_

b. Variables que almacenan la dirección de otra variable
