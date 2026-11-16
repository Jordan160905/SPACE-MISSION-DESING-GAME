# 🚀 NEXUS: Mission Control

**Diseña. Construye. Lanza. Descubre.**

Videojuego web 3D educativo creado para el **NASA Space Apps Challenge**. Diriges tu propia agencia espacial: diseñas una nave, la lanzas, viajas hasta la Luna, aterrizas, exploras con un rover y operas la misión. Todas las decisiones están conectadas por un motor de simulación con física real, explicada con palabras sencillas para niños y adultos sin conocimientos técnicos.

> Proyecto educativo independiente. No está afiliado a la NASA ni cuenta con su respaldo.

---

## ✨ Qué puedes hacer

| Etapa | En el juego |
|---|---|
| 🏢 **Mission Center** | Sala de mando en 3D. Eliges la misión LUNA-01, el modo (individual con tu nombre, o en equipo de 2 a 4 personas), la dificultad y el objetivo científico. |
| 🛠️ **Spacecraft Lab** | Construyes tu nave arrastrando piezas reales (instrumentos, paneles, baterías, antenas, propulsores…). Ves en vivo la masa, el coste, la energía y los datos. |
| 🔬 **Análisis y planificación** | El motor revisa tu diseño con fórmulas visibles. Eliges cohete, órbita, duración y ventana de lanzamiento. |
| 🎮 **Revisión** | Revisión gamificada para estudiantes, con un personaje que te guía. |
| 🚀 **Vuelo a la Luna** | Despegue y trayectoria Tierra → Luna con física real, cinco cámaras, telemetría completa y ventanas flotantes que puedes mover. |
| ⚠️ **Imprevistos** | Fallos de comunicación, calor, energía o desvíos que tienes que resolver, y a veces **contrarreloj** (15–25 s, configurable o desactivable). |
| 🔭 **Descubrimientos** | Satélites reales (ISS, Hubble, GPS…), asteroides, regiones lunares, constelaciones y nebulosas en su posición real. Los observas con la cámara y los guardas en tu diario de exploración, con su mapa. |
| 🛰️ **Rescate espacial** | Misión opcional: pilotas la nave para ayudar a un satélite averiado. Incluye tutorial. |
| 🌙 **Aterrizaje lunar** | Minijuego sencillo: mantén **ESPACIO** para frenar y usa las flechas para llegar a la zona verde. Si lo consigues hay cinemática; si fallas, el juego te explica qué mejorar. |
| 🚙 **Rover lunar** | Recoges los datos que pide tu misión (fotos, minerales o hielo), con mapa de exploración, energía solar y una pregunta científica. |
| 📊 **Operaciones e informe** | La nave trabaja en órbita y, al final, un avatar te muestra un **informe divertido**: qué pasó, qué encontraste, qué problemas hubo y cómo mejorar. |
| 🏅 **Logros** | 16 insignias, rangos **Bronce → Plata → Oro → Diamante** y una **clasificación** de puntuaciones de mayor a menor. |

El juego está en **español** y en **inglés**.

---

## 🧠 Ciencia real dentro del juego

- Gravedad lunar de 1,62 m/s², órbitas de Kepler y trayectoria Tierra–Luna calculada con física real.
- Ecuación del cohete (Tsiolkovsky) para el combustible y el Δv.
- Energía por órbita (paneles, baterías y eclipses), datos y comunicaciones.
- Satélites, estrellas y regiones lunares en sus posiciones reales.
- Cuando un dato es de juego o simulado, el juego lo indica.

---

## 🧰 Tecnologías

- [React 19](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/)
- [Vite](https://vitejs.dev/)
- [Three.js](https://threejs.org/) con [React Three Fiber](https://docs.pmnd.rs/react-three-fiber) y Drei (3D)
- [Zustand](https://zustand-demo.pmnd.rs/) (estado del juego)
- [Zod](https://zod.dev/) (validación del guardado)
- [Vitest](https://vitest.dev/) (pruebas)

---

## ▶️ Cómo ejecutarlo

Requisitos: **Node.js 20 o superior** y un navegador con WebGL (Chrome, Edge o Firefox actualizados).

```bash
git clone https://github.com/TU-USUARIO/nexus-mission-control.git
cd nexus-mission-control
npm install
npm run dev
```

Abre **http://localhost:5173** en el navegador.

Otros comandos:

```bash
npm test           # pruebas
npm run typecheck  # comprobación de tipos
npm run build      # versión de producción en dist/
npm run preview    # ver la versión de producción
```

---

## 🎮 Controles principales

| Momento | Teclas |
|---|---|
| Aterrizaje | **ESPACIO** motor · **flechas** mover · **P** pausa |
| Rover | **W/S** o **↑/↓** avanzar y retroceder · **A/D** o **←/→** girar · **E** acción · **C** cámara |
| Rescate | **flechas** girar · **W/S** avanzar o frenar · **A/D** y **R/F** desplazarse · **espacio** motor principal |

Todo también se puede hacer con los botones de la pantalla.

---

## 📁 Estructura del proyecto

```
src/
├── sim/      Motor de simulación (física, vuelo, eventos, aterrizaje, rover, logros)
├── state/    Estado del juego y guardado
├── scene/    Escenas 3D (centro de mando, laboratorio, lanzamiento, superficie lunar)
├── ui/       Pantallas e interfaz (HUD, paneles, minijuegos, informe)
├── data/     Misiones, componentes, cohetes y glosario
└── i18n/     Traducción al inglés
docs/         Fases, decisiones de diseño y supuestos
```

---

## 📸 Capturas

<!-- Sube tus imágenes a una carpeta docs/screenshots y cambia los nombres -->
![Centro de mando](docs/screenshots/centro.png)
![Aterrizaje lunar](docs/screenshots/aterrizaje.png)
![Informe y logros](docs/screenshots/logros.png)

---

## 👥 Equipo

<!-- Cambia esto por los nombres de tu equipo -->
- Nombre Apellido: rol
- Nombre Apellido: rol

---

## 📄 Licencia

<!-- Elige una licencia (por ejemplo MIT) y añade el archivo LICENSE -->
Este proyecto se distribuye bajo la licencia **MIT**. Consulta el archivo `LICENSE`.
