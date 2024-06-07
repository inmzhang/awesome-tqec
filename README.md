# Awesome TQEC

A curated list of awesome topological quantum error correction resources.

## Table of Contents

- [Papers](#papers)
- [Software](#software)
- [Tutorials and Talks](#tutorials-and-talks)
- [Links](#links)

## Papers

#### Simulator

- [Stim: a fast stabilizer circuit simulator](https://arxiv.org/abs/2103.02202)

#### Lattice Surgery

- [Surface code quantum computing by lattice surgery](https://iopscience.iop.org/article/10.1088/1367-2630/14/12/123011)
- [Low overhead quantum computation using lattice surgery](http://arxiv.org/abs/1808.06709)
- [A Game of Surface Codes: Large-Scale Quantum Computing with Lattice Surgery](https://quantum-journal.org/papers/q-2019-03-05-128/)
- [Flexible layout of surface code computations using AutoCCZ states](https://arxiv.org/abs/1905.08916)
- [Inplace Access to the Surface Code Y Basis](https://arxiv.org/abs/2302.07395) - Optimization of logical Y-basis measurement and logical S gate.
- [Cleaner magic states with hook injection](https://arxiv.org/abs/2302.12292) - Optimization of magic state injection.
- [Yoked surface codes](https://arxiv.org/abs/2312.04522) - Reduce the overhead by concatenating surface code into parity check codes.
- [A SAT Scalpel for Lattice Surgery: Representation and Synthesis of Subroutines for Surface-Code Fault-Tolerant Quantum Computing](http://arxiv.org/abs/2404.18369) - 
Synthesizer for lattice surgery subroutines.

#### Cluster State

Understand the TQEC structure from the view of cluster state.

- [Measurement-based quantum computation with cluster states](https://arxiv.org/abs/quant-ph/0301052)
- [Topological cluster state quantum computing](https://arxiv.org/abs/0805.3202)
computation.

#### ZX-Calculus

Understand the TQEC structure from the view of zx-calculus.

- [Unifying flavors of fault tolerance with the ZX calculus](http://arxiv.org/abs/2303.08829)
- [The ZX calculus is a language for surface code lattice surgery](http://arxiv.org/abs/1704.08670)

#### Time-dynamic Circuits

Using time-dynamic circuit without changing the underlying quantum code to achieve better performance/overhead or else.

- [Relaxing Hardware Requirements for Surface Code Circuits using Time-dynamics](https://arxiv.org/abs/2302.02192)
- [New circuits and an open source decoder for the color code](https://arxiv.org/abs/2312.08813)

#### Decoder

##### Minimum-weight Perfect Matching(MWPM)

- [Towards practical classical processing for the surface code: Timing analysis](https://link.aps.org/doi/10.1103/PhysRevA.86.042313)
- [Sparse Blossom: correcting a million errors per core second with minimum-weight matching](http://arxiv.org/abs/2303.15933) - Speedup MWPW by
sparse blossom algorithm on decoding graph.
- [Fusion Blossom: Fast MWPM Decoders for QEC](http://arxiv.org/abs/2305.08307) - Similar idea to Sparse Blossom, speedup MWPM by fusion blossom on
decoding graph.
- [Optimal complexity correction of correlated errors in the surface code](http://arxiv.org/abs/1310.0863) - Enhance MWPM by recursive correlated
matching.
- [Pipelined correlated minimum weight perfect matching of the surface code](http://arxiv.org/abs/2205.09828) - Correlated matching with pipelined
method.

##### Union-find(UF)

- [Almost-linear time decoding algorithm for topological codes](https://arxiv.org/abs/1709.06218)
- [Fault-tolerant weighted union-find decoding on the toric code](https://link.aps.org/doi/10.1103/PhysRevA.102.012419) - Weighted union-find decoder.

##### Neural Network(NN)

- [Learning to Decode the Surface Code with a Recurrent, Transformer-Based Neural Network](http://arxiv.org/abs/2310.05900)

##### Parallel Window

- [Scalable surface code decoders with parallelization in time](http://arxiv.org/abs/2209.09219)
- [Modular decoding: parallelizable real-time decoding for quantum computers](http://arxiv.org/abs/2303.04846)
- [Parallel window decoding enables scalable fault tolerant quantum computation](http://arxiv.org/abs/2209.08552)

##### Belief Propagation

- [Improved decoding of circuit noise and fragile boundaries of tailored surface codes](https://arxiv.org/abs/2203.04948) - Two-stage decoding combining
belief propagation and MWPM/UF.


## Software

#### Simulator

- [Stim](https://github.com/quantumlib/Stim) - A fast stabilizer circuit library.

- [Crumble](https://algassert.com/crumble) - Point-and-Click 2D QEC circuit builder.

#### Automation tool

- [tqec](https://github.com/QCHackers/tqec) - Design automation tool for tqec.

- [LaSsynth](https://zenodo.org/records/11210072) - A synthesizer for lattice surgery subroutines.

- [Lattice Surgery Compiler](https://github.com/latticesurgery-com/lattice-surgery-compiler) - Compile logical quantum circuits to lattice surgery
operations on a surface code lattice.

#### Decoder

- [PyMatching](https://github.com/oscarhiggott/PyMatching) - A fast MWPM decoder for quantum error correction code, implemented in C++.

- [Fusion Blossom](https://github.com/yuewuo/fusion-blossom) - Another fast MWPM decoder for quantum error correction code, implemented in Rust.

- [Belief Matching](https://github.com/oscarhiggott/BeliefMatching) - An implementation of belief-matching decoder.

- [Chromobius](https://github.com/quantumlib/chromobius) - An implementation of a "mobius decoder" for color code.

- [ldpc](https://github.com/quantumgizmos/ldpc) - Belief propagation(BP) implementation, also include implementations for union-find, belief-find and more
decoders(in the branch "release-v2").

## Tutorials and Talks

- [TQEC Group Meetings](https://docs.google.com/spreadsheets/d/11DSA2wzKLOrfTGNHunFvzsMYeO7jZ8Ny8kpzoC_wKQg/edit?resourcekey=0-PdGFkp5s-4XWihMSxk0UIg#gid=0) - Insightful
introductory recordings and resources by Austin Fowler and other TQEC group members.
- [A Rosetta Stone for the ZX Calculus and the Surface Code](https://www.youtube.com/watch?v=1ojXEEm_JiI) - Explain the connection between ZX Calculus
and surface code computation by Craig Gidney.
- [3D topological diagram explanation](https://docs.google.com/presentation/d/1IjZ-0W9Y22wNG5036WFnnkF5Az1Zt8jTHFTC1-e7Em4/edit?usp=sharing) - Unfinished
slides of Craig Gidney to explain how to read topological diagram from [this post](https://quantumcomputing.stackexchange.com/questions/5280/reference-that-explains-how-to-read-3d-topological-diagrams-for-surface-code-com).

## Links

- [TQEC Google group](https://groups.google.com/g/tqec-design-automation) - A community for learning about TQEC and
building the design automation tools.
- [Error Correction Zoo](https://errorcorrectionzoo.org/) - Collection of classical and quantum error correction codes, including the
topological quantum error correction codes.
- [Quantum Computing Stack Exchange](https://quantumcomputing.stackexchange.com/) - Question-and-answer site dedicated to quantum computing, where
plenty of TQEC related questions are involved.
- [SketchUp](https://www.sketchup.com/app) - Useful tool to make the space-time diagram for topological logical computation.
- [Algorithmic Assertions](https://algassert.com/) - Craig Gidney's blogs about computer science and quantum computing, where the topic
of TQEC is involved.

