
# Ivy Portfolio Strategy

Este repositorio contiene una implementación de una estrategia de inversión basada en el libro "The Ivy Portfolio" de Mebane Faber y Eric Richardson. La estrategia selecciona el activo con mejor momentum entre un universo de activos y ajusta las inversiones en consecuencia.

## Descripción

La estrategia selecciona el activo con mejor momentum entre un universo de 5 activos:
- `EFA`
- `SPY`
- `GSG`
- `IYR`
- `AGG`
- `BIL` (cuando los respectivos momentums son negativos)

El momentum se calcula utilizando la relación entre el precio actual y la media móvil de los últimos 10 o 12 meses, dependiendo del notebook utilizado. La inversión se ajusta mensualmente para seleccionar el activo con mejor rendimiento.

## Requisitos

- Python 3.x
- Pandas
- yfinance

## Instalación

1. Clona este repositorio:
   ```sh
   git clone https://github.com/JosueMonte/Ivy_Portfolio.git
   cd Ivy_Portfolio
   ```

2. Instala los paquetes requeridos:
   ```sh
   pip install pandas yfinance
   ```

## Uso

Puedes ejecutar cualquiera de los notebooks para ver la implementación y los resultados de la estrategia. Los notebooks incluyen:
- Cálculo del momentum de los activos.
- Obtención de datos históricos de los activos utilizando `yfinance`.
- Selección del mejor activo basado en el momentum.
- Registro de las decisiones de inversión mensuales.

### Notebooks Disponibles

- `ivy_portfolio_5_SMA10_bestone.ipynb`: Utiliza la media móvil de los últimos 10 meses para calcular el momentum.
  [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JosueMonte/Ivy_Portfolio/blob/main/ivy_portfolio_5_SMA10_bestone.ipynb)

- `ivy_portfolio_5_SMA12_bestone.ipynb`: Utiliza la media móvil de los últimos 12 meses para calcular el momentum.
  [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JosueMonte/Ivy_Portfolio/blob/main/ivy_portfolio_5_SMA12_bestone.ipynb)

## Ejecución

Para ejecutar un notebook:

1. Abre Jupyter Notebook:
   ```sh
   jupyter notebook
   ```

2. Navega hasta el archivo del notebook que deseas ejecutar (`ivy_portfolio_5_SMA10_bestone.ipynb` o `ivy_portfolio_5_SMA12_bestone.ipynb`) y ábrelo.
3. Ejecuta las celdas para ver los resultados.

## Resultados

Los notebooks muestran los activos seleccionados mensualmente y sus rendimientos. También se calculan los rendimientos acumulados de la estrategia.

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un issue o un pull request si tienes sugerencias o mejoras.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.
