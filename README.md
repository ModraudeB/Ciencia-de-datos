## Descripción general
Este proyecto explora y compara la evolución de los precios de las acciones y los ingresos trimestrales de Tesla y GameStop. Se emplean técnicas de extracción de datos desde fuentes públicas y visualización interactiva para facilitar el análisis comparativo entre ambas compañías.
## Objetivos
- Obtener datos históricos de precios de las acciones de Tesla y GameStop usando la API de Yahoo Finance.
- Extraer los ingresos trimestrales de ambas empresas mediante web scraping.
- Limpiar y preparar los datos para su análisis.
- Visualizar la información de manera interactiva para identificar tendencias y patrones relevantes.
## Metodología
1. **Extracción de datos bursátiles:** Se utiliza la librería `yfinance` para descargar los precios históricos de las acciones.
2. **Web scraping de ingresos:** Los ingresos trimestrales se obtienen de tablas HTML públicas mediante `requests`, `BeautifulSoup` y `pandas.read_html`.
3. **Procesamiento y limpieza:** Se normalizan los formatos de fecha y valores numéricos, eliminando inconsistencias y datos faltantes.
4. **Visualización:** Se emplea Plotly para crear dashboards interactivos que permiten comparar la evolución de precios e ingresos.
## Fuentes de datos
- [Yahoo Finance](https://finance.yahoo.com/): para precios históricos de acciones.
- [Datos de ingresos](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/revenue.htm) y [stock](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/stock.html): para ingresos trimestrales.
## Estructura del repositorio
- `Final_Assignment-v2.ipynb`: Notebook principal con todo el análisis y visualizaciones.
- `environment.yml`: Entorno reproducible para Conda.
- `README.md`: Este archivo.
- `/images`: Carpeta sugerida para guardar visualizaciones exportadas.
- `.github/workflows/run-notebook.yml`: Workflow de integración continua.
### Instalación de dependencias manual (opcional)
Si prefieres instalar dependencias manualmente:
```bash
pip install yfinance beautifulsoup4 requests "plotly>=5" pandas jupyterlab papermill
```
## Ejecución del notebook
1. Abre JupyterLab:
   ```bash
   jupyter lab
   ```
2. Abre el archivo `Final_Assignment-v2.ipynb`.
3. Ejecuta todas las celdas para reproducir los resultados y visualizar el dashboard.
## Contacto
Para dudas o sugerencias puedes abrir un issue en el repositorio o contactar al autor vía GitHub.
Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.
