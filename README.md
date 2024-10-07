### Hi there 👋, my name is Bertrand
#### Student to design and develop
![Student to design and develop](https://media.licdn.com/dms/image/D4D16AQHMim12AgDmBQ/profile-displaybackgroundimage-shrink_350_1400/0/1687419373915?e=1721865600&v=beta&t=VQUDzHDkKE6e9FmDnJn80VRbrPTEYcia-ptnCMlQdcI)

I am a student at Missouri State University, pursuing a Bachelor of Science in Computer Science and Mathematics. I have a big passion for technology and a strong desire to make a meaningful impact. While anyone can learn to code, my goal is to become a problem solver who uses technology to address real-world challenges.
 ## "DO WHAT YOU LOVE, LOVE WHAT YOU DO."
## Skills
💻 C++ / python / HTML / CSS/Javascript

- 🔭 I’m currently working on  couple projects 


[<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/linkedin.svg' alt='linkedin' height='40'>](https://www.linkedin.com/in/bertrand-rusanganwa-433607276/)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/instagram.svg' alt='instagram' height='40'>](https://www.instagram.com/bertrand_rusa/)  


Here’s a **cheat sheet** based on the requested slides from **Conversions Between RE and FSM** and **Proof of Regular/Non-Regular Languages**:
### **1. NFA → DFA Conversion (Subset Construction)**
- **Subset Construction**:
  - Start with the ε-closure of the NFA's start state as the DFA's start state.
  - For each input symbol, find the set of reachable states (ε-closure) from the current set of states.
  - Repeat this process for all states and inputs until no new states are found.
  - Each DFA state represents a **set of NFA states**.
### **2. Thompson’s Algorithm (RE to NFA)**
- **Thompson Construction**:
  - **Single Character**: Create a simple two-state NFA with the character as the transition.
  - **Concatenation (R1R2)**: Connect the NFA of `R1` to `R2` by linking `R1`'s accept state to `R2`'s start state.
  - **Union (R1 ∪ R2)**: Create a new start state with ε-transitions to the start states of `R1` and `R2`. Merge their accept states.
  - **Kleene Star (R*)**: Add ε-transitions from the accept state back to the start state, with an option to skip the NFA altogether via an ε-transition.
### **3. Subset Construction (NFA → DFA)**
- **Steps**:
  - Start from the ε-closure of the NFA start state.
  - For each input symbol, move to the set of states that can be reached (ε-closure).
  - This process continues until every possible state combination is explored.
  - The result is a DFA where each state represents a **subset of NFA states**
### **4. Using Closure Properties to Show Regular Languages**
- **Closure Properties**:
  - Regular languages are **closed** under:
    - **Union**: If `L1` and `L2` are regular, so is `L1 ∪ L2`.
    - **Concatenation**: If `L1` and `L2` are regular, so is `L1L2`.
    - **Kleene Star**: If `L` is regular, so is `L*`.
    - **Intersection and Complementation**: Regular languages are also closed under these operations.

### **5. Building Regular Expressions for Specific Languages**
- **Example: Language L = { w ∈ Σ* | w contains aa as a substring }**:
  - Regular expression: `(a ∪ b)* aa (a ∪ b)*`.
- **Example: Language L = { w ∈ Σ* | |w| = 4 }**:
  - Regular expression: `ΣΣΣΣ` (four repetitions of any symbol from Σ).
