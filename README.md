### Hi, I'm Philip 👋

Day to day, I'm a data and software engineer in financial markets. Outside of work I train a lot (mainly CrossFit and running/cycling) and build apps: I've got a couple currently, one to do with personal investing, and one making sense of my training schedule and goals.

Most of my repositories are private, as they hold my own financial and health data, but I wanted to give an overview of some of the things I get up to.

I plan in the near future to open source the non-sensitive functionality and app frontends to give you a better idea of what I'm doing.

#### Markets & money

This is where most of my spare-time energy goes, building the tools I wished existed for keeping on top of my own finances.

**finance-analysis** *(private, Python)* started as a script and has grown into a proper personal-finance platform:

- **Portfolio tracker** (Streamlit): Imports transactions from UK brokers (contract notes or CSVs, multiple providers), updates prices daily, and works out time- and money-weighted returns, Sharpe, Sortino, Calmar, drawdown, beta and tracking error. There's a demo mode with an invented portfolio, so I can show it without showing mine!
- **Spending viewer**: Sorts card transactions by merchant and shows budget-vs-actual (reads CSV files).
- **Wealth projection**: For the longer-term what-ifs.
- **Fund-overlap agent** *(experimental)*: A Claude tool-use loop that checks a fund's factsheet against my holdings, so I don't end up with two similar funds where one is 5x more expensive (it's happened).

The bit I care about most is whether the numbers are right. The transaction ledger is checked daily against my recorded holdings, and there are 2,700+ automated tests.

When a number turns out wrong, I write up why and add a check that would have caught it.

**[src](https://github.com/philip-papasavvas/src)** *(public, Python)* is the maths I like underneath all this: returns, risk ratios, stationarity and the efficient frontier, as a small package with tests and CI.

#### Training & health

Anyone that knows me, knows that I like to optimise my health, whether it's sleep, gym or nutrition.

**personal-fitness** *(private, JavaScript/TypeScript)* is my own training app, for CrossFit, running and HYROX:

- It works offline on my phone (Cloudflare Workers), with Strava sync, and sleep and recovery data from my Garmin through Apple Health.
- A Claude coach suggests changes to my plan, but nothing changes until I say yes.
- There's a searchable library of gym workouts.

#### Machine learning & AI

Way back when, I learned by building rather than reading about it.

- **[ml_sandbox](https://github.com/philip-papasavvas/ml_sandbox)** *(public)*: An SMS spam classifier (NLP) and PCA on the breast-cancer dataset.
- **[founders-ai-day](https://github.com/philip-papasavvas/founders-ai-day)** *(public)*: Prototypes from a day of building with other founders ([live demos here](https://founders-ai-day-demos.netlify.app/)).

#### How I work with AI

I use Claude Code most days, and Google Antigravity and T3 Code as well. The arithmetic stays in tested code, and the model gets the judgement calls.

Anything that goes wrong gets written into the repository, so it (hopefully) doesn't happen twice.

#### Toolbox

- **Languages**: Python (pandas, numpy, scikit-learn), SQL, JavaScript/TypeScript, HTML, CSS
- **Data & pipelines**: ETL/ELT, Dagster, SQL Server, Oracle, PostgreSQL, SQLite/libSQL
- **Cloud & infra**: AWS, Azure, Cloudflare Workers, Docker, Kubernetes, Helm, GitOps, CI/CD (GitHub Actions)
- **Front-end**: Streamlit, Dash/Plotly, AG Grid, React
- **AI**: Claude API (tool use, agents), MCP servers
- **AI coding tools**: Claude and Claude Code, Google Antigravity, T3 Code

---

Always happy to talk data, markets or personal health! Find me on [LinkedIn](https://www.linkedin.com/in/philippapasavvas/).
