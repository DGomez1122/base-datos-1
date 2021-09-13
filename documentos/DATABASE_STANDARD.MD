<!--ts-->
# Índice de Secciones
   * [Introducción](#introducción)
   * [Justificación](#justificación)
   * [Descripción del estándar](#descripción-del-estándar)
   * [Entidades](#entidades)
   * [Atributos](#atributos)
   * [Tipo de datos](#tipo-de-datos)
   * [Llaves primarias](#llaves-primarias)
   * [Llaves foráneas](#llaves-foráneas)
   * [Índices](#índices)
<!--te-->

# 
# Introducción

El presente trabajo de investigación se trata de una descripción o documentación de un estándar de nombres para la definición de esquemas de entidad relación en MySQL 8. A lo largo de la creación de la investigación encontré muchos tipos de codificación ádemas del snake case. Este estilo ha sido el elegido para la investigación donde mostrará como este se manifiesta en el formato de estándar de una base de datos.

# 
# Justificación

El estándar de nombres snake case se eligió debido a que este estilo ya se ha utilizado en otros trabajos en editores como VS code, Python, Geany. También gracias a esta investigación me ayudo a utilizar este estilo de una manera más legible como saber de otros estilos de estándares, por ejemplo el CamelCase, UpperCase. 

# 

# 
# Descripción del estándar

El estándar Snake case (or snake_case) es el proceso de escribir palabras compuestas de manera que las palabras se separen con un símbolo de subrayado o guion bajo (_) en lugar de un espacio. La primera letra suele cambiarse a minúscula. El nombre se deriva de las imágenes asociadas de guiones bajos que representan serpientes que se deslizan por el suelo entre palabras.

# 
# 
# Entidades
En la creación de entidades el estándar snake case se manifiesta de igual manera definiendo el nombre de la entidad en minúscula. 
Por ejemplo:

```bash
CREATE TABLE table_name (
    nombre_atributo1 datatype,
    nombre_atributo2 datatype,
   ....
);
```
# 
# 
# Atributos
En la creación de entidades el estándar snake case se manifiesta de igual manera definiendo el nombre del atributo en minúscula y utlizando el simbolo guión bajo (_).
Por ejemplo:

```bash
CREATE TABLE persons (
    person_id int,
    last_name varchar(255),
    first_name varchar(255),
    ....
);
```
# 
# 
# Tipo de datos

Cada columna de una tabla de base de datos debe tener un nombre y un tipo de datos.
Un desarrollador de SQL debe decidir qué tipo de datos se almacenarán dentro de cada columna al crear una tabla. El tipo de datos es una guía para que SQL comprenda qué tipo de datos se espera dentro de cada columna y también identifica cómo interactuará SQL con los datos almacenados.
Para el estándar snake case, estos no tienen una manera de escribirse, ya que son palabras preterminadas. Hay tres tipos de datos principales: cadena, numérico y fecha y hora.

Ejemplos de Cadena: char(tamño), varchar(tamaño), binary(tamaño), text(tamaño), ....

Ejemplos de Númerico: int, float, double, boolean, ...

Ejemplos de Fecha y hora: date, datetime, time, year, ...


# 
# 
# Llaves primarias

En la creación de llaves primarias el estándar snake case se usa un indicador pk para así se más fácil referenciar la llave primaria.
Por ejemplo:

```bash
CREATE TABLE persons (
    pk_person_id int,
    last_name varchar(255),
    PRIMARY KEY (pk_person_id)
);
```

# 
# 
# Llaves foráneas

En la creación de llaves foráneas el estándar snake case se usa un indicador fk para así se más fácil referenciar la llave foránea.
Por ejemplo:

```bash
CREATE TABLE persons (
    fk_person_id int,
    FOREIGN KEY (fk_person_id)
);
```

# 
# 
# Índices

En la creación de índices el estándar snake case se usa un indicador idk. Los índices se utilizan para recuperar datos de la base de datos más rápidamente que de otra manera
Por ejemplo:

```bash
CREATE INDEX idx_person
ON persons (last_name);
```

# 
