---
{"dg-publish":true,"permalink":"/procesos/generacion-de-asistencia-base/"}
---

Todos los días, mediante la ejecución de un Scheduled Task desde Workflow programado a las 7am, se ejecuta un Stored Procedure (SP_ASTNCITX) que toma la información de la tabla TCMP.CS_POSITION ([[TABLAS/Esquema TCMP\|Esquema TCMP]][[CDL's Estándar\|CDL's Estándar]]), EXT.TB_SUCMESAEMPL_WKF([[CDL's Personalizados\|CDL's Personalizados]][[TABLAS/Esquema EXT\|Esquema EXT]]) y EXT.TB_PORCPARTICIPACION_WKF([[CDL's Personalizados\|CDL's Personalizados]][[TABLAS/Esquema EXT\|Esquema EXT]]) y hace una inserción a la tabla del esquema extendido EXT.TB_ASISTENCIA_WKF ([[TABLAS/Esquema EXT\|Esquema EXT]]).

