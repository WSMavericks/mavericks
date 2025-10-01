<p align="center">
  <img src="logo.png" alt="Wall Street Mavericks" width="220"/>
</p>

<h1 align="center">WALL STREET MAVERICKS</h1>
<h3 align="center">Portal de Backtests, Bots y Formación</h3>

---

## Sobre este portal

Este repositorio centraliza:

- 📊 Backtests de estrategias de trading algorítmico  
- 🤖 Repositorios de bots con código reproducible  
- 🎓 Material educativo y cursos de formación  
- 📅 Calendario económico interactivo  
- 🤝 Afiliaciones con plataformas y proveedores de datos  

> **Nota**: Toda la información es educativa y no constituye asesoramiento financiero.

---

## Backtests y resultados

Ejemplo de tabla resumen:

| Bot          | Período   | Activo   | CAGR anual | Máx Drawdown | Sharpe | Estado       |
|--------------|-----------|----------|------------|--------------|--------|--------------|
| MR-BOT v1    | 2018–2024 | EURUSD H1 | 18.5%      | -12.4%       | 1.45   | Publicado ✅ |
| TF-BOT v2    | 2017–2024 | SPX D    | 14.2%      | -20.1%       | 0.95   | En testing 🔎 |

Ejemplo de estructura de carpetas:

/backtests
/mean-reversion-bot
README.md
backtest.ipynb
results.csv
equity_curve.png

yaml
Copiar código

<p align="center">
  <img src="assets/sample_equity_curve.png" alt="Ejemplo Equity Curve" width="500"/>
</p>

---

## Cursos y formaciones

Ofrecemos formaciones en:

- **Introducción al backtesting reproducible** (Jupyter Notebooks, datasets)  
- **Prevención de sobreajuste** (validación cruzada, walk-forward analysis)  
- **Automatización** (de backtests a ejecución en tiempo real)  

Cada curso contará con su propia landing page y materiales descargables.

---

## Calendario económico

En `docs/calendario/` encontrarás:

- Scripts para consumir APIs públicas de datos económicos  
- Tablas filtrables (HTML)  
- Exportación a CSV  

<p align="center">
  <img src="assets/sample_calendar.png" alt="Calendario Económico" width="600"/>
</p>

---

## Cómo reproducir un backtest

```bash
git clone https://github.com/tu-usuario/mavericks-portal.git
cd mavericks-portal
python -m venv .venv
source .venv/bin/activate  # macOS/Linux
.venv\Scripts\activate     # Windows
pip install -r requirements.txt
python run_backtest.py --bot mean-reversion --from 2018-01-01 --to 2024-12-31
Los resultados se guardarán en /results con reportes en HTML/PDF.

Contribuir
Haz un fork del repositorio

Crea una rama feature/tu-idea

Documenta y añade tests mínimos

Envía un Pull Request

Licencia y responsabilidad
Licencia: MIT

Todo el contenido es educativo. Los resultados no son recomendación financiera.

Contacto
Instagram / TikTok: @wallstreetmavericks

Email: contacto@wallstreetmavericks.example
