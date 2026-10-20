<!-- Header banner -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Saim%20Mehmood&fontSize=48&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=ML%20Platform%20%E2%80%A2%20AI%20Agents%20%E2%80%A2%20Infrastructure&descAlignY=58&descSize=18" alt="Saim Mehmood banner" />
</p>

<!-- Typing animation -->
<p align="center">
  <a href="https://github.com/saimmehmood">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1000&color=36BCF7&center=true&vCenter=true&width=600&lines=ML+Platform+Engineer+%40+Apple+(contract);Building+AI+agents+that+actually+ship;Voice+agents+%E2%80%A2+LLM+tooling+%E2%80%A2+ML+pipelines;MSc+Computer+Science+%40+York+University;Based+in+Toronto%2C+Canada+%F0%9F%87%A8%F0%9F%87%A6;Open+to+new+opportunities!" alt="Typing SVG" />
  </a>
</p>

<!-- Badges -->
<p align="center">
  <a href="https://www.linkedin.com/in/saimmehmoodgul/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://saimmehmood.github.io"><img src="https://img.shields.io/badge/Website-000000?style=for-the-badge&logo=githubpages&logoColor=white" alt="Website"/></a>
  <a href="mailto:saim.mehmood.gul@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <img src="https://komarev.com/ghpvc/?username=saimmehmood&style=for-the-badge&color=2c5364&label=Profile+views" alt="Profile views"/>
</p>

---

## 👋 About me

```python
class SaimMehmood:
    role       = "ML Platform Engineer @ Apple (contract, Jun 2026 – present)"
    location   = "Toronto, Canada 🇨🇦"
    education  = "MSc Computer Science, York University"
    focus      = ["ML platform engineering", "LLM agents", "Infrastructure correctness", "Spatial data mining"]
    building   = ["Voice agents for appointment booking", "AI resume tailoring", "Community scheduling apps"]
    research   = ["Trajectory analysis", "POI clustering", "Semantic relationships between regions"]
    motto      = "When a system says 'fine', go check whether it means it."
    open_to    = "Full-time roles & interesting collaborations"
```

## 💼 Now: ML Platform Engineer @ Apple

<p>
  <img src="https://img.shields.io/badge/PRs_authored-214-2a78d6?style=flat-square" alt="214 PRs authored"/>
  <img src="https://img.shields.io/badge/PRs_reviewed-287-eb6834?style=flat-square" alt="287 PRs reviewed"/>
  <img src="https://img.shields.io/badge/capacity_changes-200%2B-1baf7a?style=flat-square" alt="200+ capacity changes"/>
  <img src="https://img.shields.io/badge/dead_code_removed-~31k_lines-4a3aa7?style=flat-square" alt="~31k lines removed"/>
</p>

I work on internal AI/ML data infrastructure (contract, June 2026 to now). The common thread is **catching silent failures**, where a system reports success but quietly did the wrong thing.

- 🤖 **Built an LLM advisory agent.** On an internal time-series forecasting platform, it recommends a forecasting model for a team's data and declines when the data can't support a recommendation. I built the pipeline, the chat UI, and mutual-TLS service authentication from inside Ray Serve.
- 🧹 **Ran a tech-debt audit.** It removed ~27% of a repo (~31k lines of dead code) across five reviewed PRs. I proved the built images were byte-identical before and after. I was also the #2 reviewer of 10 engineers on that repo.
- ⚙️ **Ran capacity operations on a shared batch-compute cluster.** I made 200+ capacity changes, then fixed the provisioning tooling bugs those operations exposed. I became the #2 contributor on the main tool.
- 🖥️ **Took over a self-service capacity portal.** I went from first-time user to primary contributor in five weeks, with 21 PRs, all merged.

<details>
<summary><b>🔍 Two bugs I'm proud of catching</b> (click to expand)</summary>
<br/>

**"Memory request: 0Gi."** A confirmation prompt said a namespace I was about to drain was empty. It actually held ~10,600 GiB. The parser stripped unit suffixes with a string replace and threw away the parse error, so any value in `Mi` or `Ti` became zero. I fixed it and replayed the fix across 534 config files and 2,876 values. Exactly two changed, and both were the bug. I then found the same bug class three more times.

**Jobs that don't fail; they just sit.** Shrinking a queue needs the opposite step order from growing one. The portal's main button always used the grow order. During a reduction, a queue could advertise capacity that nothing backed, so jobs were accepted and then waited forever with no alert. Now the step order is computed and stored when the request is created, so the most-used path can't produce a silently broken queue.

