<h1 align="center" style="margin-top: 0px;">⚡ANSR:<br>Flash Amortized Neural Symbolic Regression</h1>

<div align="center">

[Project Page](https://github.com/psaegert/flash-ansr)

</div>

<img src="https://github.com/psaegert/flash-ansr/blob/main/assets/images/nsr-training.drawio.svg" width="100%">

> **⚡ANSR Training on Fully Procedurally Generated Data** Inspired by NeSymReS ([Biggio et al. 2021](https://arxiv.org/abs/2106.06427))



# Abstract
Symbolic Regression has been approached with many different methods and paradigms. The overwhelming success of transformer-based language models in recent years has since motivated researchers to solve Symbolic Regression with large-scale pre-training of data-conditioned "equation generators" at competitive levels. However, as most traditional methods, the majority of these Amortized Neural Symbolic Regression methods rely on SymPy to simplify and compile randomly generated training equations, a choice that inevitably brings tradeoffs and requires workarounds to efficiently work at scale. I show that replacing SymPy with a novel token-based simplification algorithm with hand-crafted transformation rules enables training on _fully-procedurally_ generated and _higher-quality_ synthetic data, and thus develop ⚡ANSR. On various test sets, my method perfectly recovers $+80$% more equations numerically than the NeSymReS baseline while being 84 times faster natively, and yields comparable recovery rates to PySR in a quarter of its time. I provide an in-depth performance analysis of my method on stricter and more meaningful metrics than previous work. ⚡ANSR is open-source and available on GitHub and Huggingface, and allows for straight-forward replicability on consumer-grade hardware.

# Citation
```bibtex
@software{flash-ansr2024,
    author = {Paul Saegert},
    title = {Flash Amortized Neural Symbolic Regression},
    year = 2024,
    publisher = {GitHub},
    version = {0.3.0},
    url = {https://github.com/psaegert/flash-ansr}
}
```
