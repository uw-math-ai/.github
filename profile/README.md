# Math AI Lab at UW

The Math-AI lab provides a space for mathematicians at any level (faculty, postdocs, PhD students, undergraduates, high school students, ...) to learn about formalizing mathematics with Lean, as well as learn about the intersection between Math and AI. 

We also have a research [seminar](https://math.washington.edu/events/series/math-ai-seminar).

<img width="50%" alt="math-ai-lab-group-photo" src="https://github.com/user-attachments/assets/bd3768e1-ef75-4da6-87ba-d311cb243baf" />


## Fall 2025 Math AI Lab Projects

We meet Mondays and Wednesdays from 4–5:30 pm in OUG 136.

---

### Project 1: AI for Quantum Code Compilation
- **Lead Mentor**: Andres Paz  
- **Students**: Eric Hur, Mayee Sun, Sylvie Lausier, Christian Tarta  
- **Description**: Quantum error correction (QEC) codes are traditionally described using stabilizers, which define the subspace preserved by the code. However, implementing these codes requires translating stabilizers into fault-tolerant quantum circuits—an inherently nontrivial task that depends on the constraints and capabilities of the underlying hardware architecture.  
  This project aims to develop an AI agent capable of synthesizing such circuits in a way that:  
  1. In the ideal (noiseless) setting, the resulting circuits implement the intended stabilizer structure of the code on the target architecture.  
  2. In the noisy setting, the agent searches over circuit variations to optimize fidelity, taking into account realistic noise models and architectural constraints.  
  The outcome would be a toolchain bridging the gap between abstract QEC code design and concrete, high-performance circuit implementations, enabling better exploration of architecture-specific tradeoffs in fault-tolerant quantum computing.  
- **Prerequisites**: Linear algebra (must have), ML experience (recommended)

---

### Project 2: Deep Learning of Number Theory
- **Lead Mentors**: Jarod Alper and Junaid Hasan  
- **Students**: Andrew Chen, Claire Xu, Ivonne Zhang, Akhil Srinivasan, Nina Tharamal, Hemkesh Bandi  
- **Description**: The goal is to explore to what extent modern machine learning algorithms (e.g., feedforward neural networks, transformers, LLMs) can learn number-theoretic functions such as modular arithmetic, the Möbius function, or gcd. We can first attempt to replicate results from the literature ([arXiv:2502.10335](https://arxiv.org/pdf/2502.10335), [arXiv:2308.15594](https://arxiv.org/abs/2308.15594)) and then explore our own functions and algorithms. We aim to submit to one of the major ML conferences such as ICML or ICLR.  
- **Prerequisites**: Python (must have), ML experience (desired)  
- **Code**: [GitHub repo](https://github.com/uw-math-ai/dl-nt)

---

### Project 3: Formalizing Geometric Measure Theory
- **Lead Mentor**: Ignacio Tejeda  
- **Students**: Annie Cao, Nathan Pao, Theodore Meek  
- **Description**: The goal is to formalize the following theorem in geometric analysis: if \(E\) is a set of Hausdorff dimension \(0 < s < 1\), the density \(D^s(E,x)\) fails to exist at almost every point \(x \in E\). This is Theorem 4.2 in Falconer’s *Geometry of Fractal Sets*. To get exposure with Lean and specifically with analysis in Lean, this project will begin by following Terence Tao’s *Lean Companion to Analysis I*.  
- **Prerequisites**: Lean (recommended), analysis (recommended)  
- **Code**: [GitHub repo](https://github.com/uw-math-ai/FormalizingGMT)

---

### Project 4: Formalizing Stacks
- **Lead Mentors**: Eric Klavins and Max Lieblich  
- **Additional Mentor**: Leopold Mayer  
- **Students**: Dowland Aiello, James Martin  
- **Description**: This project seeks to give formal definitions in Lean of the mathematical objects of sites, sheaves, and stacks. While these are sophisticated mathematical objects, their definitions are not hard to internalize axiomatically, assuming a basic understanding of category theory. Building off mathlib’s definition of a category, the first aim is to define a site following the Stacks Project Tag 00VG rather than using mathlib’s current definition. The focus here is on formalizing these key definitions, rather than building out a larger mathematical library with lemmas and theorems.  
- **Prerequisites**: Lean (recommended), category theory (recommended)  
- **Code**: [GitHub repo](https://github.com/uw-math-ai/formalizing-stacks)

---

### Project 5: How Good Are Language Models at Lean?
- **Lead Mentors**: Tyson Klingner and Patrick O’Melveny  
- **Students**: Kaira Nair, Drew Bladek, Xinyue Fu, Bohao Chen  
- **Description**: In an effort to understand the ability of frontier general-purpose large language models at generating Lean code, we will design an evaluation procedure for various Lean tasks such as next-step generation or entire proof generation. We will run our algorithms on existing frontier models to see which LLMs perform the best, providing valuable guidance to the Lean community on which models to use for certain use cases. The framework will be scalable so that the algorithms can be rerun when new model versions are released.  
- **Prerequisites**: ML experience (must have), Lean (recommended)  
- **Code**: [GitHub repo](https://github.com/uw-math-ai/LLMsLean)

---

### Project 6: Lean Error Correction with Language Models
- **Lead Mentor**: Vasily Ilin  
- **Students**: Ajit Mallavarapu, Evan Wang, Simon Chess, Daniel Lee, Siyuan Ge  
- **Description**: With the goal of making Lean easier to use and specifically making errors easier to debug, we will curate a Lean error dataset and train models to correct errors. There are currently large datasets of error-free code (e.g., mathlib and GitHub repositories), but no existing datasets of common human-made errors. This makes it hard to train LLMs to understand compiler feedback and fix the errors. We will assemble a dataset of erroneous proofs, compiler feedback, and error corrections, and fine-tune Qwen 4B on this dataset. We aim to submit to one of the major ML conferences such as ICML or ICLR.  
- **Prerequisites**: Python (must have), Lean (must have), an ML course (useful)  
- **Time Commitment**: At least 10 hours/week for a quarter  
- **Code**: [GitHub repo](https://github.com/uw-math-ai/lean-error-correction)

---

### Project 7: Mathematician’s Copilot — Reliable Theorem Search
- **Lead Mentors**: Vasily Ilin and Giovanni Inchiostro  
- **Students**: Sophie Szeto, Eric Leonen, Ted Guan, Artemii Remizov  
- **Description**: The broad vision is to apply modern machine learning techniques to facilitate mathematical research. As a first step, this project seeks to design search algorithms for locating theorem statements. Mathematics is unique in having precise, self-contained statements of knowledge, but no reliable tool yet exists to find them. Current frontier LLMs (e.g., ChatGPT) can approximate the right reference but often hallucinate the numbering. We will develop a search tool by scraping arXiv and other mathematical sources (e.g., the Stacks Project), extracting theorem statements, and computing embeddings of the text. At inference time, we will compare cosine similarities between user queries and stored theorems (similar to LeanSearch).  
- **Prerequisites**: Python (must have), ML course (useful)  
- **Time Commitment**: At least 5 hours/week for a quarter  

---

### Project 8: Monogenic Extensions of Regular Local Rings
- **Meeting Time**: Tuesdays 8:30–10:30 am  
- **Lead Mentors**: John Leo and Bianca Viray  
- **Additional Mentor**: Bryan Boehnke  
- **Students**: George Peykanu, Sathvik Kurapati, Tianshuo Wang, Xinyi Zhi  
- **Description**: The goal is to add to Lean two lemmas from a recent paper ([arXiv:2503.07846](https://arxiv.org/abs/2503.07846)). The first lemma states that an étale extension of regular local rings is monogenic (i.e., generated by a single element). The second lemma states that an extension of regular local rings that fails to be étale at a unique codimension 1 point is also monogenic.  
- **Prerequisites**: Lean (recommended), commutative algebra (recommended)  
- **Code**: [GitHub repo](https://github.com/uw-math-ai/monogenic-extensions)

---

### Project 9: Provable Computation in Lean
- **Lead Mentor**: Dhruv Bhatia  
- **Students**: Annis Wu, Ruslana Korolov, Zeyin Feng, Alan Chang  
- **Description**: While Lean has seen extensive use as a theorem-proving assistant, its capabilities as a computational programming language have been underutilized. The goal of this project is to begin filling that gap. Along the way, we will learn the basics of functional programming, monads, and Lean’s metaprogramming framework to implement algorithms that can both be run efficiently and be reasoned about. Our main goal is to implement basic algorithms with applications to linear algebra while also proving (in Lean) correctness of said algorithms.  
- **Prerequisites**: Lean (recommended), metaprogramming in Lean (recommended)  
- **Code**: [GitHub repo](https://github.com/uw-math-ai/provable_computation)

---

### Project 10: Reinforcement Learning for Polynomials
- **Lead Mentors**: Jarod Alper and Michael Zeng  
- **Students**: Bhaumik Mehta, Weikun (Kyle) Zhang, Rohan Pandey, Trey Adams, Naomi Morato, Evan Porter, Kaijie Jin  
- **Description**: We will use reinforcement learning to train computers to search for efficient arithmetic circuits computing specific polynomials. This is in some sense a simplified version of proof generation, where computers are trained to search for proofs of theorems, except that in this case the search space is smaller. This project may also shed light on questions in algebraic complexity theory, specifically the algebraic analogue of P vs NP. Inspired by the AlphaZero algorithm for two-player games, we will adapt it to a single-player game. The goal is to find efficient ways to compute a polynomial \(f(x_1, \dots, x_n)\) using an arithmetic circuit consisting of + and × gates together with scalar multiplication. The computer is rewarded when it finds efficient arithmetic circuits. We aim to submit to a major ML conference such as ICML or ICLR.  
- **Prerequisites**: Python (must have), ML experience (must have)  
- **Code**: [GitHub repo](https://github.com/uw-math-ai/PolyArithmeticCircuitsRL)

---

### Project 11: Teaching a Computer to Knot
- **Lead Mentors**: Allison Henrich (Seattle U) and Andrew Tawfeek  
- **Students**: Sean Kawano, Abel Mesfin, Nicole Ham, Solden Stoll  
- **Description**: Mosaic diagrams were developed in 2008 by Lomanoco and Kauffman to build quantum knot systems. Since then, their structure has been widely studied because of the convenient way they encode a knot in 3D space as a matrix. In 2014, Kuriya and Shehab showed that mosaics are a complete invariant for tame knots (i.e., real-world knots made from string).  
  In this project, we will use this matrix encoding to build and train an AI model to recognize knots through their mosaic representation. Since knots are fundamentally topological objects with connectivity patterns, we will construct an appropriate graph neural network and train it, developing milestones to gauge progress (e.g., recognizing connectedness, then number of links, etc.).  
- **Prerequisites**: Python experience (must have)


## Spring 2025 Math AI Lab Projects

### Formalization Projects

#### Project 1: Formalizing Polyhedral Geometry
- **Mentors**: Caelan Ritter and Freda Zheng, Mathematics  
- **Students**: Seven Lewis and George Peykanu  
- **Description**: In this project, the goal is to formalize the basic results in polyhedral geometry, up to the equivalence of definitions of a polyhedron in terms of halfspaces and convex hulls. A polyhedron is a generalization of a polygon to n dimensions. We can define it either as an intersection of finitely many half-spaces (i.e., the closure of one “side” of a hyperplane) or, if it is bounded, as the “convex hull” of finitely many points. An explicit goal of this project is to formalize enough of the basic definitions and results in polyhedral geometry so that we can write down the equivalence of the two definitions above. We will follow the proof outline in chapter 1 of Gaku Liu’s notes.  
- **Notes**: [Gaku Liu’s notes](https://drive.google.com/file/d/1TRg7iQ0RpIRteF2IUiKIe3E-YagVnkH0/view?usp=sharing)  
- **Code**: [GitHub repo](https://github.com/uw-math-ai/lean-polyhedral-geometry)

#### Project 2: Reinforcement Learning for Efficient Arithmetic Circuit Generation of Polynomials
- **Mentors**: Prof. Jarod Alper, Mathematics  
- **Students**: Alexandre Borentain, Hansel Lee, Claire Xu, and Weikun Zhang  
- **Description**: We will attempt to use reinforcement learning to train computers to search for efficient arithmetic circuits computing specific polynomials. In some sense, this is a simplified version of proof generation, where computers are trained to search for proofs of theorems, except that in this case the search space is smaller. Our inspiration is the AlphaZero algorithm for two-player games, which we will adapt to a one-player game. The problem we will attack is to find efficient ways to compute a polynomial \(f(x_1, \dots, x_n)\) using an arithmetic circuit consisting of + and × gates together with scalar multiplication. Our strategy is to use Monte Carlo Tree Search to train a deep neural network to learn an effective evaluation function (giving a score of how close the current state is from computing the polynomial) and a policy (a probability distribution over the next moves, with higher probability given to moves that simplify the expression). The computer is rewarded when it finds efficient arithmetic circuits.  
- **Code**: [GitHub repo](https://github.com/uw-math-ai/PolyArithmeticCircuitsRL)

#### Project 3: Metaprogramming and Writing New Tactics
- **Mentors**: Dhruv Bhatia, Mathematics  
- **Students**: Dowland Aiello, Joseph Qian, Veer Shukla, Annis Wu  
- **Description**: Teaching a person a proof is one thing, but explaining it to a computer is another beast. The computer demands explicit precision, down to the tiniest of details. Thus, any good theorem prover needs tools, or "tactics," that make theorem proving less tedious and more akin to the way people reason. Lean comes with a built-in "metaprogramming" framework that allows users to build custom tools for automatic proof generation of specific goals. In this project, students learn about functional programming and monads before tackling the basics of metaprogramming. At the end, they write their own tactics. The current task at hand is to write a tactic that can, given a set of hypotheses of the form "a < b" where a and b come from a partially ordered type, automatically prove a goal of the same form by chaining together relevant hypotheses. We use the book *Metaprogramming in Lean 4* as a reference.  
- **Reference**: [Metaprogramming in Lean 4](https://leanprover-community.github.io/lean4-metaprogramming-book/)  
- **Code**: [GitHub repo](https://github.com/dhruvashok/partial_order_tactic.git)

#### Project 4: Neural Theorem Proving
- **Mentors**: Vasily Ilin, Mathematics  
- **Students**: Henry Adams, Siyuan Ge, Attila Jamilov, Elizabeth Wang  
- **Description**: Formalization is the process of translating human-written mathematical proofs into a form that can be verified by a computer. A popular tool for this is Lean, a proof assistant that represents proofs as code. However, the process of formalizing proofs in Lean can be slow and time-consuming. Our research explores neural theorem proving strategies, which aim to automate the generation of Lean proofs. We propose a tree-based search framework to formalize mathematical theorems in Lean using language models. This approach explores potential proof steps as branches in a tree, using AI models to suggest "tactics" at each node. This has the benefit of avoiding hallucinations by rigorously checking that AI suggestions represent valid Lean code. We employ both Large Language Models such as Claude Sonnet 3.5 and specialized fine-tuned Small Language Models such as Lean-Dojo. We use Pantograph to interact with Lean, leveraging its native support of Monte Carlo tree search. We assemble a small set of simple and medium-difficulty mathematical theorems to benchmark against, called **nanoF2F**. Additionally, we benchmark our system on the well-established **miniF2F** benchmark created by OpenAI.  
- **Code**: [GitHub repo](https://github.com/uw-math-ai/autoformalization-with-llms)

#### Project 5: Matrix Manipulation and Linear Algebra in Lean
- **Mentors**: Prof. Eric Klavins, Electrical and Computer Engineering, and Haoming Ning  
- **Students**: David Bataresh and Hemkesh Bandi  
- **Description**: Lean is a proof assistant that can be used to encode and check mathematical results in machine-readable code and could one day be used to assist in the development of complex engineering systems. First, however, we need to teach it the foundations of engineering mathematics. In this project, students will contribute to a Lean library of basic results and tactics involving matrices and linear algebra. The overall goal is to support reasoning about a variety of engineering areas that depend on linear algebra, including control systems, quantum computing, and machine learning. Thus, sub-projects will begin with a result in one of these areas and work backwards to the basic results needed to support that result.  
- **Code**: [GitHub repo](https://github.com/HemkeshB/relations-linAlg-SP25-LEAN)

---

### Final Projects for Math 480: Introduction to Mathematical Formalization

#### Project 6: Proving Strong Normalization of the Calculus of Constructions
- **Mentors**: Jarod Alper and Vasily Ilin  
- **Student**: Dowland Aiello  
- **Description**: Proofs of strong normalization of the simply-typed lambda calculus have been exhaustively enumerated in the literature. A common strategy invented by W. W. Tait known as "Tait’s method" interprets types as sets of "well-behaving" terms which are known to be strongly normalizing and composed of expressions in some such set. Strong normalization of the typed SK combinator calculus has been comparatively under-studied. Herein, I demonstrate that the typical proof of strong normalization using Tait’s method holds for the typed SK combinator calculus. I also show that decomposition of the STLC into SK combinator expressions simplifies the typical proof of strong normalization.  
- **Code**: [GitHub repo](https://github.com/dowlandaiello/coc-lean)  
- **Book**: [Online link](https://dowlandaiello.com/sk-lean/)

#### Project 7: Formalizing Vizing’s Theorem in Lean
- **Mentors**: Jarod Alper and Vasily Ilin  
- **Students**: Zayna Aarbi, Helinda He, and Manish Gatti  
- **Description**: The goal is to formalize Vizing’s Theorem: every simple, undirected graph may be properly edge-colored using a number of colors that is at most one larger than the maximum degree of the graph.  
- **Code**: [GitHub repo](https://github.com/ManishSaiGatti/Math480GroupProject)  
- **Slides**: [Google Slides](https://docs.google.com/presentation/d/1N_uLORDeTjfh0iEFjjXzPVdvG6R7htz3ZhWcDOgj9-A/edit?usp=sharing)

#### Project 8: The Six-Color Theorem
- **Mentors**: Jarod Alper and Vasily Ilin  
- **Students**: Sravani Panuganti, Jeb Song, and Taylor Woodward  
- **Description**: Every simple planar graph can be properly colored with six colors. The motivation is that this is a stepping stone to the more general "five-color theorem", which in turn is a stepping stone to the "four-color theorem".  
- **Code**: [GitHub repo](https://github.com/SravaniPanu/25sp-6color)  
- **Slides**: [Google Slides](https://docs.google.com/presentation/d/1iIT73WHGqPq3Ekz5saI8R2yKzsFDOWWNuSBbs1ZqcqU)

#### Project 9: Formalizing Using LLMs
- **Mentors**: Jarod Alper and Vasily Ilin  
- **Students**: Drew Bladek, Simon Chess, and Evan Wang  
- **Description**: Large language models (LLMs) have demonstrated fairly impressive results in mathematical reasoning and proof generation. However, when applied to the Lean proof assistant, these models tend to generate code with subtle syntax errors, limiting their practical utility in auto-formalization without human intervention. In this work, we focus on improving the syntactic fluency of LLMs when generating Lean code, without targeting the correctness of mathematical content itself. We curate a small but diverse dataset of Lean code snippets and fine-tune an open-source LLM, and evaluate the syntactic validity of the model’s outputs using automated Lean parsers.  
- **Code**: [GitHub repo](https://github.com/aurasoph/lean-dataset)

---

### AG Group Formalization Project

#### Project 10: Regular Local Rings
- **Contributors**: Jarod Alper and Brian Nugent  
- **Description**: We have formalized the definition and some of the first properties of regular local rings. Specifically, we have proved that regular local rings are domains and that one-dimensional regular local rings are PIDs. We hope to further formalize (1) relationships between regular local rings and regular sequences, (2) Koszul complex, (3) regular local rings are Cohen-Macaulay, (4) characterization of regularity in terms of projective dimension (Auslander–Buchsbaum–Serre), and (5) regular local rings are UFDs (Auslander–Buchsbaum).  
- **Code**: [GitHub repo](https://github.com/JarodUW/RegularLocalRings)


## Winter 2025

### Formalization Projects

#### Project 1: Formalizing Zariski Spaces
- **Mentors**: Leo Mayer (lead)
- **Students**: Maria Berova (mberova@uw.edu)
- **Description**: [Link](https://math.washington.edu/~jarod/xll.html)

#### Project 2: Formalizing Central Limit Theorem
- **Mentors**: Vasily Ilin (lead)
- **Students**: Siyuan Ge (jamesgsy@uw.edu)
- **Description**: [Link](https://math.washington.edu/~jarod/xll.html)
- **Code**: [Link](https://github.com/uw-math-ai/central_limit_theorem)

#### Project 3: Examples and Counterexamples in Commutative Algebra
- **Mentors**: Jarod Alper (lead)
- **Description**: Construct various examples of commutative rings in Lean. To start, construct an example of a ring that is not an integral domain. (Tricky question: is the zero ring an integral domain and can you formalize it?) How about a ring that is not a PID or not a UFD? Or a non-noetherian ring? Or a noetherian local ring that is not regular. Once we construct together a few basic examples, we will pursue further examples depending on the interests of the students.

#### Project 4: Formalizing Polyhedral Geometry
- **Mentors**: Caelan Ritter (lead)
- **Description**: A polyhedron is a generalization of a polygon to n dimensions. We can define it either as an intersection of finitely many half-spaces (i.e., the closure of one "side" of a hyperplane) or, if it is bounded, as the "convex hull" of finitely many points. The goal of this project is to formalize enough of the basic definitions and results in polyhedral geometry so that we can write down the equivalence of the two definitions above. We will follow the proof outline in chapter 1 of Gaku Liu's notes.
- **Code**: [Link](https://github.com/uw-math-ai/lean-polyhedral-geometry)

#### Project 5: Metaprogramming and Writing New Tactics
- **Mentors**: Dhruv Bhatia (lead)
- **Students**: Dhruv Ashok and Joseph Qian (Joseph is not officially registered for WXLL, but is participating informally as a continuation from last quarter)
- **Description**: Learn Lean's metaprogramming framework for tactic writing. Use this to write new tactics. The current task at hand is to write a tactic that can, given a set of hypotheses of the form a < b where a and b come from a partially ordered type, prove a goal of the same form by chaining together relevant hypotheses. If we are able to finish this project, we will move on to other tactics/help with the metaprogramming groundwork for Vas's Auto-formalization project.

### AI Projects

#### Project 6: Reinforcement Learning for Proof Generation
- **Mentors**: Jarod Alper (lead), William Dudarov, Michael Zeng
- **Description**: We will attempt to use reinforced learning to solve a simplified version of proof generation. Our inspiration is the AlphaZero algorithm for two-players games, which we will adapt to a one-player game. The problem we will attack is to find efficient ways to compute a polynomial f(x_1, …, x_n) using an arithmetic circuit consisting of + and x gates together with scalar multiplication. Our strategy is to train a deep neural network consisting of an evaluation (indicating whether the model thinks the polynomial is efficiently computable) and a policy (a probability distribution over the next moves, with higher probability given to moves that simplify the expression). The computer is rewarded when it finds efficient arithmetic circuits.
- **References**: 
  - Alphazero: "Mastering Chess and Shogi by Self-Play with a General Reinforcement Learning Algorithm" by Silver, et al, [link](https://arxiv.org/abs/1712.01815)
- **Code**: [Link](https://github.com/kyleAlexandad/RL-group-6Ver-new )

#### Project 7: Auto-formalization with LLMs
- **Mentors**: Vasily Ilin (lead), Zihong Lin(?)
- **Description**: [Link](https://math.washington.edu/~jarod/xll.html)
- **Code**: [Link](https://github.com/uw-math-ai/autoformalization-with-llms)

#### Project 8: What Mathematical Functions Can Neural Networks Learn?
- **Mentors**: Jarod Alper (lead), Michael Zeng (TA)
- **Description**: We will investigate to what extent certain mathematical functions can be efficiently learned by multilayered neural networks. Can a neural network be trained to compute modular arithmetic? Modular arithmetic is important in cryptography, and some cryptosystems use the fact that linear regression (i.e., given an integer N and pairs (x_i,y_i), find m and b such that y = mx+b (mod N) closely approximates (x_i, y_i)). Can certain number theoretic functions be computed such as the Mobius function \mu(n)? Can transformers be trained to make linear algebra computations?
- **Code**: [Link](https://github.com/hilalmufti/what-functions-can-nns-learn)

## Fall 2024

- **Formalizing examples and counterexamples in commutative algebra** (Jarod Alper)  
  While most of undergraduate mathematics has been formalized, there has been relatively little focus on formalizing examples and counterexamples. We will address this and learn Lean in the process. We will start with simple examples, such as providing rings that are not integral domains or noetherian, then move onto more complicated examples like rings of integers that are not PIDs/UFDs. Students will be free to choose the exact examples based on their interests.

- **Metaprogramming and Tactics in Lean** (Dhruv Bhatia)  
  Lean is great because it can check our proofs for us. But wouldn't it be greater if it could also automate parts of the proof writing process itself? Tactics are tools built into Lean that do exactly this. In this project, we will learn about metaprogramming - the process of writing code in Lean to change its own functionality. Along the way, we'll encounter type theory, monads, and other concepts from functional programming, while diving deep into how lean actually works under the hood. Finally, we'll use these tools to write our own tactic for anyone in the lean community to use! Students are encouraged to propose their own potential tactics.

- **Generating Functions** (Herman Chau)

- **Central Limit Theorem** (Vasily Ilin)  
  CLT is a central (pun intended) result in probability and statistics, and yet it is not in mathlib. Let's fix it!

- **Topology for Algebraic Geometry** (Leopold Mayer)

## Winter 2024

- **Faculty mentors**: Jarod Alper, Andy Heald
- **Graduate student mentors**: Herman Chau, Vasily Ilin, Leopold Mayer
- **Student participants**: Dale Dai, Yujia Dai, Siyuan Ge, Tess Gerrard, Kenneth Gong, Daniel Hughes, Mitchell Levy, Benjamin Li, Xinyan Li, Nathan Louie, Rina Reimer, Alexander Sanchez, Qiguang Yan, Christie Yang, Steven Zhong

### Projects:
- **FRACTRAN**
  - Implement the programming language [FRACTRAN](https://en.wikipedia.org/wiki/FRACTRAN) in Lean and write the adder in FRACTRAN.
  - Members: Vasilly Ilin, Alex Sanchez, Mitchell Levy
  - [GitHub code](https://github.com/sanchace/FRACTRAN)

- **Continued Fraction Expansion for e** (continued from Fall 2023)
  - The continued fraction expansion of e is [1, 0, 1, 1, 2, 1, 1, 4, 1, 1, 6, 1, 1, 8, 1, 1, 10, …]
  - Members: Xinyan Li, Leopold Mayer, Christie Yang
  - [GitHub code](https://github.com/leomayer1/cont_frac)

- **Witt's Cancellation Theorem** (continuation from Fall 2023)
  - Thm: Let ⟨-,-⟩ be a symmetric bilinear form (i.e. ⟨x,y⟩ = ⟨y,x⟩ for all x,y ∈ V). Suppose that there is form-preserving map g: U → U' where U, U' ⊂ V are subspaces. Then there is a form-preserving map f: V → V extending g.
  - Cor: U ⊕ V ≅ W ⊕ V ⟹ U ≅ W.
  - Members: Andy Heald, Nathan Louie, Sarah Mathison, Qiguang Yan

- **Formalizing Math 300** (continuation from Fall 2023)
  - Goal: Formalize the exercises (and possibly results) in the Math 300 textbook by Conroy--Taggart: *An Introduction to Mathematical Reasoning*.
  - Write a Lean guide for students taking Math 300
  - [GitHub code](https://github.com/StevennZZZ/FormalizingMATH300/)
  - Members: Chengyu (Kenneth) Gong, Rina Reimer, Tess Gerrard, Anthony Xing, Yanzhe (Steven) Zhong

## Fall 2023

- **Faculty mentors**: Jarod Alper, Andy Heald, James Morrow
- **Graduate student mentors**: Herman Chau, Vasily Ilin, Leopold Mayer
- **Undergraduate TA**: Zilu (Luca) Li
- **Student participants**: Anthony Xing, Benjamin Li, Chengyu Gong, Christie Yang, George King, Nathan Louie, Qiguang Yan, Sarah Mathison, Xinyan Li, Yanzhe (Steven) Zhong, Yu He Zhang, Zhongrui An

### Projects:
- **Continued Fraction Expansion for e**
  - The continued fraction expansion of e is [1, 0, 1, 1, 2, 1, 1, 4, 1, 1, 6, 1, 1, 8, 1, 1, 10, …].
  - Members: Xinyan Li, Leopold Mayer, Christie Yang
  - [GitHub code](https://github.com/leomayer1/cont_frac)

- **Witt's Cancellation Theorem**
  - Thm: Let ⟨-,-⟩ be a symmetric bilinear form (i.e. ⟨x,y⟩ = ⟨y,x⟩ for all x,y ∈ V). Suppose that there is form-preserving map g: U → U' where U, U' ⊂ V are subspaces. Then there is a form-preserving map f: V → V extending g.
  - Cor: U ⊕ V ≅ W ⊕ V ⟹ U ≅ W.
  - Members: Andy Heald, Nathan Louie, Sarah Mathison, Qiguang Yan

- **Random Graphs**
  - Goal: Build a random graph G(n,p) with n = # of nodes with p = probability of an edge. Show that the expected number E(# edges in G(n,p)) of edges in a random graph G(n,p) is (n choose 2)p. Related goals: compute other expected numbers, e.g. number of triangles in a random graph.
  - [GitHub code](https://github.com/uw-math-ai/random_graphs)
  - Members: Zhongrui An, Hermann Chau, Vasily Ilin, George King, Benjamin Li, Yu He Zhang

- **Formalizing Math 300**
  - Goal: Formalize the exercises (and possibly results) in the Math 300 textbook by Conroy--Taggart: *An Introduction to Mathematical Reasoning*.
  - Write a Lean guide for students taking Math 300
  - [GitHub code](https://github.com/StevennZZZ/FormalizingMATH300/)
  - Members: Yanzhe (Steven) Zhong, Anthony Xing, Luca Li, Chengyu (Kenneth) Gong

## Spring 2023

- **Faculty mentor**: Jarod Alper
- **Graduate student mentors**: Vasily Ilin, Leopold Mayer
- **Student participants**: Dhruv Ashok, Gregory Baimetov, Zachary Banken, Dianna E., Luca Li, Lawrence Lin, Rico Qi, Timothy Tran, Alfie Xu, Edward Yu
- **Github repository**: [vilin97](https://github.com/uw-math-ai/LLL)

### Projects:
- **Lagrange's Theorem** (Dhruv Ashok)
  - If G is a finite group and H ⊆ G is a subgroup, then the order of H divides the order of G.

- **Abstract term rewriting** (Gregory Baimetov)
  - Goal: The confluence and the Church-Rosser property are equivalent (see [wikipedia](https://en.m.wikipedia.org/wiki/Confluence_(abstract_rewriting))).
  - Goal: Formalize the principle of well-founded induction (see [wikipedia](https://en.m.wikipedia.org/wiki/Well-founded_relation)).

- **Simplicial homology / tactics** (Zachary Banken)
  - Goal: Formalize simplicial homology including definitions of simplicial complexes, faces, and the chain group as well that the square of the boundary operator is zero.
  - Functional programming and writing simple tactics in Lean.

- **Linear algebra** (Dianna E.)
  - If V is a vector space and S, T: V → V are linear transformations such that the range of S is contained in the nullspace of T, then (ST)² = 0.

- **Compactness** (Luca Li)
  - If X is a compact space, then every closed subset is also compact.
  - If (X,d) is a metric space and every infinite subset of X has a cluster point, then X is sequentially compact.

- **Banach Fixed Point Theorem** (Lawrence Lin)
  - If (X,d) is a non-empty complete metric space and T: X → X is a contraction mapping, then T has a unique fixed point.

- **Euclidean Geometry** (Rico Qi and Edward Yu)
  - Goal: formalize Euclidean Geometry based on Hilbert's Axioms by defining points, lines, angles, and the notion of distance.
  - Formalize a solution to [Problem 1](https://artofproblemsolving.com/wiki/index.php/2023_USAMO_Problems/Problem_1) on USAMO 2023.

- **Graph theory** (Timothy Tran)
  - Goal: Every tree on n vertices has n-1 edges.

- **Mean Value Theorem** (Alfie Xu)
  - Formalize the Mean Value Theorem (currently relying on Rolle's Theorem).

## Winter 2023

- **Faculty mentor**: Jarod Alper
- **Graduate student mentors**: Vasily Ilin, Leopold Mayer
- **Student participants**: Gregory Baimetov, Zachary Banken, William Dudarov, Griffin Golias, Raymond Guo, Eva Hu, Luca Li, Lawrence Lin, Alex Sanchez
- **Github repository**: [vilin97](https://github.com/uw-math-ai/LLL)

### Projects:
- **Identities of the Fibonacci sequence Fn** (Lawrence Lin)
  - F₍ₙ₎F₍ₙ₊₂₎-F₍ₙ₊₁₎² = (-1)^(n+1)
  - F₍ₙ₎F₍ₘ₊ₙ₎ = F₍ₙ₊₁₎F₍ₘ₎ + F₍ₙ₎F₍ₘ₋₁₎
  - m | n ⟹ F₍ₘ₎ | F₍ₙ₎
  - Binet's Formula: F₍ₙ₎ = (1/√5)((1+√5)/2)^n - ((1-√5)/2)^n)

- **Group theory exercises from Herstein *Abstract Algebra*** (Alex Sanchez)
  - Let G be an abelian group, and let h₁, h₂ ∈ G be elements. Prove that there exists an element h ∈ G whose order is the least common multiple of the orders of h₁ and h₂.
  - Let G be an abelian group, and let H₁, and H₂ be subgroups. Prove that there exists a subgroup of G whose order is the least common multiple of the orders of H₁ and H₂.

- **Topology** (Zilu Li)
  - If f : X → Y is a quotient map, then for each y ∈ Y the set f⁻¹({y}) is connected. If Y is connected, then so is X.
  - If a set is connected, then so is its closure.
  - In a metric space (X,d), the following are equivalent: (a) X is compact, (b) Every infinite subset of X has a cluster point, (c) Every sequence in X has a convergent subsequence, (d) X is complete and totally bounded, (e) X is totally bounded and has the Lebesgue property.

- **Commutative algebra** (Raymond Guo)
  - An integral domain is a PID if and only if every prime ideal is principal.

- **Sequences** (Zachary Banken, Gregory Baimetov)
  - Beatty's Theorem (aka Rayleigh's Theorem): see [wikipedia](https://en.wikipedia.org/wiki/Beatty_sequence).
  - Uspensky's Theorem: it is not possible to partition the natural numbers using 3 or more Beatty sequences.

## Fall 2022

- **Faculty mentor**: Jarod Alper
- **Graduate student mentors**: Vasily Ilin, Leopold Mayer
- **Student participants**: Zachary Banken, Griffin Golias, Raymond Guo, Eva Hu, Hastin Kapoor, Luca Li, Lawrence Lin, Alex Sanchez
- **Github repositories**: [raymondpg](https://github.com/raymondpg/XLL), [vilin97](https://github.com/uw-math-ai/LLL)

**Project**: Formalizing solutions to exercises from undergraduate math textbooks such as Axler's book [Linear Algebra Done Right](https://linear.axler.net/), Mukres's book *Topology; a first course*, Silverman's book *A Friendly Introduction to Number Theory*, Silverman and Tate's book *Rational Points on Elliptic Curves*, Folland's book *Advanced Calculus*, Rudin's book *Principles of Mathematical Analysis*, and Hungerford's book *Abstract Algebra: An Introduction.*

## Spring 2022

**Formalizing Hilbert's Basis Theorem**
- **Faculty mentor**: Jarod Alper
- **Graduate student mentors**: Vasily Ilin, Leopold Mayer
- **Student participants and contributors**: Griffin Golias, Kevin Kuei, Brendan Murphy, Alex Scheffelin, Runchi Tan
- **Project**: Developed our own library for ideals of commutative rings and formalized Hilbert's 1890 proof that ideals in polynomial rings are finitely generated.
- [GitHub](https://github.com/leomayer1/WXML_Sp2022)

