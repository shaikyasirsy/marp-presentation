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

## Agenda

- What this product does
- Development & deployment
- Architecture and algorithms
- How to contribute (version control)

---

## Quick install

```bash
npm install -g @marp-team/marp-cli
marp slides.md --pdf
```

---

---
backgroundImage: url('./bg.jpeg')
backgroundSize: cover
backgroundPosition: center
---

# Our product at a glance

> Streamlined pipelines, robust observability, and tiny deploys.

---

## Architecture (high level)

- Microservices: API, Worker, Auth, Metrics
- Data store: Postgres + Redis cache
- CI/CD: GitHub Actions -> Staging -> Production

---

## Algorithmic complexity (example)

\[
T(n) = O(n)
\]

\[
T(n) = O(n \log n)
\]

---

## Pipeline latency estimation

\[
\text{throughput} = \frac{W}{\text{avg\\_service\\_time}}
\]

For \(M\) messages, work is \(O(Ms)\).

---

## Contributing

1. Fork repo.
2. Edit `slides.md`.
3. PR with changes.

---

## Contact & Resources

- Email: **23f3000880@ds.study.iitm.ac.in**

---

# Thank you!

Questions? Ping: 23f3000880@ds.study.iitm.ac.in
