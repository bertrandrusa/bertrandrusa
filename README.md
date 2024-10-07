### Hi there 👋, my name is Bertrand
#### Student to design and develop
![Student to design and develop](https://media.licdn.com/dms/image/D4D16AQHMim12AgDmBQ/profile-displaybackgroundimage-shrink_350_1400/0/1687419373915?e=1721865600&v=beta&t=VQUDzHDkKE6e9FmDnJn80VRbrPTEYcia-ptnCMlQdcI)

I am a student at Missouri State University, pursuing a Bachelor of Science in Computer Science and Mathematics. I have a big passion for technology and a strong desire to make a meaningful impact. While anyone can learn to code, my goal is to become a problem solver who uses technology to address real-world challenges.
 ## "DO WHAT YOU LOVE, LOVE WHAT YOU DO."
## Skills
💻 C++ / python / HTML / CSS/Javascript

- 🔭 I’m currently working on  couple projects 


[<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/linkedin.svg' alt='linkedin' height='40'>](https://www.linkedin.com/in/bertrand-rusanganwa-433607276/)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/instagram.svg' alt='instagram' height='40'>](https://www.instagram.com/bertrand_rusa/)  

Here’s a **cheat sheet for Finite Automata** focused on key concepts, examples, and diagrams:

---

### **Finite Automata (FA)**

1. **Definition**:
   - A Finite Automaton (FA) is a machine with a **finite number of states** used to recognize patterns within input strings.
   - **Types**:
     - **Deterministic Finite Automaton (DFA)**: Exactly one transition per input symbol.
     - **Non-deterministic Finite Automaton (NFA)**: Can have multiple transitions for a single input, including ε (empty) transitions【41†source】【44†source】.

---

### **Components of FA**:
- **States (Q)**: A finite set of states.
- **Alphabet (Σ)**: A finite set of symbols.
- **Transition Function (δ)**: Describes transitions between states based on input symbols.
- **Start State (q₀)**: The state where the machine begins.
- **Accept State (F)**: One or more accepting states that define when a string is accepted【41†source】.

---

### **DFA (Deterministic Finite Automaton)**:
- **Characteristics**:
  - For each state and input symbol, there is exactly **one transition**.
  - No ε-moves (empty transitions).
  - Accepts a string if it ends in an accept state.
- **Formal Definition**:
  - A DFA can be described as a 5-tuple: (Q, Σ, δ, q₀, F).
- **Example**:
  - DFA to recognize strings ending in `00`:
    - Q = {S1, S2, S3}
    - Σ = {0, 1}
    - δ(S1, 0) = S2, δ(S2, 0) = S3, δ(S3, 0) = S3, δ(S3, 1) = S2, etc.
    - Start State = S1, Accept State = S3【41†source】.

---

### **NFA (Non-deterministic Finite Automaton)**:
- **Characteristics**:
  - Can have **multiple transitions** for the same input from a state.
  - Can have **ε-moves**, where the machine transitions without consuming an input.
  - Accepts a string if **any** transition path leads to an accept state.
- **Formal Definition**:
  - NFA is also described by a 5-tuple: (Q, Σ, δ, q₀, F), but δ can return **multiple states** for a given input or ε-moves.
- **Example**:
  - NFA to recognize strings containing `01`:
    - Q = {S1, S2, S3}
    - Σ = {0, 1}
    - δ(S1, 0) = {S2}, δ(S2, 1) = {S3}, ε-moves possible【41†source】.

---

### **DFA vs NFA**:
- **DFA**:
  - One transition per input.
  - No ε-moves.
  - Always in one specific state at a time.
- **NFA**:
  - Multiple transitions for one input are allowed.
  - Can have ε-moves.
  - Can be in multiple states at the same time.
- **Equivalence**: Every NFA can be converted to a DFA, but the DFA might have more states【41†source】【44†source】.

---

### **Key Conversions**:

#### **NFA to DFA Conversion (Subset Construction)**:
- **Process**:
  - Each DFA state represents a **set of NFA states**.
  - Compute the ε-closure of states (set of all states reachable via ε-transitions).
  - For each input symbol, determine the set of reachable NFA states.
- **Example**:
  - If NFA states S1 and S2 can be reached on input `a`, create a DFA state representing {S1, S2}【40†source】.

---

### **Closure Properties of Finite Automata**:
- Regular languages (recognized by FA) are closed under:
  - **Union**: Combine two FA using a new start state with ε-transitions.
  - **Concatenation**: Connect the accept states of one FA to the start state of another.
  - **Kleene Star**: Add ε-transitions from accept states back to the start state【44†source】.

---

### **Regular Languages**:
- A **regular language** is one that can be recognized by a DFA or NFA.
- **Regular Expressions (RE)** describe regular languages, and every RE can be converted into an NFA【44†source】.

---

### **Important Theorems**:
- **Kleene's Theorem**: A language is regular if and only if it can be recognized by a finite automaton.
- **Pumping Lemma**: Used to prove that certain languages are not regular by showing that for large enough strings, a portion of the string can be "pumped" (repeated)【44†source】.

---

### **Key Examples**:

#### **DFA Example**:
Recognize binary strings that end in `00`:
- **States**: S1 (start), S2 (after reading 0), S3 (after reading 00).
- **Transitions**:
  - δ(S1, 0) → S2, δ(S2, 0) → S3.
  - Accept State: S3.

#### **NFA Example**:
Recognize binary strings that contain `01`:
- **States**: S1 (start), S2 (after reading 0), S3 (after reading 01).
- **Transitions**:
  - δ(S1, 0) → S2, δ(S2, 1) → S3.
  - Accept State: S3【41†source】【44†source】.

---

This cheat sheet includes the essential concepts and examples for finite automata. Make sure to focus on the differences between DFA and NFA, conversion steps, and some small examples for your reference!
