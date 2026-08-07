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

.project-publication {
  font-size: 0.9rem;
  color: #0070f3;
  margin-top: 0.5rem;
  margin-bottom: 0.5rem;
}

</style>
<!-- Página de Proyectos -->
<h1 class="page-title">Applied Projects</h1>

<!-- Proyecto 1 -->
<div class="project-card">
  <div class="project-header">
    <h2>Multimodal Argument Mining for Stance Detection</h2>
  </div>
  <div class="project-institution">INRIA, CNRS, i3S — France</div>
  <div class="project-supervisor">Supervisor: HDR. Serena Villata | MARIANNE Team</div>
  <p class="project-description">
      Does an image change what a tweet is arguing, or just decorate 
      it? I built and benchmarked text-only, vision-only, and multimodal 
      architectures — DeBERTa-v3 paired with CLIP, BLIP, and ALIGN — 
      across five fusion strategies, from simple concatenation to gated 
      fusion, on the ImageArg dataset (tweets on gun control and 
      abortion). Text alone gets you far: F1 = 0.933. But a CLIP 
      vision-only model, with no text at all, still reaches F1 = 0.725 — 
      enough to show images aren't just decoration, they carry real 
      argumentative weight on their own.
  </p>
  <p class="project-publication">
    📄 Published at <strong>COMMA 2026</strong> — <em>"Multimodal Stance 
    Detection in Controversial Tweets"</em>
  </p>
  <div class="project-skills">
    <strong>Skills & Tools:</strong> Python, PyTorch, DeBERTa-v3, CLIP/BLIP/ALIGN, 
    PEFT, data augmentation, hyperparameter optimization, OCR<br/>
    <strong>Repo:</strong> <a href="https://github.com/DBlassio/multimodal-argmining">GitHub</a>
  </div>
</div>

<!-- Proyecto 2 -->
<div class="project-card">
  <div class="project-header">
    <h2>Gated Multimodal Fusion for Sexism Detection in Memes</h2>
  </div>
  <div class="project-institution">PRHLT Research Center, UPV — Spain</div>
  <p class="project-description">
    Sexism in memes doesn't just live in the text or the image, so I 
    built a system that also reads how people's brains and eyes respond 
    to them. This project fuses text, image, EEG, and eye-tracking 
    signals through a gated fusion mechanism that learns, per meme, how 
    much to trust each modality, the weights are the explanation. The gates converged 
    on a clear, reproducible hierarchy: image dominates (β ≈ 0.98), EEG adds real 
    complementary signal (α ≈ 0.48), eye-tracking gets mostly ignored once EEG is present (λ ≈ 0.03).
  </p>
  <p class="project-publication">
    📄 Published at <strong>CLEF 2026</strong> — <em>"Gated 
    Multimodal Fusion with Neurophysiological Signals for Sexism 
    Detection in Memes"</em> — sole author
  </p>
  <div class="project-skills">
    <strong>Skills & Tools:</strong> Python, PyTorch, mDeBERTa-v3, ALIGN, 
    gated fusion, cross-attention, EEG signal processing, multi-task learning<br/>
    <strong>Repo:</strong> <a href="https://github.com/DBlassio/multimodal-exist">GitHub</a>
  </div>
</div>

<!-- Proyecto 3 -->
<div class="project-card">
  <div class="project-header">
    <h2>EEG Spatial Gates (Topographic Transformer) </h2>
  </div>
  <div class="project-institution">PRHLT Research Center, UPV — Spain</div>
  <div class="project-supervisor">Supervisors: Prof. Paolo Rosso, Dr. Marco Siino</div>
  <p class="project-description">
    A direct extension of my CLEF 2026 work: what if EEG isn't just 80 
    flat numbers, but a brain with actual geography? I built a 
    spatial EEG Transformer that treats each of the 16 electrodes as a 
    token with topographic positional embeddings, testing whether 
    preserving that spatial structure, and gating per channel instead 
    of per modality, reveals which brain regions actually respond to 
    sexist content. Four architectures, increasing complexity, same 
    question throughout: does the brain's geometry matter, or is a flat 
    vector just as good?
  </p>
  <div class="project-skills">
    <strong>Skills & Tools:</strong> Python, PyTorch, Transformers, 
    topographic positional embeddings, EEG spatial modeling, interpretability<br/>
    <strong>Repo:</strong> <a href="https://github.com/DBlassio/multimodal-eeg-spatial-gates">GitHub</a>
  </div>
</div>

<!-- Proyecto 4 -->
<div class="project-card">
  <div class="project-header">
    <h2>RAG arXiv Research Assistant <span style="font-size:0.75rem;font-weight:500;color:#0070f3;">(Ongoing)</span></h2>
  </div>
  <div class="project-institution"></div>
  <p class="project-description">
      Here is an AI research assistant that answers questions over a corpus of 
      arXiv papers, grounded strictly in what's actually in the papers, 
      nothing else. I care about knowing what a model actually relies 
      on, not assuming it works, so every layer here is verifiable: 
      tokenizer-aware chunking, cosine-matched indexing, and generation
      that refuses to answer when the retrieved evidence doesn't support it. 
      Tested it explicitly: it declines off-topic questions with no hallucinated
      fallback, and grounds its answers in exact figures when the evidence is strong. 
      RAGAS evaluation and API deployment.
  </p>
  <div class="project-skills">
    <strong>Skills & Tools:</strong> Python, LangChain, BGE embeddings, 
    ChromaDB, Claude API, RAGAS, tokenizer-aware chunking<br/>
    <strong>Repo:</strong> <a href="https://github.com/DBlassio/rag-arxiv-fds">GitHub</a>
  </div>
</div>