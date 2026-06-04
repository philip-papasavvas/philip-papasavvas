### Hi, I'm Philip 👋

During the day I work with data, in financial markets. Outside of work, I build for fun, usually quite a lot- something to do with  financial markets, exploring the capabilities of Claude Code to assist me with admin, or making sense of my own health data.

Most of my repositories are private, due to the nature of information contained in them, which is personal, but I wanted to give an overview of some of the things I get up to.

#### Markets & money
This is where most of my spare-time energy — building the tools I wished
existed for keeping on top of my own finances.

- *finance-analysis* *(private)* — what started as a script has grown into a
  proper personal-finance platform, as an alternative to Kubera (for tracking investments and bank accounts):
  - a **portfolio tracker** (multi-page Streamlit app, which looks similar to the terminal) that
    imports transactions from UK brokers (as contract notes, or CSVs), auto-updates prices (using yfinance),
    and runs the full set of performance metrics — time- and money-weighted returns, CAGR, Sharpe,
    Sortino, max drawdown, volatility, VaR, alpha/beta. This allows me to analyse how different constituents in
    the portfolio are performing, as well as calculating the correlation of different funds to each other
    to make sure I'm not too overexposed in one area, or have redundant funds that are very highly correlated, and one fund is 5x
    more expensive than another (it's happened)
  - a **spending viewer** that classifies card transactions by merchant and shows
    budget-vs-actual (usually over budget) and where the money's actually going
  - a **fund-overlap agent** — a Claude tool-use agent that works out how much two
    funds really hold in common (to ensure I'm not buying redundant funds which overalap, helps simplify mental clarity)
  - a **wealth projection** model for the longer-term what-ifs
  - the plumbing behind it: SQLite, deployed on Google Cloud Run with Litestream
    replication, plus a demo mode so it can be shown without real positions
- **[src](https://github.com/philip-papasavvas/src)** *(public)* — the maths I
  like underneath all this: stationarity, return distributions, the efficient
  frontier.
#### Machine learning
Way back when, I learned by building rather than reading about it.
- **[ml_sandbox](https://github.com/philip-papasavvas/ml_sandbox)** — an SMS spam
  classifier (NLP) and PCA on the breast-cancer dataset.

#### Quantified self
Anyone that knows me, knows that I like to optimise my health - whether it's sleep, gym, or nutrition. Luckily, since I have multiple wearables, they have APIs which allow me to write code to make sense of what they spit out
— training load, recovery, and the occasional "is this actually working?".
- Personal dashboards pulling from **Strava, Garmin, Oura and WHOOP** *(private)*.

#### Other bits 
There are some general utilities I have that assist in my new repositories. 

#### Founders' AI day
- **[founders-ai-day](https://github.com/philip-papasavvas/founders-ai-day)** — a
  space to bring ideas together with others building in AI.

#### Also on the go
A few things that don't have a public home yet, but keep me busy:

- A property feasibility / development-appraisal tool for sizing up sites.
- A weekly planner that tracks workstreams across the projects I've got running.
- A running set of notes and algorithms picked up from my work.

#### Toolbox
Mostly Python and SQL, with whatever else the job needs:

- **Languages & data** — Python (pandas, numpy, scikit-learn), SQL, SQLite,
- **Web & front-end** — JavaScript, HTML, CSS; building marketing sites and small web apps
- **Pipelines** — ETL/ELT, Dagster, cross-database wrangling
- **Cloud & infra** — AWS, Azure, GCP (Cloud Run), Docker, Kubernetes, Helm, GitOps, CI/CD
- **Dashboards** — Streamlit, Dash/Plotly, AG Grid
- **AI** — building agents on the Claude API (tool-use), and a quite a lot of Claude Code
---

Always happy to talk data, markets, or personal health — find me on
[LinkedIn](https://www.linkedin.com/in/philippapasavvas/).
