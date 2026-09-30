# Auditoría de cumplimiento · Calculadora CSAPG

**Documento fuente:** Procediment de convocatòries internes CSAPG · ID 6455 · versión 1.0 · 10/12/2025  
**Fecha de auditoría:** 30/09/2026  
**Estado:** revisión técnica avanzada; no declarar todavía equivalencia plena con la valoración oficial.

## Conclusión de auditoría

La matriz principal de rutas, máximos y tasas está correctamente trasladada en los supuestos comprobados. Se han superado **13 comprobaciones de enrutamiento/baremo** y **15 comprobaciones de reglas transversales** del motor.

Aun así, la versión actual necesita varios ajustes antes de poder afirmar que la formulación reproduce el procedimiento con la máxima fidelidad: existen validaciones documentales que la interfaz todavía presupone y un criterio de desempate que debe separar estrictamente "formación" de investigación/docencia.

## Casos de regresión comprobados

1. Grupo 2.2 · Enfermería · área común · cambio de turno/servicio → orden por antigüedad; formación solo para desempate.
2. Grupo 2.2 · Enfermería · UCI · cambio de turno/servicio → baremo 70/30.
3. Grupo 2.2 · Enfermería · área común · incremento de jornada → baremo 60/40.
4. Grupo 2.2 · Fisioterapia · Neurología · cambio de categoría → baremo 70/30.
5. Resto de categorías Grupo 2.2 → no se inventa un baremo numérico no definido de forma inequívoca.
6. Grupo 3 · TCAI · UCI · cambio de turno/servicio → baremo 70/30.
7. Grupo 3.2 · área común · cambio de turno/servicio → antigüedad.
8. Grupo 3.2 · área común · incremento de jornada → baremo 60/40.
9. Grupos 4-7 · cambio de turno/servicio → antigüedad.
10. Grupos 4-7 · incremento de jornada/cambio de categoría → baremo 60/40.
11. SEM → control de requisito de 30 ECTS + 3 años de experiencia.
12. Grupo 3 especial → tasas literales 0,20/0,10 presencial y 0,16/0,08 online.
13. Grupos 4-7 → tasas 0,01 presencial y 0,008 online.

## Simulaciones aritméticas

- G2.2 Enfermería UCI: 12 años antigüedad + 8 categoría + 5 servicio = 30 puntos de experiencia. Méritos simulados = 19. Total = 49.
- G2.2 Enfermería común, incremento: 12 antigüedad + 8 categoría = 20. Méritos simulados = 11,40. Total = 31,40.
- TCAI UCI: 10 antigüedad + 6 categoría + 4 servicio = 24. Méritos simulados = 11,10. Total = 35,10.
- G3.2 común, incremento: 10 antigüedad + 6 categoría = 16. Méritos simulados = 20. Total = 36.
- Grupo 4, incremento: 15 antigüedad + 10 categoría = 25. Méritos simulados = 10,80. Total = 35,80.
- Grupo 1.2: 20 antigüedad + 15 experiencia = 35. Méritos brutos 40,60, limitados a 40. Total = 75.

## Ajustes obligatorios antes de considerar la herramienta "cerrada"

### 1. Desempate de áreas comunes
El procedimiento habla de **puntuación obtenida en la formación sin límite establecido**. El cálculo de desempate debe incluir solo formación (cursos + formación académica + certificados que formen parte del bloque formativo), y **no investigación/docencia**.

### 2. Situaciones asimiladas a activo
La comprobación de acceso no debe formularse únicamente como "estar en activo". Debe permitir también las situaciones asimiladas previstas en el apartado 2.1.4.

### 3. Validez documental de cursos
Un curso solo debe darse como puntuación segura si:
- puede acreditarse;
- la entidad organizadora/expedidora encaja en las admitidas;
- el contenido está relacionado con la vacante;
- ha finalizado antes de la apertura/publicación de la convocatoria.

Si no se puede afirmar alguno de esos extremos, debe mostrarse como pendiente de validación, no como punto seguro.

### 4. Formación no relacionada
Debe existir una opción expresa "no relacionada con la vacante", que dé 0 puntos.

### 5. Titulaciones adicionales
Antes de sumar puntos debe comprobarse que la titulación cumple la rama, nivel, institución/homologación y vinculación exigidos en el apartado aplicable. En los Grupos 3 debe contrastarse con el listado concreto de titulaciones sanitarias del procedimiento; en Grupos 4-7, además, debe ser de nivel igual o superior y de la misma rama de estudios.

### 6. Experiencia desde la obtención del título
En Grupo 2.2 áreas comunes y Grupos 4-7 la experiencia en la categoría se computa a partir de la obtención del título requerido. La interfaz debe pedir al usuario que introduzca únicamente ese periodo o comprobar la fecha.

### 7. Empates en baremos completos
En incremento de jornada/cambio de categoría, si empatan en puntuación total, tiene preferencia quien tenga mayor antigüedad al CSAPG; si persiste el empate, se usa formación sin límite. El resultado debe mostrar esta regla.

### 8. Grupo 1.2 · cambio de turno/servicio
Existe una tensión interpretativa entre la regla general del apartado 2.2.1 para áreas comunes y el baremo general del apartado 3.2, ya que el Grupo 1.2 no clasifica sus puestos como comunes/especiales. No debe presentarse como lectura indiscutible: conviene marcarlo como criterio a validar por la Comisión Mixta/Comisión de trabajo.

### 9. Resto de categorías del Grupo 2.2
Para incremento/cambio de categoría no existe un baremo numérico específico inequívoco en el texto. Mantener bloqueado el total automático es correcto. Para cambio de turno/servicio debe revisarse si corresponde aplicar directamente la regla general de antigüedad de áreas comunes.

### 10. Requisitos que no puntúan pero condicionan la adjudicación
El resultado debe recordar:
- reconocimiento médico de aptitud;
- adaptación al calendario de la vacante;
- posibles excepciones de puestos de confianza o vacantes reservadas;
- permanencia mínima efectiva tras adjudicación, con las excepciones del procedimiento.

## Puntos sujetos a validación/interpretación

- Meses incompletos cuando el texto dice "por cada año" sin definir prorrateo.
- Relación de un curso con la vacante y, cuando corresponda, su carácter específico del servicio.
- Validez de la entidad organizadora/homologación.
- Duración mínima de postgrados (150 h) y másteres (300 h) cuando no consta.
- Formación previa a la titulación de acceso y aplicación de la excepción de compatibilidad.
- Titulaciones adicionales de los Grupos 3 y 4-7.
- Actividades de investigación y docencia y el significado práctico de "actividad y/o año".
- Tasas de formación de Grupo 3: se aplican literalmente aunque sean muy superiores a otros grupos.

## Reglas de seguridad de cálculo

- No completar silenciosamente lagunas del protocolo.
- Si falta una condición documental, mostrar "pendiente de validación".
- Aplicar los máximos de cada factor después de sumar sus componentes.
- Utilizar la fecha de publicación como corte y excluir formación finalizada el mismo día o posteriormente.
- Si constan horas y créditos, prevalecen las horas.
- Solo ECTS: 1 ECTS = 25 horas.
- Solo créditos CFC: 1 crédito = 10 horas.
- Sin horas/créditos: 3 horas por día solo si los días son identificables.
- Si no consta modalidad: online.
- ACTIC: solo nivel superior, máximo 1 punto.
- Catalán: solo nivel superior, máximo 2 puntos.
- Otros idiomas: nivel superior por idioma, suma máxima 1 punto.
- La titulación mínima de acceso no puntúa.
- La puntuación oficial corresponde a la evaluación de los órganos previstos en el procedimiento.
