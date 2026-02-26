💸 Actualizador de cotizaciones(Argentina)

Una aplicación web de escritorio construida con Streamlit que automatiza la extracción, procesamiento y volcado de cotizaciones financieras y datos agropecuarios de Argentina en una planilla de Excel local.

✨ Características Principales

Extracción de Divisas: Realiza scraping y consultas a APIs para obtener el Dólar Oficial (BNA), Dólar MEP y Dólar Libre (Blue).

Índices Macroeconómicos: Obtiene valores históricos actualizados de UVA, Índice CAC (Cámara Argentina de la Construcción), Salario Mínimo Vital y Móvil (SMVyM) e IPC.

Agro / Pizarra Rosario: Descarga los precios diarios de cereales (Trigo, Maíz, Sorgo, Girasol, Soja) aplicando formato condicional en Excel para resaltar valores estimativos.

Gestión Inteligente de Excel: Crea automáticamente las hojas faltantes, rellena fechas sin cotización (arrastrando el último valor válido) y aplica estilos y anchos de columna.

Actualización Autónoma: Cuenta con un sistema de memoria persistente que detecta si pasaron más de 24 horas desde la última carga exitosa para auto-ejecutarse.

Interfaz de Configuración: Permite al usuario seleccionar el archivo .xlsx de destino visualmente mediante el explorador de archivos nativo del sistema operativo.

Protección contra Bloqueos: Detecta si el archivo Excel está siendo utilizado por otro usuario o programa para evitar corrupciones de datos.

🛠️ Tecnologías Utilizadas

Python 3

Streamlit: Para la interfaz gráfica de usuario.

Pandas: Procesamiento, limpieza y reestructuración de datos (DataFrames).

BeautifulSoup4 & Requests: Web scraping y consumo de APIs REST.

Openpyxl: Lectura, escritura y estilizado de archivos Excel.

Tkinter: Integrado para cuadros de diálogo de selección de archivos nativos.

🚀 Uso

Instala las dependencias necesarias:

pip install streamlit requests pandas beautifulsoup4 openpyxl urllib3


Ejecuta la aplicación:

streamlit run _📈_Consulta de cotizaciones.py


En la primera ejecución, la aplicación te pedirá buscar o crear un archivo Excel de destino. ¡Luego se actualizará de forma autónoma!
