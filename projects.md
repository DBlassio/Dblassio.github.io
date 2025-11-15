<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Applied Projects</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Inter', sans-serif;
      background: #f9f9f9;
      color: #111;
      margin: 0;
      padding: 0;
      line-height: 1.6;
    }

    h1 {
      text-align: center;
      font-weight: 600;
      margin: 2rem 0;
      font-size: 2rem;
    }

    .projects-container {
      max-width: 900px;
      margin: 0 auto;
      padding: 0 1rem;
    }

    .project-card {
      background: #fff;
      padding: 1.5rem 2rem;
      margin: 1.5rem 0;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.05);
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .project-card:hover {
      transform: translateY(-3px);
      box-shadow: 0 6px 16px rgba(0,0,0,0.08);
    }

    .project-header {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      flex-wrap: wrap;
      gap: 0.5rem;
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
      font-size: 1rem;
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
</head>
<body>

  <h1>Applied Projects</h1>

  <div class="projects-container">

    <!-- Proyecto 1 -->
    <div class="project-card">
      <div class="project-header">
        <h2>Multimodal Argument Mining for Stance Detection</h2>
        <span class="project-date">Feb 2026 (On-going)</span>
      </div>
      <div class="project-institution">INRIA, CNRS, i3S - MARIANNE Team, France</div>
      <div class="project-supervisor">
        Supervisor: Dr. Serena Villata | Team: MARIANNE – Computational argumentation in natural language
      </div>
      <p class="project-description">
        Researching how linguistic and visual information jointly shape persuasive communication. Building multimodal models that integrate text + images for stance classification. Implementing transformer models (LLMs/VLMs), with computer vision techniques and early/intermediate/late fusion, to analyze how images modify argumentative intent and stance polarity (Abortion / Gun Control).
      </p>
      <div class="project-skills">
        <strong>Skills & Tools:</strong> Python, PyTorch, Hugging Face Transformers, LLM fine-tunning, multimodal embeddings, F1-Score Optimization<br/>
        <strong>Repo / Docs:</strong> <a href="https://github.com/DBlassio/multimodal-argmining" target="_blank">GitHub</a>
      </div>
    </div>

    <!-- Proyecto 2 -->
    <div class="project-card">
      <div class="project-header">
        <h2>Dynamical Structure-Function Correlations of fMRI Human Brain Signals under LSD</h2>
        <span class="project-date">Aug 2025</span>
      </div>
      <div class="project-institution">INRIA - CRONOS Team, France</div>
      <div class="project-supervisor">
        Supervisor: Dr. Rodrigo Cofré | Team: CRONOS - computational neuroscience & brain dynamics
      </div>
      <p class="project-description">
        Studied the effect of LSD on dynamic brain functional states using phase-based fMRI connectivity, clustering, and statistical analysis. Computed fractional occupancy, state transitions, Markov chain entropy, and structure-function correlations.
      </p>
      <div class="project-skills">
        <strong>Skills & Tools:</strong> Python (numpy, scipy, pandas, scikit-learn, matplotlib, seaborn), EEG/fMRI signal processing, Hilbert transform, K-means clustering, statistical tests, Git/GitHub, LaTeX<br/>
        <strong>Repo / Docs:</strong> <a href="https://github.com/DBlassio/phase_coherance_consciousness" target="_blank">GitHub</a>
      </div>
    </div>

  </div>

</body>
</html>
