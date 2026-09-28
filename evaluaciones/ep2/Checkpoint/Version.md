# Versión Preliminar del Modelo de Datos

Para soportar la navegación relacional y el almacenamiento estructurado (utilizando datos ficticios y sintéticos), el MVP trabajará con las siguientes entidades principales y sus relaciones:

**Entidad: Proyecto**
* `id_proyecto` (Int, Primary Key)
* `titulo` (String)
* `descripcion_breve` (String)
* `area_tematica` (String)
* `ano_ejecucion` (Int)
* `estado_proyecto` (String)
* `url_imagen` (String)

**Entidad: Integrante**
* `id_integrante` (Int, Primary Key)
* `nombre_completo` (String)
* `rol_cargo` (String)
* `organizacion_asociada` (String)

**Entidad Relacional: Proyecto_Integrante**
* `id_relacion` (Int, Primary Key)
* `id_proyecto` (Int, Foreign Key)
* `id_integrante` (Int, Foreign Key)