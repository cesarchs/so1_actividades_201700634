# Actividad 1 - 201700634

## - Tipos de Kernel y sus diferencias
Un kernel, o mejor conocido como un núcleo, específicamente en la rama de la informática, no es que más que un software especial que forma parte importante del sistema operativo de cualquier ordenador. Por lo general, cuenta con la característica de que el mismo se ejecuta en un modo privilegiado, también llamado y mejor conocido como modo núcleo. Dentro de sus principales funciones, está el hecho de que facilita cualquier programa principal y necesario en el hardware del ordenador y es el encargado de gestionar cada uno de ellos para que funcionen de forma correcta.

### funciones: 
existen distintos programas cuyo acceso es bastante limitado en cuanto al hardware se refiere, pero para eso existen los núcleos: para gestionar cada uno de esos programas y decidir cuál, y cuánto tiempo, va a funcionar el mismo en el ordenador.  
El kernel no cumple sólo con las funciones antes descritas, sino que es bastante funcional y permite diversas acciones, como el hecho de que los mismos cumplen con una serie de pasos (abstracciones) que permiten que el sistema cuente con una interfaz segura y limpia.

- Kernel monolíticos:  
Este tipo de núcleo es aquel que facilita la abstracción del hardware subyacente sin importar su grado de potencia o variedad. Para realizar una comparación objetiva, estos núcleos son bastante complejos en cuanto a su manejo, siendo comparados con los próximos que vamos a observar. Hace más de veinte años, estos núcleos eran los principales en ser catalogados como obsoletos e inservibles, además de innecesarios. Sin embargo, con el tiempo han sido catalogados como mejorados e importantes, aunque no precisamente los mejores.

- Microkernel:  
Mejor conocidos como micronúcleos, estos son aquellos que son catalogados como mejores en comparación con el kernel anterior, debido a que el mismo cumple una serie de pequeñas abstracciones mucho más simples que las comúnmente observadas en el kernel monolítico, y su función principal es utilizar diversas aplicaciones para facilitar su funcionalidad. Su verdadero objetivo principal, es el de implementar estos servicios de forma separada en cuanto a la política de funcionamiento del sistema, se refiere. De este modo se busca que el núcleo funcione de maravilla y sea bastante simple y organizado de utilizar.

- Núcleos híbridos:  
Este tipo de kernel, es aquel que se considera una gran modificación del microkernel, que si bien son bastante similares en cuanto a diversas características, se diferencian debido a que este cuenta con un espacio adicional que cumple la función de permitir que el mismo se ejecute de forma mucho más rápida y funcional. Sin embargo, cualquiera de estos dos núcleos es bastante funcional, incluso los micronúcleos comunes, los cuales tienen un excelente rendimiento. Muchos de los sistemas operativos que se aplican hoy en día, cuentan con estos dos tipos de núcleos ya que ambos funcionan muy bien.

- Exonúcleos:  
Y por último, tenemos los Exonúcleos, los cuales son aquellos que si bien no cuentan con ningún tipo de abstracción, son aquellos que permiten el uso de bibliotecas. Dicho de otro modo, son núcleos que funcionan de maravilla al momento de ofrecer mucha funcionalidad, gracias a que los mismos cuentan con un acceso directo al hardware del sistema. Esto quiere decir, que gracias a esta gran característica, el desarrollador podrá ser capaz de permitir todas esas decisiones importantes en cuanto al rendimiento del sistema se refiere. Además, se caracterizan gracias a que son muy pequeños y a que esto realmente no limita su gran funcionamiento. Sin embargo, se sigue prefiriendo el uso de los dos kernel anteriores para los diversos sistemas que se utilizan hoy en día.


## - User vs Kernel Mode

Un procesador de un equipo que ejecuta Windows tiene dos modos diferentes: el modo de usuario y el modo kernel.

El procesador cambia entre los dos modos en función del tipo de código que se ejecuta en el procesador. Las aplicaciones se ejecutan en modo de usuario y los componentes principales del sistema operativo se ejecutan en modo kernel. Aunque muchos controladores se ejecutan en modo kernel, algunos controladores pueden ejecutarse en modo de usuario.

### User 
Al iniciar una aplicación en modo de usuario, Windows crea un proceso para la aplicación. El proceso proporciona a la aplicación un espacio de direcciones virtuales privado y una tabla de identificadores privados. Dado que el espacio de direcciones virtuales de una aplicación es privado, una aplicación no puede modificar los datos que pertenecen a otra aplicación. Cada aplicación se ejecuta de forma aislada y, si una aplicación se bloquea, el bloqueo se limita a esa aplicación. Otras aplicaciones y el sistema operativo no se ven afectados por el bloqueo.

Además de ser privado, el espacio de direcciones virtuales de una aplicación en modo de usuario es limitado. Un proceso que se ejecuta en modo de usuario no puede acceder a direcciones virtuales reservadas para el sistema operativo. Limitar el espacio de direcciones virtuales de una aplicación en modo de usuario impide que la aplicación modifique los datos críticos del sistema operativo, y posiblemente perjudiciales.

### Kernel Mode
Todo el código que se ejecuta en modo kernel comparte un único espacio de direcciones virtuales. Por lo tanto, un controlador en modo kernel no está aislado de otros controladores y del propio sistema operativo. Si un controlador en modo kernel escribe accidentalmente en la dirección virtual incorrecta, los datos que pertenecen al sistema operativo u otro controlador podrían verse comprometidos. Si se bloquea un controlador en modo kernel, todo el sistema operativo se bloquea.

