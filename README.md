# Actividad 5: regresiones con Python

Abre `Regresion_LML.ipynb` en Jupyter Notebook o Google Colab y ejecuta sus
celdas de arriba hacia abajo. El notebook lee `Datos_Complementarios_CLV.xlsx`
desde la misma carpeta. En Google Colab, primero sube el Excel al entorno.
El notebook está guardado en UTF-8 para conservar acentos y caracteres
especiales.

## Instalar lo necesario

```powershell
python -m pip install pandas numpy matplotlib scikit-learn openpyxl
```

El notebook carga la hoja de ventas, completa valores nulos, trata valores
extremos con el rango intercuartílico, transforma algunos predictores con
`log(1+x)`, y muestra correlaciones, regresión lineal simple y múltiple, y
regresión logística con oversampling manual.

Incluye gráficas descriptivas de la distribución y los valores extremos de las
ventas, las marcas más frecuentes, un mapa de calor con valores de correlación,
gráficas de valores reales frente a predichos y una matriz de confusión.
Para cada clase de la regresión logística también reporta precisión, recall,
F1 y soporte, además de una gráfica para comparar precisión, recall y F1 entre
venta baja y venta alta.

El notebook guarda las gráficas en la carpeta `figuras` al ejecutarse. El
archivo `Reporte_Regresiones.tex` incluye esas imágenes en el reporte detallado.
Ejecuta todas las celdas del notebook y luego compila el `.tex` con pdfLaTeX
desde esta carpeta. Si una imagen falta, el documento muestra un recuadro con
el nombre que espera.
