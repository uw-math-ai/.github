# Math AI Lab at UW

The Math-AI lab provides a space for mathematicians at any level (faculty, postdocs, PhD students, undergraduates, high school students, ...) to learn about formalizing mathematics with Lean, as well as learn about the intersection between Math and AI. 

We also have a research [seminar](https://math.washington.edu/events/series/math-ai-seminar).

<img src="https://github.com/user-attachments/assets/171af19b-f9f7-4006-bc80-226edb2d6391" width="50%">


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

#### Project 3: Examples and Counterexamples in Commutative Algebra
- **Mentors**: Jarod Alper (lead)
- **Description**: Construct various examples of commutative rings in Lean. To start, construct an example of a ring that is not an integral domain. (Tricky question: is the zero ring an integral domain and can you formalize it?) How about a ring that is not a PID or not a UFD? Or a non-noetherian ring? Or a noetherian local ring that is not regular. Once we construct together a few basic examples, we will pursue further examples depending on the interests of the students.

#### Project 4: Formalizing Polyhedral Geometry
- **Mentors**: Caelan Ritter (lead)
- **Description**: A polyhedron is a generalization of a polygon to n dimensions. We can define it either as an intersection of finitely many half-spaces (i.e., the closure of one "side" of a hyperplane) or, if it is bounded, as the "convex hull" of finitely many points. The goal of this project is to formalize enough of the basic definitions and results in polyhedral geometry so that we can write down the equivalence of the two definitions above. We will follow the proof outline in chapter 1 of Gaku Liu's notes.

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

#### Project 7: Auto-formalization with LLMs
- **Mentors**: Vasily Ilin (lead), Zihong Lin(?)
- **Description**: [Link](https://math.washington.edu/~jarod/xll.html)

#### Project 8: What Mathematical Functions Can Neural Networks Learn?
- **Mentors**: Jarod Alper (lead), Michael Zeng (TA)
- **Description**: We will investigate to what extent certain mathematical functions can be efficiently learned by multilayered neural networks. Can a neural network be trained to compute modular arithmetic? Modular arithmetic is important in cryptography, and some cryptosystems use the fact that linear regression (i.e., given an integer N and pairs (x_i,y_i), find m and b such that y = mx+b (mod N) closely approximates (x_i, y_i)). Can certain number theoretic functions be computed such as the Mobius function \mu(n)? Can transformers be trained to make linear algebra computations?

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
  - [GitHub code](https://github.com/Vilin97/random_graphs)
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
- **Github repository**: [vilin97](https://github.com/Vilin97/LLL)

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
- **Github repository**: [vilin97](https://github.com/Vilin97/LLL)

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
- **Github repositories**: [raymondpg](https://github.com/raymondpg/XLL), [vilin97](https://github.com/Vilin97/LLL)

**Project**: Formalizing solutions to exercises from undergraduate math textbooks such as Axler's book [Linear Algebra Done Right](https://linear.axler.net/), Mukres's book *Topology; a first course*, Silverman's book *A Friendly Introduction to Number Theory*, Silverman and Tate's book *Rational Points on Elliptic Curves*, Folland's book *Advanced Calculus*, Rudin's book *Principles of Mathematical Analysis*, and Hungerford's book *Abstract Algebra: An Introduction.*

## Spring 2022

**Formalizing Hilbert's Basis Theorem**
- **Faculty mentor**: Jarod Alper
- **Graduate student mentors**: Vasily Ilin, Leopold Mayer
- **Student participants and contributors**: Griffin Golias, Kevin Kuei, Brendan Murphy, Alex Scheffelin, Runchi Tan
- **Project**: Developed our own library for ideals of commutative rings and formalized Hilbert's 1890 proof that ideals in polynomial rings are finitely generated.
- [GitHub](https://github.com/leomayer1/WXML_Sp2022)

