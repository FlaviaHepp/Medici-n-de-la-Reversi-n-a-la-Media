Medición de la Reversión a la Media
Desviación del Precio respecto a la SMA 200
📌 Descripción

Este proyecto identifica acciones que se encuentran significativamente alejadas de su valor de equilibrio de largo plazo, utilizando la Media Móvil Simple de 200 períodos (SMA 200) como referencia.

La hipótesis central es la de reversión a la media:
cuando el precio se desvía de forma extrema de su promedio histórico, aumenta la probabilidad de que:

el precio corrija (si está sobreextendido)

o rebote (si está excesivamente castigado)

🧠 Insight clave

¿Qué acciones están cotizando más de un ±10% respecto a su SMA 200, sugiriendo una posible reversión a la media?

Este tipo de desvíos no suelen sostenerse indefinidamente, especialmente en activos líquidos y seguidos por el mercado.

📊 Valor de negocio

Este análisis aporta valor en:

Identificación de oportunidades contrarias
Detectar activos potencialmente sobrevalorados o infravalorados.

Gestión de riesgo
Alertar sobre precios alejados de su zona de equilibrio.

Timing de entrada y salida
Complementar señales de momentum con señales de exceso.

Construcción de portafolios
Evitar sobreponderar activos con desvíos extremos.

🗂️ Estructura de datos requerida
indicadores_tecnicos

ticker_id

fecha

sma_200

precios_diarios

ticker_id

fecha

close

⚙️ Lógica del análisis

Precio actual

Se toma el precio de cierre del activo.

Referencia de largo plazo

Se utiliza la SMA 200 como proxy del valor medio.

Cálculo del desvío porcentual

(Precio − SMA_200) / SMA_200 × 100


Clasificación automática

+10% → Sobrevalorada (posible venta)

< −10% → Infravalorada (posible compra)

Dentro del rango → Zona normal

Filtrado

Se muestran solo desvíos absolutos mayores al 10%.

📈 Interpretación de resultados

Desvío positivo elevado

Precio extendido al alza

Riesgo de corrección

Desvío negativo elevado

Precio castigado

Potencial rebote técnico

Importante
La señal no implica reversión inmediata; debe confirmarse con:

Momentum

Volumen

Contexto macro o sectorial

🚀 Posibles extensiones

Ajustar umbral por volatilidad del activo

Combinar con RSI o ADX

Medir persistencia del desvío en el tiempo

Separar análisis por sector

Crear un Índice de Extremidad de Precio

🧪 Notas técnicas

Se recomienda indexar:

precios_diarios (ticker_id, fecha)

indicadores_tecnicos (ticker_id, fecha)

SMA 200 es un estándar, pero puede adaptarse (100 / 300) según horizonte.

Ideal para mercados líquidos y con histórico suficiente.# Medici-n-de-la-Reversi-n-a-la-Media
Medición de la Reversión a la Media
