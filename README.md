# 🔬 Física & Mecánica Interactiva

Una plataforma web interactiva, moderna y didáctica para aprender física clásica, termodinámica, mecánica de fluidos y principios aeronáuticos mediante simulaciones interactivas en tiempo real renderizadas a 60 FPS con HTML5 Canvas y Tailwind CSS.

---

## 🚀 Temas y Simulaciones Incluidas

### 1. ⚙️ Motor a Pistón de 4 Tiempos (Ciclo Otto)
- **Cinemática completa del mecanismo biela-manivela y árbol de levas superior**:
  - Pistón forjado con 3 aros de compresión/aceite, bulón con buje de bronce y falda estilizada.
  - Válvulas con resortes helicoidales accionadas por levas excéntricas a relación 1:2.
  - Inyección de combustible atomizado y deflagración con partículas y chispas.
- **Los 4 tiempos del ciclo (720° de giro del cigüeñal)**:
  1. **Admisión (0° - 180°):** Apertura sincronizada de la válvula de admisión, descenso de PMS a PMI y aspiración de la mezcla.
  2. **Compresión (180° - 360°):** Cierre hermético de válvulas, ascenso del pistón y aumento de presión y temperatura.
  3. **Explosión / Combustión (360° - 540°):** Chispa de alta tensión en la bujía, deflagración de la mezcla y descenso forzado del pistón (¡único tiempo que genera trabajo motriz!).
  4. **Escape (540° - 720°):** Apertura de la válvula de escape y evacuación de gases quemados.
- **Interactividad Estable (Zero Jitter):** Control de RPM, avance paso a paso (+15°), scrubber manual de 0° a 720°, y detección interactiva por puntero (hover) con fichas técnicas.

### 2. 🚛 Inercia y Marcos de Referencia (El Salto en el Tráiler)
- Explicación y resolución del dilema clásico: *¿Qué ocurre si saltas dentro de un camión que viaja a 100 km/h?*
- Principio fundamental de la **1ª Ley de Newton (Inercia)**: Al estar dentro del camión, el cuerpo y el aire encerrado ya comparten la velocidad horizontal ($v_x = 100\text{ km/h}$). Al brincar verticalmente, no existe ninguna fuerza neta horizontal ($F_x = 0$), por lo que se aterriza en el mismo punto exacto.
- **Interactividad:**
  - Alternancia entre **Marco de Referencia Externo** (observador en la carretera: trayectoria parabólica) y **Marco de Referencia Interno** (observador dentro del camión: salto vertical puro).
  - Escenarios dinámicos:
    - 🟢 *Velocidad Constante:* Inercia perfecta.
    - 🛑 *Frenazo en el aire:* El camión desacelera pero el saltador conserva su velocidad, desplazándose hacia adelante.
    - ⚡ *Aceleración brusca:* El camión se adelanta y el saltador cae hacia atrás.
    - 💨 *Plataforma abierta (pickup):* La resistencia del viento exterior frena al saltador.
  - Telemetría en tiempo real: velocímetro, vector de velocidad $v_x$, vector $v_y$ y desplazamiento de aterrizaje.

### 3. 🌊 Presión Atmosférica vs. Presión Hidrostática
- Comparación entre la columna de aire (gas compresible) y la masa oceánica (líquido incompresible 800 veces más denso).
- **Regla de oro:** Cada ~10 metros de profundidad de agua marina suman **+1 atmósfera** de presión adicional.
- **Interactividad:**
  - Sonda vertical continua desde la cima del Monte Everest (+8,848 m) hasta las profundidades abisales de la Fosa de las Marianas (-10,928 m / >1,085 atm).
  - Simulación física de la **Ley de Boyle ($P \cdot V = \text{cte}$)**: globo flexible que se expande en la estratosfera y se comprime drásticamente bajo el agua.
  - Conversión instantánea de unidades: **atm**, **kPa**, **bar** y **psi**.
  - Hitos rápidos: Everest, CDMX / Bogotá, Nivel del Mar, Buceo recreativo (-30m), Zona crepuscular (-100m), Naufragio del Titanic (-3,800m) y Fosa de las Marianas (-10,928m).

### 4. ✈️ Altura vs. Altitud (AGL vs. MSL)
- Claridad conceptual aeronáutica y topográfica:
  - **MSL (Mean Sea Level - Altitud):** Distancia vertical desde el nivel medio del mar hasta el avión (medida con altímetro barométrico ajustado a QNH).
  - **AGL (Above Ground Level - Altura):** Distancia vertical real entre el avión y el terreno que sobrevuela directamente debajo (medida con radioaltímetro).
  - **Elevación del Terreno:** Cota del relieve o de la pista sobre el nivel del mar.
  - Relación: $\text{Altura (AGL)} = \text{Altitud (MSL)} - \text{Elevación Terreno}$.
- Alerta didáctica sobre el peligro de **CFIT** (*Controlled Flight Into Terrain*).
- **Interactividad:**
  - Avión navegable sobre relieve dinámico (océano, llanuras costeras, cordilleras montañosas con nieve y meseta aeroportuaria).
  - Brackets de medición visual en vivo para Altitud (MSL), Altura (AGL) y Elevación.
  - Sistema de Alerta de Proximidad al Terreno (**GPWS**) con advertencia acústica/visual `"PULL UP! TERRAIN AHEAD!"` cuando la altura AGL es inferior al umbral de seguridad.
  - Modo piloto automático y presets de aproximación.

### 5. 💧 Flujo Laminar vs. Flujo Turbulento
- Dinámica del Número de Reynolds ($Re = \frac{\rho v D}{\mu}$):
  - **Régimen Laminar ($Re < 2,300$):** Capas de fluido deslizándose en láminas paralelas suaves sin mezclarse.
  - **Régimen Turbulento ($Re > 4,000$):** Inestabilidades, vórtices alternantes de Von Kármán y mezcla caótica.
- **Simulador Interactivo:**
  - **Modo Túnel Hidrodinámico:** Flujo alrededor de un cilindro con inyección de tinte de colores y formación de estela de vórtices.
  - **Modo Chorro Laminar:** Efecto de "Agua Congelada" donde el chorro parece una vara sólida de cristal hasta que se perturba con el dedo.
  - Selector de fluidos reales (Agua, Aceite, Glicerina ultra viscosa, Aire).

---

## 🛠️ Tecnologías Utilizadas

- **HTML5 Semántico**: Estructura accesible y modular en un solo archivo `index.html`.
- **Tailwind CSS**: Diseño moderno, temas oscuros, estética glassmorphism y adaptabilidad responsiva completa.
- **JavaScript Moderno (ES6+)**: Motores de animación a 60 FPS con `requestAnimationFrame` y cinemática en Canvas 2D.
- **Zero Dependencias Pesadas**: Carga instantánea y compatibilidad universal con navegadores de escritorio y móviles.

---

## 📄 Licencia

Este proyecto está distribuido bajo la licencia MIT.
