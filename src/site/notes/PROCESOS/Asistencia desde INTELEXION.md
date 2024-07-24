---
{"dg-publish":true,"permalink":"/procesos/asistencia-desde-intelexion/"}
---

Durante el transcurso del día, ITX (Intelexion) manda un CDL con la información de las asistencias de cada uno de los empleado activos por sucursal. Para esto, se creó un [[CDL's Personalizados\|CDL's Personalizados]] con la información requerida con el File Type **ASTNC**. 
Una vez depositado el CDL en el SFTP se hace una validación con un [[STORED PROCEDURE/Stored Procedure\|Stored Procedure]]. Este último valida la información y hace 2 procesos:
+ Inserta los datos en la tabla del [[TABLAS/Esquema EXT\|Esquema EXT]] TB_ASISTENCIA_ITX_HIS
+ De la tabla del [[TABLAS/Esquema EXT\|Esquema EXT]] TB_ASISTENCIA_WKF, verifica que registros coinciden en las columnas ID_EMPLEADO y FECHA_ASISTENCIA con las columnas ID_EMPLEADO, FECHA_LECTURA de la tabla EXT.TB_ASISTENCIA_ITX_TMP y modifica el valor de la columna ASISTENCIA_ITX de la tabla EXT.TB_ASISTENCIA_WKF pasándolo de false a true.