# jpl NetTools · v1.6.1

**Herramientas prácticas de redes y soporte IT · JPL Network · Jordi Pérez Llorà**

[**Abrir la aplicación**](https://jpl-network.github.io/jpl-nettools/)

Un laboratorio de 14 herramientas para calcular direccionamiento, planificar redes, documentar incidencias y practicar diagnóstico. Desarrollado con asistencia de IA en HTML, CSS y JavaScript, sin backend ni instalación.

## Herramientas

| Área | Funciones |
| --- | --- |
| Direccionamiento | Calculadora IPv4, VLSM, detección de solapamientos, conversor de máscaras y comprobador IP/subred/gateway |
| Configuración | Plantillas VLAN Cisco IOS/IOS XE, planificador de sede y comparación literal de configuraciones |
| Soporte | Diagnóstico guiado, informes de incidencias, biblioteca de comandos y análisis de salidas |
| Aprendizaje | Ejercicios de subnetting y casos prácticos de diagnóstico |

## Cómo usarlo

Abre la aplicación y selecciona una herramienta en el menú o búscala por nombre. También puedes descargar el repositorio y abrir `index.html` localmente. No necesitas instalar dependencias.

El planificador permite exportar CSV, guardar y recuperar proyectos JSON e imprimir el plan. Los informes de incidencias se pueden descargar como TXT. **No hay guardado automático:** descarga los proyectos que quieras conservar.

Cinco herramientas incluyen botones **Cargar ejemplo** y **Restablecer**: solapamientos, comparación de configuraciones, análisis de salidas, informes de incidencias y planificador de sede. Los ejemplos utilizan datos ficticios. Antes de reemplazar datos introducidos se solicita confirmación.

El menú agrupa las herramientas por función y las numera del 01 al 14. En móvil se muestra completo, sin desplazamiento interno.

## Ejemplo práctico

Divide `192.168.1.0/24` entre departamentos de `60, 25, 10, 2` hosts. El planificador VLSM asigna bloques de mayor a menor tamaño y comprueba que caben en la red base. En el planificador de sede se añade además una dirección para el gateway de cada departamento.

## Privacidad y alcance

- Los cálculos y las entradas se procesan en el navegador. No hay cuentas, analítica ni envío de direcciones IP a un backend de la aplicación.
- Las tipografías se solicitan a Google Fonts; GitHub Pages puede registrar accesos al alojamiento.
- Las herramientas no conectan con dispositivos ni ejecutan los comandos que generan.
- Las plantillas requieren revisar plataforma y configuración existente antes de utilizarlas.
- El comparador es literal y el analizador trabaja con patrones; no sustituyen un diagnóstico técnico del entorno.
- IPv4 /31 se interpreta como enlace punto a punto y /32 como dirección individual. VLSM reserva red y broadcast: dos hosts requieren /30.

## Estado de validación

La lógica dispone de pruebas locales para IPv4, VLSM, solapamientos, máscaras, VLAN, planificación/importación, pertenencia IP, diferencias y patrones de análisis. Los archivos de prueba todavía no forman parte de este repositorio público.

Revisión de la web publicada el 6 de noviembre de 2026: navegación de las 14 vistas, búsqueda sin acentos, errores de IPv4 y capacidad del planificador, apertura/cierre del diálogo y revisión del planificador a ancho móvil. No se observaron errores de JavaScript durante ese recorrido. En la revisión manual guiada, el autor confirmó la descarga y recuperación de proyectos JSON, la apertura de CSV en Excel, la impresión a PDF sin columnas cortadas, la descarga de informes TXT y el funcionamiento de los ejemplos y del restablecimiento. También confirmó el menú completo en su móvil. Estas comprobaciones cubren los casos revisados, no todas las combinaciones de datos o navegadores. No se han realizado pruebas en dispositivos de red reales.

## Mejoras y errores

Puedes comunicar fallos o proponer mejoras en [GitHub Issues](https://github.com/JPL-NETWORK/jpl-nettools/issues). Indica la herramienta, el resultado esperado y lo que ocurrió; utiliza datos ficticios y evita incluir información de clientes o credenciales.

## Últimos cambios

- v1.6: ejemplos y restablecimiento en cinco herramientas, historial y enlace a incidencias.
- v1.6.1 y ajustes de presentación: marca jpl NetTools, numeración consecutiva, portada «Herramientas para Networking» y menú móvil completo.

## Autor

**JPL Network · Jordi Pérez Llorà** — Redes, sistemas y soporte IT.

Proyecto desarrollado con asistencia de IA, orientado a practicar y mostrar procesos de trabajo técnico.
