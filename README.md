# CI/CD con GitHub Actions (Python)

Este repositorio contiene un ejemplo de pipeline CI/CD utilizando GitHub Actions para una aplicación Python simple.

## ¿Qué hace el pipeline?

El workflow ejecuta:

1. Instalación de dependencias.
2. Análisis estático básico (linting con flake8).
3. Ejecución de pruebas (tests unitarios si existen).
4. Validación de que la aplicación se ejecuta correctamente.

## Estructura del repositorio

- app.py — Aplicación Python de ejemplo.
- requirements.txt — Dependencias necesarias para ejecutar el proyecto.
- .github/workflows/ci.yml — Pipeline CI/CD definido en GitHub Actions.

## Requisitos

- Python 3.9 o superior
- GitHub Actions habilitado en el repositorio

## Ejecución local

pip install -r requirements.txt
python app.py

## Pipeline CI/CD

Cada vez que se haga un push o pull request a la rama main, GitHub Actions ejecutará automáticamente:

- Instalación de dependencias.
- Linting.
- Pruebas.
- Ejecución del script.

El estado del pipeline puede verse en la pestaña Actions del repositorio.
