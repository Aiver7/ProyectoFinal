{\rtf1\ansi\ansicpg1252\cocoartf2907
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # Huellas al d\'eda\
\
## Integrantes del Equipo\
\
### Alex Aiverson Palacios Mosquera\
**Programa Acad\'e9mico:** Ingenier\'eda Industrial\
**Descripci\'f3n, Habilidades y Fortalezas:** \
Fundamentos de Python, habilidades medias en dise\'f1o gr\'e1fico, edici\'f3n de im\'e1genes digitales, organizaci\'f3n, an\'e1lisis de problemas y cumplimiento de fechas.\
**Aporte al proyecto:** \
Creaci\'f3n del nombre del proyecto y el logo, apoyar en la definici\'f3n de requisitos, la documentaci\'f3n y la creaci\'f3n del c\'f3digo.\
\
### Iv\'e1n Ricardo Naranjo Bustamante\
**Programa Acad\'e9mico:** Ingenier\'eda Industrial\
**Descripci\'f3n, Habilidades y Fortalezas:** \
Alta capacidad de adaptaci\'f3n a cualquier contexto o din\'e1mica de trabajo, junto con un nivel intermedio de ingl\'e9s. Destaca por su versatilidad y facilidad para integrarse a diferentes entornos.\
**Aporte al proyecto:** \
Participaci\'f3n equitativa e integral en todas las fases del proyecto, brindando apoyo transversal tanto en la estructuraci\'f3n documental como en el desarrollo t\'e9cnico, ajust\'e1ndose r\'e1pidamente a los requerimientos puntuales del equipo.\
\
## Descripci\'f3n\
\
### Logo \
![Logo de Huella PQRS](images/logo.jpeg) \
\
### Descripci\'f3n \
Este proyecto consiste en el desarrollo de un sistema de informaci\'f3n por consola dise\'f1ado para centralizar y administrar las Peticiones, Quejas, Reclamos y Sugerencias (PQRS) relacionadas con la atenci\'f3n veterinaria de perros y gatos. El software automatiza la asignaci\'f3n de radicados \'fanicos, controla los tiempos m\'e1ximos de respuesta de 30 d\'edas y genera estad\'edsticas clave, optimizando la gesti\'f3n documental y el servicio prestado por la organizaci\'f3n.\
\
## Licencia del software \
\
1. **Licencia para el C\'f3digo Fuente (MIT):** Todo el c\'f3digo ejecutable alojado en la carpeta `src/` se distribuyen bajo la Licencia MIT, permitiendo su libre uso, modificaci\'f3n y distribuci\'f3n.\
2. **Licencia para Documentaci\'f3n y Recursos Gr\'e1ficos (Creative Commons):** Siguiendo las directrices del curso, todos los documentos, manuales, el logo y los textos alojados en `docs/` e `images/` est\'e1n registrados bajo la licencia **CC BY-NC 4.0** (Atribuci\'f3n-NoComercial 4.0 Internacional).\
\
## Reporte de visi\'f3n\
\
### Problema que se busca resolver\
\
Huellas al dia recibe PQRS por medios como redes sociales, correo electr\'f3nico,\
tel\'e9fono y atenci\'f3n presencial. Cuando estas solicitudes se gestionan\
manualmente, resulta m\'e1s dif\'edcil mantener la informaci\'f3n organizada,\
consultar el estado de cada caso y verificar cu\'e1les se acercan a su\
fecha m\'e1xima de respuesta.\
\
Huellas al D\'eda busca reunir esas tareas en un programa de consola que\
permita registrar y consultar la informaci\'f3n de manera estructurada.\
\
###  Objetivo general\
\
Desarrollar un programa de consola en Python que permita a Huellas al dia\
registrar, consultar y gestionar las PQRS relacionadas con la atenci\'f3n\
de perros y gatos, utilizando archivos de texto (.txt) para conservar la\
informaci\'f3n y generar reportes de apoyo a la gesti\'f3n.\
\
### Objetivos espec\'edficos\
\
- Registrar los datos del solicitante y la informaci\'f3n de cada PQRS.\
- Clasificar las solicitudes como petici\'f3n, queja, reclamo o sugerencia.\
- Asignar a cada registro un identificador consecutivo dentro de su\
  tipo de solicitud.\
- Almacenar cada tipo de PQRS en un archivo plano independiente.\
- Consultar las solicitudes registradas y su estado.\
- Permitir el avance del estado desde \'abRegistrada\'bb hasta \'abSolucionada\'bb,\
  pasando por \'abEn proceso\'bb.\
- Calcular y mostrar la fecha m\'e1xima de respuesta establecida para\
  cada solicitud.\
- Generar un comprobante de radicaci\'f3n en formato TXT.\
- Presentar estad\'edsticas que ayuden a conocer el volumen y la gesti\'f3n\
  de las solicitudes.\
\
### Beneficios esperados\
\
- Organizar las PQRS recibidas por diferentes canales.\
- Facilitar la consulta de solicitudes y de su estado.\
- Disminuir errores asociados con la asignaci\'f3n manual de consecutivos.\
- Apoyar el seguimiento de los plazos de respuesta.\
- Contar con comprobantes de radicaci\'f3n uniformes.\
- Obtener estad\'edsticas \'fatiles para revisar la gesti\'f3n de MEPEGA.\
\
## Especificaci\'f3n de requisitos\
\
### Requisitos funcionales\
\
- Mostrar un men\'fa principal con opciones para registrar, consultar, actualizar estados, ver estad\'edsticas y salir. El usuario puede seleccionar cada opci\'f3n desde la consola. \
- Registrar una PQRS con datos del solicitante, informaci\'f3n de la solicitud y datos relacionados. El registro se guarda \'fanicamente si supera las validaciones.\
- Permitir seleccionar el tipo de solicitud: Petici\'f3n, Queja, Reclamo o Sugerencia. El sistema rechaza valores distintos de los permitidos.\
- Asignar un ID entero consecutivo a cada PQRS, comenzando en 1 y con una secuencia independiente por tipo. Una nueva petici\'f3n recibe el ID siguiente de `Peticion.txt`, sin depender de los IDs de `Queja.txt`. \
- Guardar cada tipo de PQRS en su archivo plano correspondiente. | Las peticiones se guardan solo en `Peticion.txt`; las quejas, en `Queja.txt`; los reclamos, en `Reclamo.txt`; y las sugerencias, en `Sugerencia.txt`. \
- Registrar autom\'e1ticamente el estado inicial `Registrada`. Toda PQRS reci\'e9n creada tiene ese estado.\
- Calcular la fecha m\'e1xima de respuesta sumando 30 d\'edas calendario a la fecha de registro. | La fecha calculada queda asociada al registro y aparece en el radicado.\
- Consultar las PQRS registradas y mostrar su informaci\'f3n y estado actual. | El usuario puede identificar una PQRS mediante su tipo y su ID.\
- Permitir el cambio de estado `Registrada` \uc0\u8594  `En proceso` \u8594  `Solucionada`. El sistema acepta el siguiente estado permitido y rechaza saltos o retrocesos.\
- Generar un comprobante de radicaci\'f3n en un archivo TXT. El archivo contiene los datos exigidos y puede abrirse como texto.\
- Mostrar una PQRS consultada con el mismo formato b\'e1sico del radicado. La consulta refleja el estado actual del registro.\
- Calcular el promedio de d\'edas de respuesta de las PQRS solucionadas. El reporte muestra un resultado entero cuando existen casos con fecha de soluci\'f3n registrada. \
- Presentar cinco estad\'edsticas adicionales sobre los registros. Cada estad\'edstica muestra resultados calculados a partir de los archivos planos.\
- Permitir salir del programa desde el men\'fa principal. La ejecuci\'f3n termina sin modificar los registros existentes.\
- Generar el radicado como archivo de texto TXT. \
- Delimitar el comprobante mediante un marco de caracteres ASCII, como `+`, `-` y `|`. \
- Hacer que cada l\'ednea del comprobante tenga exactamente 120 caracteres. \
- Centrar y alinear las secciones principales. \
- Mostrar el nombre del sistema y el t\'edtulo del comprobante. \
- Mostrar tipo de solicitud, ID, fecha y hora de radicaci\'f3n, estado y fecha m\'e1xima de respuesta. \
- Mostrar nombre, documento, tel\'e9fono, correo y direcci\'f3n del solicitante. \
- Mostrar canal de recepci\'f3n, tipo de mascota, campus y asunto. \
- No incluir la descripci\'f3n detallada de la solicitud. \
- Mostrar `N/A` cuando la direcci\'f3n no se haya registrado. \
\
### Requisitos no funcionales\
\
- El men\'fa y los mensajes deben ser claros para el administrador. \
- Los registros deben conservarse al cerrar y volver a abrir el programa.\
- Guardar una PQRS nueva no debe borrar ni sobrescribir registros anteriores. \
- Los cuatro archivos planos deben manejar la misma estructura. Comparar los campos almacenados en cada archivo. \
- Las validaciones, la lectura y escritura de archivos, y los reportes deben separarse en m\'f3dulos.\
- El programa debe ejecutarse con Python 3 en un entorno que cumpla sus dependencias.\
- El c\'f3digo debe estar en `src/`, la documentaci\'f3n en `docs/`, las im\'e1genes en `images/` y los archivos en `data/`. \
- Cada l\'ednea generada en un radicado debe tener 120 caracteres.\
\
## Plan de proyecto\
\
###  Actividades y productos\
\
- Reuni\'f3n inicial y elaboraci\'f3n de las tres actas\
- Definici\'f3n del nombre, logo y licencias \
- Elaboraci\'f3n del reporte de visi\'f3n \
- Especificaci\'f3n de requisitos \
- Elaboraci\'f3n y revisi\'f3n del plan de proyecto \
- Dise\'f1o de clases, m\'f3dulos y archivos planos \
- Implementaci\'f3n de validaciones \
- Implementaci\'f3n del almacenamiento que son M\'f3dulo `archivos.py` y archivos TXT de datos\
- Implementaci\'f3n del men\'fa y registro de PQRS \
- Implementaci\'f3n de consulta y cambio de estado \
- Generaci\'f3n del comprobante de radicaci\'f3n \
- Implementaci\'f3n de estad\'edsticas \
- Pruebas y correcci\'f3n de errores \
- Manual, revisi\'f3n final y preparaci\'f3n de la sustentaci\'f3n \
 **El total de horas del equipo son 60** \
\
### Diagrama de Gantt\
\
El siguiente diagrama muestra las actividades previstas para las\
16 semanas acad\'e9micas del proyecto.\
\
![Diagrama de Gantt de Huellas al D\'eda](images/GANTT.jpg)\
\
### Presupuesto en tiempo de formaci\'f3n\
\
Para el desarrollo de este software, nuestro equipo, compuesto por 2 integrantes, ha proyectado una inversi\'f3n total de 58 horas de trabajo. \
\
**C\'e1lculo de la remuneraci\'f3n:**\
**Base de liquidaci\'f3n:** 1 Salario M\'ednimo Legal Vigente (SMLV) correspondiente a pr\'e1ctica profesional.\
**Jornada mensual de referencia:** 240 horas.\
**Valor por hora invertida:** Al dividir 1 SMLV entre las 240 horas mensuales, se obtiene que cada hora de desarrollo equivale aproximadamente al 0.417% de 1 SMLV.\
**Costo Total del Proyecto:** Al multiplicar el valor por hora por las 58 horas totales invertidas por el equipo, el presupuesto del proyecto equivale a una remuneraci\'f3n en tiempo de formaci\'f3n del 24.17% de 1 SMLV.\
\
<a href="https://github.com/Aiver7/ProyectoFinal"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Huellas al dia</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> \'a9 2026 por</font></font><a href="https://example.com"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> Alex Aiverson Palacios Mosquera e Iv\'e1n Ricardo Naranjo Bustamante  </font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> tiene licencia</font></font><a href="https://creativecommons.org/licenses/by-nc-sa/4.0/"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> CC BY-NC-SA 4.0</font></font></a><img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/nc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/sa.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;">}