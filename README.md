# Simulador Eólico Interactivo — TecNM

[![Ver en vivo](https://img.shields.io/badge/Demo-Ver%20en%20Vivo-00e5a0?style=for-the-badge&logo=google-chrome&logoColor=black)](https://simuladorgeneradoreolico.netlify.app/)



Este es un simulador web desarrollado para la visualización y análisis del potencial energético eólico. La herramienta permite modelar el comportamiento de aerogeneradores considerando variables geográficas y físicas específicas de la región.

## ⚙️ Especificaciones Técnicas
* **Motor Gráfico:** HTML5 Canvas (renderizado a 60 FPS).
* **Base Física:** Ecuación de potencia aerodinámica con corrección por altitud.
* **Smart Grid:** Lógica de consumo distribuido (Alumbrado, Residencial, Industrial).
* **Reportes:** Exportación de datos de sesión mediante `Chart.js`.

## 📐 Parámetros de Simulación (Modelo Físico)

El simulador se rige bajo la siguiente fórmula de potencia eólica:

**P = 0.5 * ρ * A * v³ * Cp * η**

| Variable | Descripción | Valor / Fórmula |
| :--- | :--- | :--- |
| **ρ** (Rho) | Densidad del aire | 1.005 kg/m³ (Ags, 1888m) |
| **A** | Área de barrido | π * R² |
| **Cp** | Coeficiente de potencia | 0.45 (Práctico / Límite Betz) |
| **η** (Eta) | Eficiencia del generador | 0.92 (92%) |
| **Cut-in** | Velocidad de inicio de carga | 12.6 km/h |
| **Cut-out** | Velocidad de corte por seguridad | 90 km/
## 🗺️ Mapa de Ruta (Roadmap)
Planeamos seguir mejorando el simulador con las siguientes características:
- [ ] **Módulo de Baterías:** Simular un sistema de almacenamiento para la Smart Grid cuando no hay viento.
- [ ] **Historial Local:** Guardar los resultados de simulaciones pasadas usando `localStorage`.
- [ ] **Selector de Ciudades:** Permitir cambiar la altitud (modificando automáticamente la densidad del aire  **ρ**) para comparar Aguascalientes con ciudades costeras.
- [ ] **Modo Climático Automatizado:** Conectar una API de clima real para simular con el viento actual de la región
## 👥 Créditos y Autores
Desarrollado como proyecto académico para el **Instituto Tecnológico de Aguascalientes (TecNM)**.

* **Desarrollador:** [Ivan Dilan Picazo Flores](https://github.com/ivan)
* **Materia:** [Introduccion a la Fisica Aplicada en la Ciberseguridad ]
* **Profesor:** [Joseph Daniel Pineda Sandoval]





