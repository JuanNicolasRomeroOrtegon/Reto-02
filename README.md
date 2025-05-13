# Reto-02

Presento un diagrama UML que modela el sistema de transporte público de Bogotá: TransMilenio. Represento las entidades principales del sistema, sus características y comportamientos (atributos y métodos), así como las relaciones que existen entre ellas (composición y herencia)
Abstraigo los elementos que componen el sistema de Transmilenio y muestro como se comportan ellos entre sí.

## Descripción general

El sistema está compuesto por varias clases que interactúan entre ellas para representar el transporte público:

- Transmilenio es la clase principal del sistema. Tiene elementos que son: estaciones, buses, funcionarios, usuarios, rutas y horarios.

- Las estaciones contienen componentes que son puertas anticolados, torniquetes, taquillas y puentes peatonales.

- Los buses tienen atributos como placa, tipo (troncal, alimentador, SITP, etc.) y capacidad. Cada bus sigue una ruta y opera según un horario específico.

- Las rutas definen el trayecto que sigue un bus a través de una serie de estaciones.

- Los horarios indican los días y la frecuencia con la que circulan los buses.
  
- Tipos de funcionarios que trabajan el sistema:
  - Guardias: vigilan las estaciones, atienden consultas y pitan.
  - Taquilleros: procesan pagos y atienden a los usuarios.
  - Encargados de limpieza: realizan el aseo.
  - Policías: se encargan de asegurar el orden.

- Los usuarios están clasificados en dos tipos:
  - Regulares: tienen su saldo en la tarjeta y pagan el pasaje.
  - Irregulares: evaden el pasaje.
  - 
## Relaciones principales

- Composición:
  - Transmilenio se compone de estaciones, buses, funcionarios, usuarios, rutas y horarios.
  - Las estaciones tienen elementos físicos como puertas, torniquete, taquilla y puente peatonal.

- Herencia:
  - Funcionarios es una clase base de donde se heredan los guardias, los taquilleros, el personal de limpieza y los policías.
  - Los usuarios regulares e irregulares se heredan de Usuarios.

- Relaciones:
  - Las estaciones están relacionadas con las rutas.
  - Los buses siguen rutas y se rigen por horarios.
  - Las estaciones son usadas por los usuarios y supervisadas por los funcionarios.

