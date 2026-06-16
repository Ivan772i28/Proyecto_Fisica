
# Simulador Eólico Interactivo — TecNM Aguascalientes

Este es un simulador web desarrollado para la visualización y análisis del potencial energético eólico. La herramienta permite modelar el comportamiento de aerogeneradores considerando variables geográficas y físicas específicas.

## ⚙️ Especificaciones Técnicas
* **Motor Gráfico:** HTML5 Canvas (renderizado a 60 FPS).
* **Base Física:** Ecuación de potencia aerodinámica con corrección por altitud.
* **Smart Grid:** Lógica de consumo distribuido (Alumbrado, Residencial, Industrial).
* **Reportes:** Exportación de datos de sesión mediante `Chart.js`.

## 📐 Parámetros de Simulación (Modelo Físico)
El simulador se rige bajo la fórmula:
$$P = \frac{1}{2} \cdot \rho \cdot A \cdot v^3 \cdot C_p \cdot \eta$$

| Variable | Descripción | Valor/Fórmula |
| :--- | :--- | :--- |
| $\rho$ | Densidad del aire | 1.005 kg/m³ (Ags, 1888m) |
| $A$ | Área de barrido | $\pi R^2$ |
| $C_p$ | Coeficiente de potencia | 0.45 (Práctico) |
| $\eta$ | Eficiencia | 0.92 |
| Cut-in | Velocidad de inicio | 12.6 km/h |
| Cut-out | Velocidad de corte | 90 km/h |
