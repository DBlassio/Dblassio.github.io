<!-- Agrega este bloque al inicio para los estilos -->
<style>
body {
  font-family: 'Inter', sans-serif;
  background: #f9f9f9;
  color: #111;
  line-height: 1.6;
  padding: 1rem;
}

h1.page-title {
  text-align: center;
  font-weight: 600;
  margin: 2rem 0;
}

.project-card {
  background: #fff;
  padding: 1.5rem;
  margin: 1.5rem auto;
  max-width: 800px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.05);
}

.project-header {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
}

.project-header h2 {
  font-size: 1.3rem;
  font-weight: 600;
  margin: 0;
}

.project-date {
  font-size: 0.95rem;
  color: #666;
}

.project-institution {
  font-weight: 500;
  margin-top: 0.2rem;
}

.project-supervisor {
  font-size: 0.95rem;
  color: #555;
  margin-top: 0.2rem;
}

.project-description {
  margin-top: 0.5rem;
  text-align: justify;
}

.project-skills {
  font-size: 0.9rem;
  margin-top: 0.5rem;
}

.project-skills a {
  color: #0070f3;
  text-decoration: none;
}

.project-skills a:hover {
  text-decoration: underline;
}
</style>

<!-- Página de Proyectos -->
<h1 class="page-title">Applied Projects</h1>

<!-- Proyecto 1 -->
<div class="project-card">
  <div class="project-header">
    <h2>Multimodal Argument Mining for Stance Detection</h2>
    <span class="project-date">Feb 2026 (On-going)</span>
  </div>
  <div class="project-institution">INRIA, CNRS, i3S - France</div>
  <div class="project-supervisor">
    Supervisor: Dr. Serena Villata | Team: MARIANNE – Computational Argumentation in Natural Language
  </div>
  <p class="project-description">
    Researching how linguistic and visual information jointly shape persuasive communication. Building multimodal models that integrate text + images for stance classification. Implementing transformer models (LLMs/VLMs), with computer vision techniques and early/intermediate/late fusion, to analyze how images modify argumentative intent and stance polarity (Abortion / Gun Control).
  </p>
  <div class="project-skills">
    <strong>Skills & Tools:</strong> Python, PyTorch, Hugging Face Transformers, LLM fine-tunning, multimodal embeddings, F1-Score Optimization<br/>
    <strong>Repo / Docs:</strong> <a href="https://github.com/DBlassio/multimodal-argmining">GitHub</a>
  </div>
</div>

<!-- Proyecto 2 -->
<div class="project-card">
  <div class="project-header">
    <h2>Dynamical Structure-Function Correlations of fMRI Human Brain Signals under LSD</h2>
    <span class="project-date">Aug 2025</span>
  </div>
  <div class="project-institution">INRIA - France</div>
  <div class="project-supervisor">
    Supervisor: Dr. Rodrigo Cofré | Team: CRONOS - Computational Neuroscience & Brain Dynamics
  </div>
  <p class="project-description">
    Research on how LSD alters dynamic brain functional states using phase-based fMRI connectivity. Applied unsupervised learning with k-means clustering on phase coherence vectors to identify canonical brain states, capturing recurrent dynamic patterns. Designed modular Python pipelines for reproducible analysis and intuitive visualization of altered conscious states.
  </p>
  <div class="project-skills">
    <strong>Skills & Tools:</strong> Python, scipy, scikit-learn, seaborn, time series analysis, EEG/fMRI signal processing, Hilbert transform, K-means clustering, statistical tests.<br/>
    <strong>Repo / Docs:</strong> <a href="https://github.com/DBlassio/phase_coherance_consciousness">GitHub</a>
  </div>
</div>
