# TypeScript III - Leccion II - Task 1

## Union Types

1. En tus palabras. Define qué es un Union Type

- Es la forma en la que le decimos a TypeScript que **un valor** puede **ser de uno o más tipos** (dependiendo de la complejidad del Union Type).

2. ¿Qué clase de métodos se puede usar directamente sobre un Union Value?

- Union type al ser la **unión** de 2 o más tipos, solo se puede acceder a los métodos que están en la **intersección** del **conjunto de todos los miembros**. Por ejemplo: una función la cuál recibe un Union Value:`string[] | string` puede acceder al método `.slice()` de ese valor ya que tanto un **array** como un **string** tienen ese método en su prototipo.

3. ¿Cómo se llama el proceso de verificar el tipo concreto de un Union Type para así usarlo como ese tipo en específico?

- El proceso es conocido como `Narrowing`. Consiste en validar el tipo de dato a través de un condicional. Así, TypeScript sabrá que métodos o propiedades **en específico** pueden usarse con cada tipo.
