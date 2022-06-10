GF601, otoño 2022

# Tarea 4: Series de tiempo y regresión lineal múltiple

En esta tarea se analizará el régimen hidro-climático de la cuenca del río Trancura en la región
de la Araucanía. Para ello, considere los registros diarios de caudal (en mm) en la estación
DGA 9414001 (“Rio Trancura Antes Rio Llafenco”) y de precipitación del producto CR2MET
integrada sobre la cuenca, ambos disponibles en la plataforma de datos CAMELS-CL (https://
camels.cr2.cl/). Para lo que sigue, considere el periodo 1979-2018 y elimine los días bisiestos.

1. A partir de los registros diarios, calcule el ciclo estacional medio de ambas variables
    aplicando un análisis armónico en la forma que estime conveniente (cuidado con los días
    faltantes). Justifique los pasos seguidos. Apoyado en gráficos simples (valor vs. día del
    año), compare los ciclos obtenidos respecto de lo que se deriva mediante promedios
    simples. Describa e interprete brevemente los ciclos resultantes para caudal y
    precipitación, así como las diferencias entre estas variables.
2. Haga un análisis espectral de las series de anomalías diarias de caudal y precipitación. En
    ambos periodogramas, compare su resultado con un espectro de referencia de tipo AR(1) y
    someta las amplitudes de todo el espectro a un test de hipótesis con un nivel de
    significancia estadística de 0.05, sin considerar el problema de multiplicidad de pruebas.
    Comente brevemente su resultado e interprete las diferencias entre los espectros de
    ambas variables.
3. Considerando ahora las series mensuales de caudal y precipitación en Trancura,
    disponibles en la misma base de datos, construya y evalúe un modelo de regresión lineal
    simple para anomalías mensuales de caudal en función de las anomalías de precipitación.
    Muestre las series de anomalías de caudal observado junto con su predicción y
    compárelas en diagrama de dispersión. ¿Cómo cambia el desempeño del modelo si se
    añaden como predictores anomalías de precipitación con desfase (-) de 1, 2 y 3 meses?
    Sin hacer un análisis mayor, comente respecto de los problemas de sobre-ajuste y multi-
    colinealidad en su modelo multivariado.
4. Finalmente, evalúe un modelo multivariado similar al anterior, pero calculado para cada
    mes del año de forma independiente. ¿Mejora la capacidad predictiva del caudal mensual
    con esta estrategia? ¿Cómo varía esta capacidad según la estación del año? Intente
    sintetizar su resultado en un sólo gráfico.