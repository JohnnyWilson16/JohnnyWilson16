<div align="center">

# Hi, I'm Johnny Wilson Dougherty

<p align="center">
  <b>AI/ML engineer building agentic RAG systems, LLM-assisted data pipelines, and data-quality tooling.</b>
</p>

<p align="center">
  <a href="https://linkedin.com/in/johnny-wilson-dougherty-81693b292"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:johnnydougherty09@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

</div>

## 📌 About Me

- 🛡️ **Maintainer of [FreshData](https://github.com/FreshCode-Org/freshdata)**: explainable data cleaning for pandas and Polars, published on PyPI as [`freshdata-cleaner`](https://pypi.org/project/freshdata-cleaner/). I wrote most of the codebase (~480 commits, 95 merged PRs) and review outside contributions.
- 🌐 **13 merged upstream PRs** in projects I don't maintain, including [CPython](https://github.com/python/cpython/pull/158962), [pandas](https://github.com/pandas-dev/pandas/pull/70838), [TensorFlow](https://github.com/tensorflow/tensorflow/pull/129229), [Ultralytics](https://github.com/ultralytics/ultralytics/pull/26711), [Docling](https://github.com/docling-project/docling/pull/4240) and [AutoGPT](https://github.com/Significant-Gravitas/AutoGPT/pull/14875). Full list below.
- 🛠️ Python, FastAPI, Pydantic, pandas, Polars, DuckDB, LangChain, CrewAI, ChromaDB, Ollama, Pytest.
- 🎯 Open to full-time AI/ML roles (remote or onsite) and freelance GenAI / data engineering work.

---

## 🚀 Projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3 align="center">🛡️ <a href="https://github.com/FreshCode-Org/freshdata">FreshData</a> (maintainer)</h3>
      <ul>
        <li>Explainable, automated data cleaning for pandas and Polars, with DuckDB support.</li>
        <li>Schema-preserving Polars/DuckDB bridges, semantic and per-field validation, text sanitizers and privacy filters.</li>
        <li>Benchmark suite, streaming telemetry, and PyPI Trusted Publishing CI/CD.</li>
        <li><b>Looking for contributors:</b> see the <a href="https://github.com/FreshCode-Org/freshdata/issues">open issues</a>.</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3 align="center">🤖 <a href="https://github.com/JohnnyWilson16/agentic-rag-system">Agentic RAG System</a></h3>
      <ul>
        <li>Agentic RAG over financial reports (CrewAI, LangChain, ChromaDB) that plans queries, checks evidence and cites sources.</li>
        <li>Local-first: inference runs through Ollama, and the config rejects non-local LLM endpoints.</li>
        <li>Three-tier guardrails (input, retrieval confidence, output grounding) with a pytest suite.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3 align="center">🔄 <a href="https://github.com/JohnnyWilson16/self-healing-data-pipeline">Self-Healing Data Pipeline</a></h3>
      <ul>
        <li>Detects upstream schema drift and remaps column headers at runtime instead of failing the job.</li>
        <li>Layered resolution: exact match → mapping cache → heuristics/fuzzy match → LLM fallback.</li>
        <li>LLM prompts contain only column names and expected types, never row values.</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3 align="center">📊 <a href="https://github.com/JohnnyWilson16/complaint-intelligence-system">Complaint Intelligence System</a></h3>
      <ul>
        <li>Customer complaint triage with supervised NLP classifiers, served through FastAPI.</li>
        <li>Automated routing, sentiment breakdown and reporting.</li>
      </ul>
    </td>
  </tr>
</table>

---

## 🌐 Merged Upstream Contributions

<table>
  <thead>
    <tr>
      <th align="left">Project</th>
      <th align="left">PR</th>
      <th align="left">What it fixed</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="https://github.com/python/cpython">CPython</a></td>
      <td><a href="https://github.com/python/cpython/pull/158962">#158962</a></td>
      <td>asyncio: the threaded child watcher no longer blocks the event loop on macOS when a child process is stopped (<code>SIGSTOP</code>) rather than exited (<a href="https://github.com/python/cpython/issues/158287">gh-158287</a>).</td>
    </tr>
    <tr>
      <td><a href="https://github.com/pandas-dev/pandas">pandas</a></td>
      <td><a href="https://github.com/pandas-dev/pandas/pull/70838">#70838</a></td>
      <td>Python CSV engine: custom converters that return unhashable values (lists, dicts) no longer crash type inference (<a href="https://github.com/pandas-dev/pandas/issues/56848">#56848</a>).</td>
    </tr>
    <tr>
      <td><a href="https://github.com/tensorflow/tensorflow">TensorFlow</a></td>
      <td><a href="https://github.com/tensorflow/tensorflow/pull/129229">#129229</a></td>
      <td><code>tf.data</code>: <code>from_tensor_slices</code> / <code>from_tensors</code> convert host arrays on CPU instead of allocating GPU memory during dataset construction (<a href="https://github.com/tensorflow/tensorflow/issues/71744">#71744</a>).</td>
    </tr>
    <tr>
      <td><a href="https://github.com/ultralytics/ultralytics">Ultralytics</a></td>
      <td><a href="https://github.com/ultralytics/ultralytics/pull/26711">#26711</a></td>
      <td>Clear error instead of a TensorRT assertion when exporting INT8 engines with <code>nms=True</code> on JetPack 6 (<a href="https://github.com/ultralytics/ultralytics/issues/26655">#26655</a>).</td>
    </tr>
    <tr>
      <td><a href="https://github.com/docling-project/docling">Docling</a></td>
      <td><a href="https://github.com/docling-project/docling/pull/4240">#4240</a></td>
      <td>Safe fallback when Pydantic's <code>serialize_as_any</code> reports a false circular reference, which was crashing conversions (<a href="https://github.com/docling-project/docling/issues/4229">#4229</a>).</td>
    </tr>
    <tr>
      <td><a href="https://github.com/Significant-Gravitas/AutoGPT">AutoGPT</a></td>
      <td><a href="https://github.com/Significant-Gravitas/AutoGPT/pull/14875">#14875</a></td>
      <td>Copilot <code>web_fetch</code>: keeps main page content instead of truncating raw HTML early, moves HTML cleaning off the event loop, and warns on JS-only page shells (<a href="https://github.com/Significant-Gravitas/AutoGPT/issues/14828">#14828</a>).</td>
    </tr>
    <tr>
      <td><a href="https://github.com/headroomlabs-ai/headroom">Headroom</a></td>
      <td><a href="https://github.com/headroomlabs-ai/headroom/pull/3579">#3579</a></td>
      <td>Proxy budget limits now enforced on OpenAI and Gemini routes and on WebSocket frames (<a href="https://github.com/headroomlabs-ai/headroom/issues/3374">#3374</a>).</td>
    </tr>
    <tr>
      <td><a href="https://github.com/NVIDIA/SkillSpector">SkillSpector (NVIDIA)</a></td>
      <td><a href="https://github.com/NVIDIA/SkillSpector/pull/903">#903</a></td>
      <td>Stops flagging HTTP <code>DELETE</code> verbs in REST route tables as destructive filesystem deletes (<a href="https://github.com/NVIDIA/SkillSpector/issues/832">#832</a>).</td>
    </tr>
    <tr>
      <td><a href="https://github.com/semantica-agi/semantica">Semantica</a></td>
      <td><a href="https://github.com/semantica-agi/semantica/pull/1603">#1603</a></td>
      <td>Nested metadata filtering in the MCP <code>handle_query_decisions</code> handler (<a href="https://github.com/semantica-agi/semantica/issues/1247">#1247</a>).</td>
    </tr>
    <tr>
      <td><a href="https://github.com/Dpro-at/Tel-Agent">Tel-Agent</a></td>
      <td><a href="https://github.com/Dpro-at/Tel-Agent/pull/243">#243</a>, <a href="https://github.com/Dpro-at/Tel-Agent/pull/244">#244</a>, <a href="https://github.com/Dpro-at/Tel-Agent/pull/248">#248</a>, <a href="https://github.com/Dpro-at/Tel-Agent/pull/252">#252</a></td>
      <td>Mattermost channel transport, gateway auth fix, mention cleanup and locale updates.</td>
    </tr>
  </tbody>
</table>

<sub>All merged PRs: <a href="https://github.com/pulls?q=is%3Apr+author%3AJohnnyWilson16+is%3Amerged">github.com/pulls?q=author:JohnnyWilson16+is:merged</a></sub>

---

## 📬 Contact

- **Email**: [johnnydougherty09@gmail.com](mailto:johnnydougherty09@gmail.com)
- **LinkedIn**: [linkedin.com/in/johnny-wilson-dougherty-81693b292](https://www.linkedin.com/in/johnny-wilson-dougherty-81693b292)
- **Location**: Vijayawada, Andhra Pradesh, India (open to remote or onsite)
