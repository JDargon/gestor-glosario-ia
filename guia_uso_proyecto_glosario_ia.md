# Guía de uso del Proyecto: Glosario de inteligencia artificial

Este proyecto sirve para crear, revisar y mantener de forma colaborativa un glosario de términos relacionados con la inteligencia artificial en formato Markdown.

El archivo principal del glosario es:

`glosario_ia_inicial.md`

Este archivo se considera la fuente de verdad del proyecto. Las nuevas entradas no se añaden directamente al archivo hasta que hayan sido propuestas, revisadas y consolidadas.

## Estructura del proyecto

El proyecto está organizado en cuatro chats principales:

* `00 - Comprobación de instrucciones`
* `01 - Propuestas de nuevas entradas`
* `02 - Revisión y duplicados`
* `03 - Glosario consolidado`

Cada chat tiene una función concreta dentro del flujo de trabajo.

## 00 - Comprobación de instrucciones

Este chat se usa para comprobar que el proyecto está utilizando correctamente el archivo principal y las instrucciones.

Sirve para verificar:

* cuántas entradas tiene el glosario;
* si una entrada concreta ya existe;
* si hay encabezados `###`;
* si la estructura sigue siendo uniforme;
* si el archivo activo en Fuentes es el correcto.

Ejemplo de uso:

```text
/CONTAR

Comprueba el archivo principal `glosario_ia_inicial.md`.

Indica:
1. Cuántas entradas contiene.
2. Si existe una entrada concreta.
3. Si hay algún encabezado `###`.
4. Si la estructura sigue siendo uniforme.
```

## 01 - Propuestas de nuevas entradas

Este chat se usa para proponer nuevos términos candidatos.

El usuario solo tiene que escribir uno o varios términos, sin necesidad de dar explicaciones largas.

Ejemplo con un solo término:

```text
Prompt
```

Ejemplo con varios términos:

```text
MCP
Autoprompting
Skill
Conector
```

El chat debe comprobar si cada término ya existe en `glosario_ia_inicial.md`, si aparece como variante, traducción o concepto equivalente, y decidir si conviene:

* crear una entrada nueva;
* ampliar una entrada existente;
* rechazar por duplicado;
* dejar pendiente de revisión.

Si procede crear una entrada, el chat genera una propuesta en Markdown.

Al final de la respuesta debe aparecer siempre un bloque llamado:

```text
Pendientes para revisión:
- Término 1
- Término 2
```

Ese bloque sirve para que el chat `02` pueda revisar las propuestas sin que el usuario tenga que copiar textos largos.

## 02 - Revisión y duplicados

Este chat se usa para revisar las entradas candidatas antes de incorporarlas al glosario.

Normalmente basta con escribir:

```text
/revisar
```

El chat intentará tomar el último bloque `Pendientes para revisión` generado en el chat `01`.

Si no lo encuentra, pedirá que se pegue solo la lista corta de pendientes, por ejemplo:

```text
Pendientes para revisión:
- MCP / Model Context Protocol
- Autoprompting
- Skill / habilidad
```

El chat revisa cada término, comprueba duplicados, corrige redacción y decide un estado:

* Aprobada
* Revisada
* Rechazada por duplicado
* Integrada en otra entrada
* Pendiente de revisión

Las entradas con estado `Revisada` o `Aprobada` pueden pasar al chat `03` para incorporarse al archivo principal.

## 03 - Glosario consolidado

Este chat se usa para generar una nueva versión completa del archivo Markdown.

Solo debe utilizarse cuando una o varias entradas ya hayan sido revisadas en el chat `02`.

La consolidación debe:

* mantener todas las entradas existentes;
* añadir solo las entradas revisadas;
* no eliminar ni resumir entradas anteriores;
* no usar subsecciones `###`;
* conservar la estructura uniforme;
* ordenar las entradas alfabéticamente;
* indicar cuántas entradas había antes y cuántas hay después;
* devolver el Markdown completo actualizado.

Ejemplo de petición:

```text
Incorpora estas entradas revisadas al archivo principal `glosario_ia_inicial.md`.

Mantén todas las entradas existentes.
No elimines ni resumas ninguna.
No uses subsecciones `###`.
Conserva la estructura uniforme con encabezados `##`.
Ordena alfabéticamente todas las entradas.
Indica cuántas entradas había antes y cuántas habrá después.
Devuelve el Markdown completo actualizado.

Entradas revisadas para incorporar:

[pegar aquí las entradas revisadas]
```

## Sustitución del archivo principal

El archivo `.md` no se actualiza automáticamente en Fuentes.

Cuando el chat `03` genera una nueva versión consolidada:

1. Descargar el archivo actualizado.
2. Renombrarlo como:

```text
glosario_ia_inicial.md
```

3. Ir al proyecto.
4. Entrar en la pestaña `Fuentes`.
5. Quitar la versión anterior del archivo.
6. Subir la nueva versión.
7. Comprobar en `00 - Comprobación de instrucciones` que el archivo nuevo está activo.

## Formato obligatorio de las entradas

Todas las entradas principales deben usar encabezado de segundo nivel:

```markdown
## Término principal / equivalente o explicación en español si procede
```

Después debe ir la definición en uno o varios párrafos breves.

Ejemplo:

```markdown
## Vibe coding / programación por conversación con IA

Práctica de desarrollo de software en la que una persona construye o modifica código dando instrucciones en lenguaje natural a una herramienta de IA.

El vibe coding puede ser útil para prototipar o explorar ideas, pero requiere revisión humana.
```

## Normas de estilo

Las entradas deben:

* estar escritas principalmente en español;
* mantener el término inglés cuando sea el más habitual;
* evitar traducciones artificiales;
* explicar qué es el concepto y para qué sirve;
* diferenciar conceptos relacionados sin duplicarlos;
* evitar fechas, porcentajes o atribuciones personales innecesarias;
* no incluir enlaces ni bibliografía dentro de la entrada salvo que se decida cambiar el criterio del glosario;
* mantener un nivel de detalle parecido al resto del archivo.

## Normas de estructura

El glosario debe mantener una estructura uniforme:

* un único título principal `# Glosario de inteligencia artificial`;
* cada entrada principal con `##`;
* no usar subsecciones `###`;
* no duplicar entradas equivalentes;
* mantener orden alfabético;
* conservar todas las entradas válidas en cada consolidación.

## Flujo resumido

El flujo normal de trabajo es:

```text
01 - Propuestas
↓
02 - Revisión y duplicados
↓
03 - Glosario consolidado
↓
Actualizar archivo en Fuentes
↓
00 - Comprobación
```

## Estado actual del glosario

El número de entradas puede cambiar con cada consolidación.

Para conocer el estado actual del glosario, debe comprobarse siempre el archivo principal:

`glosario_ia_inicial.md`

El conteo debe hacerse contando los encabezados `##` del archivo principal.

La guía no debe usarse como fuente de verdad para el número de entradas, porque puede quedar desactualizada después de nuevas incorporaciones.

## Fase futura

Cuando este flujo esté suficientemente probado, se podrá crear un GPT personalizado llamado, por ejemplo:

`Gestor de glosario IA`

Ese GPT podrá unificar las funciones de propuesta, revisión y consolidación en un solo asistente.

Más adelante, una fase avanzada podría conectar el GPT con un repositorio de GitHub mediante API para consultar el glosario, crear ramas, proponer cambios y abrir pull requests.
