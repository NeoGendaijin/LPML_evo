# LPML_evo

Use LPML like format for strategy evolution

## Research Project: Evolution of Strategies and Norms Using Natural Language Tags

### Overview

This project explores the evolution of strategies and norms among agents using a tag-based format in natural language. The core idea is to enable agents to dynamically generate new strategies through dialogue, using tags like `<walk>` and `<negotiate>`.

### Core Ideas

- **Evolution of Strategies with Tags**: Agents can dynamically generate new strategies through dialogue using tags.
- **Extended Communication**: Analyze natural language and visualize strategic patterns using embeddings like UMAP.
- **Game Theoretical Approach**: Simulate the evolution of social norms and relationships using Axelrod's metanorm game.

### System Architecture

#### Strategy Description Format

Agents use XML-like tags to express their internal state, decision process, and action plans.

```xml
<strategy>
  <observe>
    Enemy spotted at (x=100, y=50) with low shield.
  </observe>
  <calculate>
    If I attack now, probability of success = 0.75; risk level moderate.
  </calculate>
  <decide>
    Proceed with attack, but maintain fallback plan.
  </decide>
</strategy>
```

#### Hierarchical and Dynamic Tag Generation

Agents generate nested tags based on the situation, simulating interactions like negotiation and resource sharing.

```xml
<interaction>
  <negotiation>
    <propose>
      Let's form an alliance for the next 3 turns.
    </propose>
    <counter_propose>
      How about sharing 50% of resources instead?
    </counter_propose>
  </negotiation>
</interaction>
```

### Implementation

- **Language Processing and Embeddings**: Use UMAP or t-SNE for embedding creation and strategy visualization.
- **Simulation Experiments**: Conduct simulations in multi-agent environments to observe strategy evolution.

### Future Work

- Optimize tag generation algorithms.
- Conduct real-world experiments to identify effective strategy patterns.
