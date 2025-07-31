## Análisis de Precios e Ingresos – Tesla vs GameStop

### Resumen del proyecto
Este proyecto tiene como objetivo extraer y analizar datos históricos de precios de las acciones y los ingresos de Tesla y GameStop, utilizando técnicas de web scraping y la librería `yfinance`. Se desarrolla un dashboard interactivo con Plotly para comparar visualmente ambas empresas.

### Objetivo
- Extraer datos de precios históricos y reportes de ingresos de Tesla y GameStop.
- Realizar análisis comparativo y visualización interactiva mediante dashboards.

### Clonar el repositorio y crear el entorno
```bash
git clone ${{ github.repository_url }}
cd <nombre-del-repositorio>
conda env create -f environment.yml
conda activate final-stocks
```

### Instalación de dependencias manual (opcional)
Si prefieres instalar dependencias manualmente:
```bash
pip install yfinance beautifulsoup4 requests "plotly>=5" pandas jupyterlab papermill
```

### Ejecución del notebook
1. Abre JupyterLab:
   ```bash
   jupyter lab
   ```
2. Abre el archivo `Final_Assignment-v2.ipynb`.
3. Ejecuta todas las celdas para reproducir los resultados y visualizar el dashboard.

### Integración continua
Cada vez que haces un push o pull request a la rama `main`, el workflow de GitHub Actions (`.github/workflows/run-notebook.yml`) ejecuta automáticamente el notebook principal (`Final_Assignment-v2.ipynb`) usando papermill. Si alguna celda falla, la acción marcará el workflow como fallido, ayudando a garantizar la reproducibilidad y calidad del análisis.

### Capturas de pantalla
Si incluyes imágenes de resultados, colócalas en la carpeta `/images` y enlázalas aquí:
- ![Dashboard comparativo](images/dashboard.png)

### Licencia
Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.
