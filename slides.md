---
marp: true
theme: custom
paginate: true
math: true
size: 16:9
---

<style>
:root {
  --header-bg: #0b3d91;
  --accent: #00a3ff;
  --text: #f7f9fb;
  --muted: #bcd2ff;
}
section {
  font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
}
section.title {
  background: linear-gradient(135deg, var(--header-bg), #072b5b);
  color: var(--text);
}
.box {
  display: inline-block;
  padding: 0.35rem 0.6rem;
  border-radius: 8px;
  background: rgba(255,255,255,0.04);
  color: var(--muted);
  font-size: 0.9em;
}
pre,
code {
  background: rgba(0,0,0,0.5);
  border-radius: 6px;
  padding: 0.35rem;
}
footer {
  position: absolute;
  right: 1rem;
  bottom: 0.6rem;
  font-size: 0.85rem;
  color: rgba(255,255,255,0.75);
}
</style>

---
<!-- class: title -->
# Product Documentation — **AwesomeApp**

> Maintainable docs for engineers, product, and QA

<div class="box">Version control + Marp</div>

<footer>Contact: 23f3000880@ds.study.iitm.ac.in</footer>

---

## What is Marp?

Marp (Markdown Presentation) is a powerful tool to create presentations using Markdown. It supports:

- Technical presentations
- Documentation slides
- Academic and conference talks
- Teaching materials
- Hosting via GitHub Pages

---

## Installation

```bash
# Install Marp CLI globally
npm install -g @marp-team/marp-cli

# One-time use without install
npx @marp-team/marp-cli@latest

# Local project install
npm install --save-dev @marp-team/marp-cli
```

---
<!-- _backgroundImage: url('./bg.jpeg') -->
<!-- _backgroundSize: cover -->
<!-- _backgroundPosition: center -->
![bg](./bg.jpeg)
![bg fit](./bg.jpeg)
![bg cover](./bg.jpeg)

# Our product at a glance

> Streamlined pipelines, robust observability, and tiny deploys.

---

## Architecture (high level)

- Microservices: API, Worker, Auth, Metrics
- Data store: Postgres + Redis cache
- CI/CD: GitHub Actions -> Staging -> Production

---

## Algorithmic complexity example

Average-case deduplication complexity:

$$
T(n) = O(n) \\ \text{(hashing + lookup)}
$$

Sorting then deduplication:

$$
T(n) = O(n \\log n)
$$

---

## Pipeline latency estimation

Given $W$ workers and average service time:

$$
\\text{throughput} = \\frac{W}{\\text{avg\\_service\\_time}}
$$

For $M$ messages of size $s$, total work:

$$
O(Ms)
$$

---

## Best Practices

- Keep slides focused and minimal
- Use consistent styling
- Test output formats
- Optimize images before including

---

## Contact & Resources

- Email: **23f3000880@ds.study.iitm.ac.in**
- Repo contains `slides.md` and `bg.jpeg`

---

# Thank you!

Questions? Ping: **23f3000880@ds.study.iitm.ac.in**