</details>

## 🛠️ Tech stack

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=py,go,ts,js,scala,cs,cpp,html,css,react,nodejs,tensorflow,pytorch,sklearn,kubernetes,docker,git,linux&perline=9" alt="Tech stack" />
  </a>
</p>

## 🚀 Featured projects

<p align="center">
  <a href="https://github.com/saimmehmood/pharmacy-appointment-agent">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=saimmehmood&repo=pharmacy-appointment-agent&theme=tokyonight&hide_border=true" alt="pharmacy-appointment-agent" />
  </a>
  <a href="https://github.com/saimmehmood/ai_resume_tailor">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=saimmehmood&repo=ai_resume_tailor&theme=tokyonight&hide_border=true" alt="ai_resume_tailor" />
  </a>
  <a href="https://github.com/saimmehmood/semantic_relationships">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=saimmehmood&repo=semantic_relationships&theme=tokyonight&hide_border=true" alt="semantic_relationships" />
  </a>
  <a href="https://github.com/saimmehmood/ghusul_app">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=saimmehmood&repo=ghusul_app&theme=tokyonight&hide_border=true" alt="ghusul_app" />
  </a>
</p>

<details>
<summary><b>🤖 AI & agents</b> (click to expand)</summary>
<br/>

| Project | What it does |
|---|---|
| [pharmacy-appointment-agent](https://github.com/saimmehmood/pharmacy-appointment-agent) | Voice-ready conversational agent on Retell AI that books pharmacy appointments |
| [ai_resume_tailor](https://github.com/saimmehmood/ai_resume_tailor) | Uses LLMs to tailor a resume to a specific job description |
| [ai_engineer_assessment](https://github.com/saimmehmood/ai_engineer_assessment) | AI engineering take-home work |
| [nlp_squad](https://github.com/saimmehmood/nlp_squad) | Fixed-up BERT question-answering tutorial on SQuAD |

</details>

<details>
<summary><b>🗺️ Research: spatial & trajectory data mining</b></summary>
<br/>

| Project | What it does |
|---|---|
| [semantic_relationships](https://github.com/saimmehmood/semantic_relationships) | Learns semantic relationships between geographic areas from moving-object trajectories |
| [POI_Clustering](https://github.com/saimmehmood/POI_Clustering) | Clusters points of interest to characterize regions |
| [covid_19_risk](https://github.com/saimmehmood/covid_19_risk) | Uses trajectories to estimate the COVID-19 infection risk of geographic areas |
| [location-based-services](https://github.com/saimmehmood/location-based-services) | Location-based services experiments |
| [ExpertDeveloperRecommendation](https://github.com/saimmehmood/ExpertDeveloperRecommendation) | Search engine for finding expert developers by skill |

</details>

<details>
<summary><b>🧩 Apps & tools</b></summary>
<br/>

| Project | What it does |
|---|---|
| [ghusul_app](https://github.com/saimmehmood/ghusul_app) | Community app for scheduling Ghusul volunteers |
| [bookmark_manager](https://github.com/saimmehmood/bookmark_manager) | Chrome extension that organizes bookmarks by year, month & topic |
| [leet_code_solutions](https://github.com/saimmehmood/leet_code_solutions) | My LeetCode & CodeSignal solutions |

</details>

## 📊 GitHub stats

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=saimmehmood&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" alt="GitHub stats" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=saimmehmood&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=saimmehmood&theme=tokyonight&hide_border=true" alt="GitHub streak" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=saimmehmood&theme=tokyo-night&hide_border=true&area=true" alt="Contribution graph" />
</p>

<!-- Contribution snake (generated daily by .github/workflows/snake.yml) -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/saimmehmood/saimmehmood/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/saimmehmood/saimmehmood/output/github-snake.svg" />
    <img alt="Contribution snake" src="https://raw.githubusercontent.com/saimmehmood/saimmehmood/output/github-snake.svg" />
  </picture>
</p>

## 🤝 Let's connect

I'm **open to work**. If you're hiring for ML platform, infrastructure, or AI engineering, or want to collaborate on agents or spatial data, reach out on [LinkedIn](https://www.linkedin.com/in/saimmehmoodgul/) or [email](mailto:saim.mehmood.gul@gmail.com).

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=120&section=footer" alt="footer" />
</p>
