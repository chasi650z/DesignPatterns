# DesignPatterns

Diseño de Solución: Mejorando la Implementación del Aplicativo de Automóviles en Codificando Con Patrones Cía. Ltda.

1. Corrección del Patrón Repositorio:

Pepito debe abordar el problema reportado por el equipo de QA en la implementación del patrón repositorio. Antes de solucionar este problema, es crucial establecer un método para probar la funcionalidad sin depender de la base de datos.

a. Implementación de Repositorio en Memoria:

Crear una implementación de repositorio en memoria que simule las operaciones CRUD sin interactuar con la base de datos. Esto permitirá a Pepito probar la funcionalidad del sistema sin depender de una base de datos completa.

2. Patrón de Diseño para Propiedades por Defecto:

Pepito debe diseñar un patrón que permita agregar propiedades por defecto a los vehículos de manera flexible y que minimice los cambios en el código para futuras adiciones.

a. Patrón Decorator:

Utilizar el patrón Decorator para agregar propiedades adicionales a los vehículos de manera dinámica. Cada propiedad adicional se implementará como un decorador independiente.

b. Diseño Flexible:

Cada propiedad adicional se encapsulará en su propio decorador, permitiendo que nuevas propiedades se agreguen fácilmente sin modificar el código existente. Esto asegura que los cambios mínimos sean necesarios para el próximo sprint.

3. Implementación del Factory Method para Nuevos Modelos:

Para abordar la futura adición de nuevos modelos de automóviles, el arquitecto sugiere la implementación del patrón Factory Method.

a. Factory Method:

Crear una interfaz común llamada CarFactory que define un método para la creación de nuevos modelos. Cada modelo específico, como Escape, implementará esta interfaz y proporcionará su propia lógica de creación.

b. Flexibilidad para Nuevos Modelos:

La implementación del Factory Method permitirá que se añadan nuevos modelos en el futuro sin modificar el código existente. Cuando se introduce un nuevo modelo, simplemente se crea una nueva clase que implementa la interfaz CarFactory.
