---
marp: true
theme: custom
paginate: true
math: true
size: 16:9
---

<!--- Custom theme is declared below using Marp's style block. -->
<style>
/* Custom Marp theme: "custom" */
:root {
  --header-bg: #0b3d91;
  --accent: #00a3ff;
  --text: #f7f9fb;
  --muted: #bcd2ff;
}
section {
  font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
}
/* Title slide */
section.title {
  background: linear-gradient(135deg, var(--header-bg), #072b5b);
  color: var(--text);
}
/* Small accent boxes */
.box {
  display: inline-block;
  padding: 0.35rem 0.6rem;
  border-radius: 8px;
  background: rgba(255,255,255,0.04);
  color: var(--muted);
  font-size: 0.9em;
}
/* Make code blocks stand out */
pre,
code {
  background: rgba(0,0,0,0.5);
  border-radius: 6px;
  padding: 0.35rem;
}
/* Footer area for contact*/
footer {
  position: absolute;
  right: 1rem;
  bottom: 0.6rem;
  font-size: 0.85rem;
  color: rgba(255,255,255,0.75);
}
</style>

---
<!-- Title slide -->
<!-- class: title -->
# Product Documentation — **AwesomeApp**

> Maintainable docs for engineers, product, and QA

<div class="box">Version control + Marp</div>

<footer>Contact: 23f3000880@ds.study.iitm.ac.in</footer>

---

<!-- Agenda slide with custom styling -->
class: lead

## Agenda

- What this product does
- Development & deployment
- Architecture and algorithms
- How to contribute (version control)

---

## Quick install

```bash
# install marp CLI and render
npm install -g @marp-team/marp-cli
marp slides.md --pdf
```

Notes:
- Keep `slides.md` at repo root or `docs/` folder for GitHub Pages.

---

<!-- Background image slide: using an openly available image. Replace URL with your repo asset for offline builds. -->

class: lead
style: background-image: url('https://images.unsplash.com/photo-1518779578993-ec3579fee39f?auto=format&fit=crop&w=1600&q=80'); background-size: cover; background-position: center; color: white;

# Our product at a glance

> Streamlined pipelines, robust observability, and tiny deploys.

---

## Architecture (high level)

- Microservices: API, Worker, Auth, Metrics
- Data store: Postgres + Redis cache
- CI/CD: GitHub Actions -> Staging -> Production

---

## Algorithmic complexity (example)

We use a deduplication algorithm with average-case complexity shown below.

The common step is hashing each record then checking membership in a hash table (set):

\[
T(n) = O(n) \quad\text{(expected time for hashing + lookup for n items)}
\]

If we sort then dedupe (stable) we get:

\[
T(n) = O(n \log n)
\]

---

## Example: Pipeline latency estimation

Given M messages and W workers. A simple bound on throughput (assuming no contention):

\[
\text{throughput} = \frac{W}{\text{avg\\_service\\_time}}
\]

If service time scales with payload size \(s\) as \(O(s)\), then for \(M\) messages total work is \(O(Ms)\).

---

## Contributing

1. Fork the repo and create a topic branch `docs/feature-x`.
2. Update `slides.md` in `docs/` or repo root.
3. Open a PR and mention reviewers.

> Use `?v=1` query to bust caches when testing GitHub Pages (e.g., `slides.md?v=2`).

---

## Slide styling tips

- Use `class:` and `style:` slide attributes for ad-hoc tweaks.
- Put reusable CSS into a dedicated `.css` and include it when rendering: `marp --theme ./docs/marp-theme.css slides.md`.

---

<!-- Contact + footer with page number enabled by paginate: true above -->

# Contact & Resources

- Author: Technical Writing — Product Team
- Email: **23f3000880@ds.study.iitm.ac.in**
- Repo: Put `slides.md` in your GitHub repo and use the raw URL (see below)

---

class: center

# Thank you!

Questions? Ping: 23f3000880@ds.study.iitm.ac.in

