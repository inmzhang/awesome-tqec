# Awesome TQEC

A curated list of awesome topological quantum error correction resources.

## Table of Contents

- [Papers](#papers)
- [Software](#software)
- [Tutorials and Talks](#tutorials-and-talks)
- [Links](#links)

## Papers

#### History

Selected chronological references for the development of topological quantum
error correction.

- [Quantum codes on a lattice with boundary](https://arxiv.org/abs/quant-ph/9811052) - The toric code, memory only.
- [Topological quantum memory](https://arxiv.org/abs/quant-ph/0110143) - Computation using a stack of tori with transversal interactions.
- [A fault-tolerant one-way quantum computer](https://arxiv.org/abs/quant-ph/0510135) - Computation using a 3D cluster state with only local interactions in 3D.
- [Fault-tolerant quantum computation with high threshold in two dimensions](https://arxiv.org/abs/quant-ph/0610082) and [Topological fault-tolerance in cluster state quantum computation](https://arxiv.org/abs/quant-ph/0703143) - Build the 3D cluster state layer by layer so only a bi-layer of locally connected 2D hardware is required.
- [High threshold universal quantum computation on the surface code](https://arxiv.org/abs/0803.0272) - A version of the 2D scheme reduced to a single nearest-neighbor-coupled 2D layer of hardware; at this point everything was based on braiding holes (defects) in the surface.
- [Topological cluster state quantum computing](https://arxiv.org/abs/0805.3202) - A simplified version of the 3D cluster state scheme.
- [Quantum computing with nearest neighbor interactions and error rates over 1%](https://arxiv.org/abs/1009.3686) and [Towards practical classical processing for the surface code](https://arxiv.org/abs/1110.5133) - Beginning to learn how to decode the surface code better.
- [Surface code quantum computing by lattice surgery](https://arxiv.org/abs/1111.4022) - Original proposal for lattice surgery on an unrotated surface code.
- [Proof of finite surface code threshold for matching](https://arxiv.org/abs/1206.0800) - Proof that high levels of error can be suppressed exponentially using the surface code.
- [Surface codes: Towards practical large-scale quantum computation](https://arxiv.org/abs/1208.0928) - Comprehensive review of defect-based surface code quantum computation.
- [A bridge to lower overhead quantum computation](https://arxiv.org/abs/1209.0510) - Compressing defect-based TQEC.
- [Time-optimal quantum computation](https://arxiv.org/abs/1210.4626) - Shows that TQEC-based computation is not inherently slow given sufficient qubits.
- [Minimum weight perfect matching of fault-tolerant topological quantum error correction in average O(1) parallel time](https://arxiv.org/abs/1307.1740) - Scalable parallel decoding.
- [Optimal complexity correction of correlated errors in the surface code](https://arxiv.org/abs/1310.0863) - Using information about correlated errors to decode better.
- [Logic gates at the surface code threshold: Superconducting qubits poised for fault-tolerant quantum computing](https://arxiv.org/abs/1402.4848) - Early experimental work at the surface code threshold error rate.
- [Low overhead quantum computation using lattice surgery](https://arxiv.org/abs/1808.06709), [Efficient magic state factories with a catalyzed |CCZ&gt; to 2|T&gt; transformation](https://arxiv.org/abs/1812.01238), and [Flexible layout of surface code computations using AutoCCZ states](https://arxiv.org/abs/1905.08916) - Lattice surgery using the rotated surface code.
- [Suppressing quantum errors by scaling a surface code logical qubit](https://arxiv.org/abs/2207.06431) and [Quantum error correction below the surface code threshold](https://arxiv.org/abs/2408.13687) - Experimental demonstration of a below-threshold surface code, from the initial milestone to the current state of the art.
- [Surface code off-the-hook: diagonal syndrome-extraction scheduling](https://arxiv.org/abs/2602.09099) - Latest circuits for the surface code.

#### Simulator

- [Stim: a fast stabilizer circuit simulator](https://arxiv.org/abs/2103.02202)
- [SOFT: a high-performance simulator for universal fault-tolerant quantum circuits](https://arxiv.org/abs/2512.23037)
- [Tsim: Fast Universal Simulator for Quantum Error Correction](https://arxiv.org/abs/2604.01059)

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

##### Tensor Network(TN)

- [Efficient algorithms for maximum likelihood decoding in the surface code](10.1103/PhysRevA.90.032326) - MLD for surface code under code-capacity noise.
- [Tensor Network Decoding Beyond 2D](http://arxiv.org/abs/2310.10722) - MLD for surface code under circuit-level noise.

##### Neural Network(NN)

- [Learning to Decode the Surface Code with a Recurrent, Transformer-Based Neural Network](http://arxiv.org/abs/2310.05900)

##### Parallel Window

- [Scalable surface code decoders with parallelization in time](http://arxiv.org/abs/2209.09219)
- [Modular decoding: parallelizable real-time decoding for quantum computers](http://arxiv.org/abs/2303.04846)
- [Parallel window decoding enables scalable fault tolerant quantum computation](http://arxiv.org/abs/2209.08552)

##### Belief Propagation

- [Improved decoding of circuit noise and fragile boundaries of tailored surface codes](https://arxiv.org/abs/2203.04948) - Two-stage decoding combining
belief propagation and MWPM/UF.

#### Experiment

- [Suppressing quantum errors by scaling a surface code logical qubit](https://www.nature.com/articles/s41586-022-05434-1) - Suppression of logical
error when scaling surface code from distance 3 to 5.


## Software

#### Simulator

- [Stim](https://github.com/quantumlib/Stim) - A fast stabilizer circuit library.

- [Crumble](https://algassert.com/crumble) - Point-and-Click 2D QEC circuit builder.

- [SOFT](https://github.com/haoliri0/SOFT) - A high-performance simulator for universal fault-tolerant quantum circuits.

- [tsim](https://github.com/QuEraComputing/tsim) - A GPU-accelerated quantum circuit sampler for QEC with support for non-Clifford gates.

#### Automation tool

- [tqec](https://github.com/tqec/tqec) - State-of-the-art quantum compilation for the surface code.

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

#### Evidence auditing and verification

- [QEC Evidence Auditor — Standard Mathematical V1](https://github.com/cxclrfx/QEC-Evidence-Auditor) - Technical showcase of proprietary offline Auditor and Verifier programs for mathematical QEC artifacts, with five validation modes.

## Tutorials and Talks

- [TQEC Group Meetings](https://docs.google.com/spreadsheets/d/11DSA2wzKLOrfTGNHunFvzsMYeO7jZ8Ny8kpzoC_wKQg/edit?resourcekey=0-PdGFkp5s-4XWihMSxk0UIg#gid=0) - Insightful
introductory recordings and resources by Austin Fowler and other TQEC group members.
- [A Rosetta Stone for the ZX Calculus and the Surface Code](https://www.youtube.com/watch?v=1ojXEEm_JiI) - Explain the connection between ZX Calculus
and surface code computation by Craig Gidney.
- [3D topological diagram explanation](https://docs.google.com/presentation/d/1IjZ-0W9Y22wNG5036WFnnkF5Az1Zt8jTHFTC1-e7Em4/edit?usp=sharing) - Unfinished
slides of Craig Gidney to explain how to read topological diagram from [this post](https://quantumcomputing.stackexchange.com/questions/5280/reference-that-explains-how-to-read-3d-topological-diagrams-for-surface-code-com).
- [QEC23](https://www.youtube.com/@QEC23) - Recording of 6th International Conference on Quantum Error Correction, some talks are about TQEC.

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
