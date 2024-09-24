# Jupyter Notebook - El hogar del buho

Este proyecto me permitió crear mi CV personal utilizando Jupyter Notebook. El CV se crea en en un notebook que posteriormente se convierte a HTML utilizando una plantilla personalizada, y se puede alojar en GitHub Pages.

Resultado final: https://elhogardelbuho.com

## Estructura del Proyecto

- `docker-compose.yml`: Configuración de Docker.
- `notebook/`: Contiene el notebook y la plantilla personalizada.
- `resume.ipynb`: Notebook con el contenido del CV.
- `index.html`: CV exportado a HTML.

## Instrucciones de Configuración

1. Iniciar Jupyter Notebook:

```bash
docker-compose -f notebooks/docker-compose.yml up --build -d
```

2. Visualiza el contenido en localhost:8888 

3. Generar HTML desde el notebook:

```bash
jupyter nbconvert --execute --to html --template=notebook/personal_template --output=../index.html notebook/resume.ipynb
```