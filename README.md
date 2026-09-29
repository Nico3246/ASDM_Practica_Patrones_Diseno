# Práctica ASDM — Patrones de Diseño en Java

Práctica académica desarrollada en **Java** para trabajar de forma aplicada varios **patrones de diseño orientados a objetos** dentro de un pequeño sistema de gestión de personajes y ejércitos.

El objetivo del proyecto es didáctico: practicar la identificación, implementación e integración de distintos patrones dentro de una misma aplicación de consola.

## Contexto académico

Este repositorio corresponde a una práctica universitaria del curso **2025/26**. No pretende ser una aplicación de producción ni un proyecto profesional independiente, sino una implementación enfocada al aprendizaje de patrones de diseño.

## Patrones implementados

El proyecto integra los siguientes patrones:

- **Factory Method**  
  Creación de distintos tipos de personajes mediante creadores concretos, como guerreros, arqueros y magos.

- **Prototype**  
  Clonación de personajes existentes a partir de objetos ya creados.

- **Composite**  
  Representación de ejércitos que pueden estar formados por personajes y por otros ejércitos.

- **Observer**  
  Gestión de eventos relacionados con la muerte de personajes y la actualización de elementos dependientes.

- **Iterator**  
  Recorrido y gestión de colecciones de personajes mediante distintos iteradores.

- **Decorator**  
  Ampliación dinámica de las características de los personajes, por ejemplo mediante la incorporación de armas.

- **Facade**  
  La clase `FacadeJuego` centraliza el acceso a las distintas funcionalidades del sistema y presenta un menú principal al usuario.

## Funcionamiento general

La aplicación se ejecuta por consola. Al iniciarse, se cargan varios personajes de ejemplo y se muestra un menú con operaciones como:

1. Crear un personaje.
2. Clonar un personaje.
3. Crear un ejército.
4. Gestionar la muerte de un personaje.
5. Listar personajes.
6. Subir de nivel.
7. Añadir armas.
8. Salir.

Cada una de estas operaciones sirve como caso práctico para uno o varios patrones de diseño.

## Estructura principal

El código fuente se encuentra en:

```text
src/practica_2025_26/
```

Entre las clases principales se encuentran:

- `Practica_2025_26`: punto de entrada de la aplicación.
- `FacadeJuego`: fachada principal y menú de interacción.
- `PatronFactoryMethod`
- `PatronPrototype`
- `PatronComposite`
- `PatronObserver`
- `PatronIterator`
- `PatronDecorator`
- `Personaje` y sus implementaciones.
- `Ejercito`
- Clases creadoras, iteradores y decoradores asociados a cada patrón.

## Tecnologías

- **Java**
- **NetBeans**
- **Ant**, mediante el archivo `build.xml`

## Ejecución

La forma más directa de ejecutar la práctica es abrir el repositorio como proyecto de NetBeans y ejecutar la clase principal:

```text
src/practica_2025_26/Practica_2025_26.java
```

La aplicación crea una instancia de `FacadeJuego` y lanza el menú principal mediante `iniciarJuego()`.

También puede compilarse mediante Ant si se dispone de un entorno Java correctamente configurado:

```bash
ant
```

## Enfoque del proyecto

La prioridad de esta práctica es mostrar de forma clara cómo colaboran distintos patrones dentro de una misma aplicación. Por ello, algunas decisiones de diseño están orientadas a facilitar el estudio y la identificación de cada patrón más que a construir una arquitectura de producción.

## Autor

Repositorio mantenido por [Nico3246](https://github.com/Nico3246).
