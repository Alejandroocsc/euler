# Enfriamiento de una taza de café

Este ejercicio compara la solución exacta de una ecuación diferencial separable con una aproximación mediante el método de Euler.

## Problema y solución exacta

Una taza comienza a 80 °C en una habitación a 20 °C. Su temperatura satisface:

```text
dT/dt = -0.5(T - 20),   T(0) = 80
```

El tiempo está en minutos y la temperatura en grados Celsius. Al separar variables e integrar:

```text
dT/(T - 20) = -0.5 dt
ln|T - 20| = -0.5t + C
T(t) = 20 + 60e^(-0.5t)
```

La constante se obtiene de la condición inicial. El cuaderno aplica Euler con `h = 0.2` en `[0, 1]`, muestra una tabla con el error absoluto y grafica ambas soluciones.

## Ejecutar el cuaderno

1. Abre `euler_separable.ipynb` en VS Code o Jupyter.
2. Selecciona un entorno de Python con `numpy`, `matplotlib` e `ipykernel`. Si faltan, instálalos en ese entorno con:

   ```text
   python -m pip install numpy matplotlib ipykernel
   ```

3. Ejecuta las celdas en orden.

En este equipo puedes seleccionar el entorno virtual `.venv` de la carpeta principal de Ecuaciones Diferenciales. El entorno virtual no forma parte de los archivos que se compartirán.
