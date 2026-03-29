# Suponiendo que tu modelo se llama 'm' y tu pronóstico 'forecast'
from prophet.plot import plot_plotly, plot_components_plotly

# 1. Guardar la gráfica principal
fig1 = m.plot(forecast)
fig1.savefig('coffee_forecast.png', dpi=300, bbox_inches='tight')

# 2. Guardar los componentes (Tendencia y Estacionalidad)
fig2 = m.plot_components(forecast)
fig2.savefig('coffee_trends.png', dpi=300, bbox_inches='tight')
