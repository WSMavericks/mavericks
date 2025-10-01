# WALL STREET MAVERICKS — Portal de Backtests y Recursos

Bienvenido a la **sala central** de WALL STREET MAVERICKS: aquí encontrarás los backtests de nuestros bots de trading, afiliaciones y partners, cursos y formaciones, calendario económico, y recursos para contribuir o replicar nuestros resultados.

---

## Índice

1. [Sobre este portal](#sobre-este-portal)
2. [Backtests y resultados](#backtests-y-resultados)
3. [Bots y repositorios](#bots-y-repositorios)
4. [Afiliaciones y partners](#afiliaciones-y-partners)
5. [Cursos y formaciones](#cursos-y-formaciones)
6. [Calendario económico](#calendario-económico)
7. [Cómo reproducir un backtest](#cómo-reproducir-un-backtest)
8. [Contribuir / Pull requests](#contribuir--pull-requests)
9. [Licencia y responsabilidad](#licencia-y-responsabilidad)
10. [Contacto](#contacto)

---

## Sobre este portal

Este repositorio actúa como **portal público** donde divulgamos:

* Resultados de backtests de nuestros bots (metodología y código reproducible).
* Material formativo (cursos, guías, notebooks).
* Enlaces a afiliaciones, herramientas y proveedores de datos.
* Un calendario económico integrado con eventos relevantes para trading.

> Nota: los resultados mostrados son educativos y de investigación; no constituyen asesoramiento financiero.

---

## Backtests y resultados

Cada backtest tiene su propia carpeta con:

* `README.md` con resumen ejecutivo (periodo, activo, timeframe, parámetros).
* Código reproducible (Python / Jupyter notebooks).
* CSV con métricas (CAGR, drawdown máximo, Sharpe, trades, etc.).
* Gráficas y reportes en HTML/PDF.

**Estructura de ejemplo:**

```bash
/backtests
  /mean-reversion-bot
    README.md
    backtest.ipynb
    results.csv
    equity_curve.png
  /trend-following-bot
    README.md
    backtest.py
    report.html
```

**Ejemplo de tabla de resumen (en README principal):**

| Bot       | Período   | Activo    | CAGR anual | Máx Drawdown | Sharpe | Estado        |
| --------- | --------- | --------- | ---------- | ------------ | ------ | ------------- |
| MR-BOT v1 | 2018–2024 | EURUSD H1 | 18.5%      | -12.4%       | 1.45   | ✅ Publicado   |
| TF-BOT v2 | 2017–2024 | SPX D     | 14.2%      | -20.1%       | 0.95   | 🧪 En testing |

---

## Bots y repositorios

Cada bot tiene un repositorio/paquete propio con:

* Código modular y requisitos (`requirements.txt` / `pyproject.toml`).
* Tests mínimos y ejemplo de uso.
* Notebooks para exploración de parámetros.

**Tips para mantener repositorios de bots:**

* Versiona los parámetros (semántico: v1.0.0).
* Incluye seeds y versiones de librerías para reproducibilidad.
* Documenta la fuente de datos (proveedor, símbolo, ajuste por dividendos, timezone).

---

## Afiliaciones y partners

En esta sección listamos las plataformas y servicios con los que trabajamos (con transparencia sobre los beneficios de afiliación):

* Proveedor de datos X — calidad intradiaria (enlace y nota sobre coste).
* Plataforma de ejecución Y — latencia y coste por orden.

> Transparencia: siempre indicaremos si recibimos comisiones por enlaces de afiliado.

---

## Cursos y formaciones

Ofrecemos cursos y mini-bootcamps orientados a traders cuantitativos:

* **Introducción al backtesting reproducible** — notebooks, datasets, ejercicios.
* **Optimización y prevención de sobreajuste** — técnicas y checklists.
* **Automatización y despliegue** — desde pruebas a live trading.

Cada curso tendrá su propia landing con temario, duración y requisitos.

---

## Calendario económico

Integraremos un calendario económico con filtros por país, impacto y tipo de evento. En `docs/calendario/` habrá scripts que consumen APIs públicas (o archivos CSV actualizados) y generan vistas filtrables.

**Cómo presentarlo:**

* Tabla resumida en README (próximos 7 días).
* Link a una vista interactiva (HTML) dentro del repositorio.

---

## Cómo reproducir un backtest

1. Clona el repo:

   ```bash
   git clone https://github.com/tu-usuario/mavericks-portal.git
   ```
2. Crea y activa un entorno virtual:

   ```bash
   python -m venv .venv
   source .venv/bin/activate  # macOS / Linux
   .\.venv\Scripts\activate  # Windows
   pip install -r requirements.txt
   ```
3. Descarga los datos (script `scripts/download_data.py` o indica proveedor).
4. Ejecuta:

   ```bash
   python run_backtest.py --bot mean-reversion --from 2018-01-01 --to 2024-12-31
   ```
5. Revisa `results/` y el `report.html` generado.

---

## Contribuir / Pull requests

¡Contribuciones bienvenidas! Para colaborar:

1. Haz fork del repo.
2. Crea una rama `feature/tu-idea`.
3. Añade tests mínimos y documentación.
4. Crea un PR describiendo el cambio y su impacto en resultados.

Añade un issue antes de implementar cambios grandes en la metodología de backtesting.

---

## Licencia y responsabilidad

* Licencia: [MIT] (o la que prefieras).
* Disclaimer: todo contenido es educativo; no somos asesores financieros. Los usuarios asumen la responsabilidad de usar los resultados.

---

## Contacto

* Instagram / TikTok: `@wallstreetmavericks`
* Email: `contacto@wallstreetmavericks.example`

---

### Última nota

Esta portada sirve como **plantilla** y guía de organización para el portal en GitHub.

> Hecho con ❤️ por WALL STREET MAVERICKS
