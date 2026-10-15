# Diagnóstico de la Situación Logística | LogisPyme

Herramienta web interactiva y autocontenida (*single-file app*) diseñada para evaluar de forma exhaustiva el nivel de madurez operativa y estratégica de la cadena de suministro en empresas.

El cuestionario analiza **puntos de control clave** organizados en 8 fases logísticas:
1. **Estrategia**: Organización, formación, comunicación y planificación global.
2. **Compras**: Homologación de proveedores, negociación y digitalización.
3. **Gestión de Stock y Aprovisionamiento**: Parámetros de inventario, previsión de la demanda y control.
4. **Almacén**: *Layout*, sistemas de almacenaje, manutención y seguridad.
5. **Manipulación en Almacén**: Procesos operativos de entrada, *picking* y expedición.
6. **Transporte de Distribución**: Planificación de rutas, gestión de flotas y última milla.
7. **Logística Inversa**: Gestión de devoluciones (RMA), economía circular y residuos.
8. **Experiencia del Cliente**: Niveles de servicio (SLA), resolución de incidencias y satisfacción.

---

## Características principales

* **100 % Autocontenido**: Todo el código (HTML5, estilos CSS3 y lógica en JavaScript) reside en un único archivo. No requiere servidores, Node.js ni bases de datos externas.
* **Aleatorización anti-sesgo**: Las opciones de respuesta se desordenan automáticamente en cada sesión para garantizar respuestas objetivas.
* **Almacenamiento local (Offline)**: Guarda los diagnósticos directamente en el almacenamiento del navegador (`localStorage`), permitiendo consultar el histórico y reanudar evaluaciones.
* **Informe ejecutivo instantáneo**:
  * Cálculo automático del nivel de madurez (Inicial, Básico, En desarrollo, Consolidado o Avanzado).
  * Gráfico de radar (estrella) vectorial en SVG con comparativa frente a la media del sector.
  * Plan de recomendaciones prioritarias según los puntos débiles detectados.
* **Exportación y descarga**:
  * Exportación de resultados a CSV (resumen y detalle de respuestas).
  * Copia de seguridad en formato JSON.
  * Vista adaptada a impresión directa para generar informes en PDF (`Ctrl + P` o `Cmd + P`).

---

## Modo de uso

### 1. Ejecución local (en tu ordenador)
1. Descarga o clona el archivo `diagnostico_logistico.html` en tu equipo.
2. Haz doble clic sobre el archivo para abrirlo con cualquier navegador moderno (*Chrome, Edge, Firefox, Safari*).
3. No se requiere conexión a internet (salvo para cargar la tipografía inicial).

### 2. Publicación en la web (GitHub Pages)
Para convertirlo en una aplicación web accesible mediante enlace:
1. Sube el archivo a este repositorio con el nombre `index.html`.
2. Ve a **Settings** > **Pages** en GitHub.
3. En la sección **Branch**, selecciona `main` (o `master`) y la carpeta `/ (root)`.
4. Haz clic en **Save**. En unos segundos tendrás tu enlace público listo para compartir con clientes o alumnos.

---

## Flujo de trabajo dentro de la aplicación

1. **Datos de la empresa**: Introduce la información general de la organización, sector y fecha.
2. **Cumplimentación por fases**: Navega por las 8 fases respondiendo a cada una de las preguntas de opción múltiple.
3. **Validación y guardado**: En la pestaña *Finalizar y grabar*, el sistema comprobará que no queden preguntas pendientes y almacenará el registro.
4. **Informe**: Accede al informe ejecutivo para revisar el diagnóstico, consultar el gráfico radar e imprimirlo o descargarlo en PDF.
