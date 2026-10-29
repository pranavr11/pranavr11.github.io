---
layout: page
title: Projects
permalink: /projects/
---

- **[HFold](/assets/papers/hfold.pdf)** (15-442 final project)

  Full self-attention provides strong long-context reasoning but scales quadratically with sequence length, making long-context inference expensive. We introduce HFold, an inference-time heap-folding mechanism that augments sliding-window attention with a bounded cache of high-relevance hidden states. HFold retrieves selected historical states during inference and folds evicted states back into the heap using learned summary and relevance models. We evaluate HFold against full attention and sliding-window attention on Pythia 14M and 31M using WikiText and SCROLLS. Our results suggest that HFold can recover global token relationships lost by sliding-window attention more effectively, but the current prototype is not hardware optimized and has substantial throughput overhead.
- **[EGDW](/assets/papers/egdw.pdf)** (11-785 final project)

  Over the past 5 years, advancements in deep learning have been centered around transformer-based models, most notably Large Language Models. They achieve strong performance across the board but rely on self-attention, a mechanism that incurs an expensive quadratic cost in sequence length. Recent recurrent architectures, such as Mamba, offer linear inference time through compressed representations of historical data. However, these approaches see degraded performance on long-context tasks due to their inherent representation limits. Google's TITANS architecture aims to address this by mimicking the human memory system: short-term memory via standard attention, long-term memory via a novel neural memory module, and fixed memory via a set of persistent weights. The neural memory module is updated using a "surprise"-based rule, heavily dependent on gradient magnitude and thus susceptible to catastrophic memory updates when outlier gradients are encountered. We propose Expected Gradient Divergence Weighting (EGDW), a probabilistic update method for the neural memory module. EGDW models gradients as instances of a random variable and down-weighs gradients that are unlikely under the current gradient distribution, using local and global surprise terms derived from fundamental probabilistic bounds. On a 10B-token subset of FineWebEdu, EGDW-TITANS achieves lower validation cross-entropy than the original TITANS baseline with higher train loss, indicating greater generalization. This outlines the potential for novel probabilistic-divergence-based gradient descent algorithms to stabilize memory updates and improve long-context abilities in language models and neural networks at large.
- **[PushT](/assets/papers/pusht.pdf)** (10-701 final project)

  Generalist imitation learning methods have shown strong performance in robotic manipulation from human demonstrations. A recent direction in this area is action chunking, where a policy predicts a sequence of future actions instead of a single step, enabling improved planning over long horizons. In this work, we adopt the Action Chunking with Transformers (ACT) architecture. We also consider human intervention methods such as DAgger, which mitigate compounding errors in behavioral cloning by aggregating expert corrections during policy rollouts. This project studies the long-horizon Push-T task, where an agent must push a T into a goal zone. While diffusion and flow matching methods achieve high success rates, the effectiveness of action chunking and its interaction with DAgger-style human intervention remain underexplored; we evaluate how ACT performs in this setting and its impact on success rate.

<br>

Current projects
- **Ultimate tic-tac-toe**, building on [minimax.dev](https://minimax.dev/docs/ultimate/)
- **Clash Royale RL bot**
- **Self-driving bike**

  Current state

  <div class="bike-photos">
    <a href="/assets/bike/frame.jpg"><img src="/assets/bike/frame.jpg" alt="Disassembled bike frame on a stand, with wheels and tires on the floor"></a>
    <a href="/assets/bike/parts.png"><img src="/assets/bike/parts.png" alt="Orange bag of wires, a multimeter, and small electronics"></a>
    <a href="/assets/bike/controller.jpg"><img src="/assets/bike/controller.jpg" alt="Motor controller, wiring harness, and a circuit board on a table"></a>
  </div>

<style>
.bike-photos {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 12px;
  margin: 0.75rem 0 0.25rem;
}
.bike-photos img {
  width: 100%;
  aspect-ratio: 1;
  object-fit: cover;
  display: block;
}
@media (max-width: 700px) {
  .bike-photos {
    grid-template-columns: 1fr;
  }
  .bike-photos img {
    aspect-ratio: auto;
    object-fit: contain;
  }
}
</style>
