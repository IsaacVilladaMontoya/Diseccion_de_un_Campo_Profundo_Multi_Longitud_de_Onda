# Parte B del proyecto.

En esta rama se realiza el analisis cosmológico de la region de interes (AR: 135.5, DEC: 0.5). Todo el proceso de extraccion y representación esta adjunto en el notebook de python `SSDS_analisis.ipynb` Esta es su estructura:


- **Extracción:** Se utiliza una celda de Bash para enviar una consulta SQL al SkyServer de SDSS.

- **Lógica de Datos:** Se realiza un INNER JOIN relacional entre las tablas de espectroscopía y fotometría de los datos extraidos. Se extrae la clase del objeto (class), el corrimiento al rojo (z) y las magnitudes ultravioleta y verde (u, g), limitando la búsqueda exactamente a la región de interes.

- **Análisis:** Se grafica el Corrimiento al Rojo vs Índice de Color (
) para cada clase, separando visualmente las Galaxias de los Cuásares. Se guardan las graficas en la ubicación `imagenes_spec/`

- **Exploración Web:** Se utilizo la interfaz web de MAST para buscar si el Telescopio Espacial Hubble (HST) o el James Webb (JWST) han tomado imágenes de alta resolución en las coordenadas exactas de este campo profundo.

Se concluye que almenos en la plataforma de MAST no existe ningún registro de alguna toma o observación de Hubble para esa zona. por otro lado, se incluye una captura de pantalla de la imagen tomada por JWST en la ubicación del repo: `imagenes_misiones/`. 
