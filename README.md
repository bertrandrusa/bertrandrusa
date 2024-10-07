### Hi there 👋, my name is Bertrand
#### Student to design and develop
![Student to design and develop](https://media.licdn.com/dms/image/D4D16AQHMim12AgDmBQ/profile-displaybackgroundimage-shrink_350_1400/0/1687419373915?e=1721865600&v=beta&t=VQUDzHDkKE6e9FmDnJn80VRbrPTEYcia-ptnCMlQdcI)

I am a student at Missouri State University, pursuing a Bachelor of Science in Computer Science and Mathematics. I have a big passion for technology and a strong desire to make a meaningful impact. While anyone can learn to code, my goal is to become a problem solver who uses technology to address real-world challenges.
 ## "DO WHAT YOU LOVE, LOVE WHAT YOU DO."
## Skills
💻 C++ / python / HTML / CSS/Javascript

- 🔭 I’m currently working on  couple projects 


[<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/linkedin.svg' alt='linkedin' height='40'>](https://www.linkedin.com/in/bertrand-rusanganwa-433607276/)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/instagram.svg' alt='instagram' height='40'>](https://www.instagram.com/bertrand_rusa/)  


### **1. NFA → DFA Conversion (Subset Construction)**
Here’s a **simplified cheat sheet** for **Conversion Between Finite Automata (FA) and Regular Expressions (RE)**:
### **1. NFA → DFA Conversion (Subset Construction)**
- **Goal**: Convert an **NFA** (which can have multiple paths and ε-transitions) into a **DFA** (which can’t).
- **Steps**:
  1. Start with the **ε-closure** (all reachable states without consuming input) of the NFA's **start state** as the DFA's start state.
  2. For each input symbol, check where the NFA can move and record those states.
  3. Every set of NFA states becomes a **DFA state**.
  4. Continue until no new DFA states are needed.
### **2. Thompson’s Algorithm (RE to NFA)**
- **Purpose**: Convert a regular expression into an NFA using simple building blocks.
- **Steps**:
  - **Single Character (a)**: Create a two-state NFA, with `a` as the transition between them.
  - **Concatenation (R1R2)**: Connect the NFA for `R1` to the NFA for `R2`.
  - **Union (R1 ∪ R2)**: Create a new start state and accept state, and add ε-transitions to both `R1` and `R2`.
  - **Kleene Star (R*)**: Add ε-transitions to loop from the accept state back to the start, and an ε-transition to skip the entire NFA
### **3. Subset Construction (NFA → DFA)**
- **Key Idea**: Treat **each set of NFA states** as a single DFA state.
- **Steps**:
  1. Start at the **ε-closure** of the NFA’s start state.
  2. For each input, move to all reachable states and treat this as a new DFA state.
  3. Repeat for all inputs and states until the DFA is fully built.
### **4. Regular Expression to NFA Quick Guide**
- **a**: NFA for the character `a`.
- **R1R2**: Concatenate the NFAs for `R1` and `R2`.
- **R1 ∪ R2**: Use ε-transitions to create a choice between `R1` and `R2`.
- **R***: Add ε-loops to repeat the NFA, allowing zero or more occurrences.
### **5. Key Concepts**
- **ε-Closure**: All states that can be reached by ε-transitions.
- **Concatenation**: Combine two NFAs one after the other.
- **Union**: Split the path between two NFAs.
- **Kleene Star**: Allows repeating the NFA or skipping it entirely.
