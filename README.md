### Hi there 👋, my name is Bertrand
#### Student to design and develop
![Student to design and develop](https://media.licdn.com/dms/image/D4D16AQHMim12AgDmBQ/profile-displaybackgroundimage-shrink_350_1400/0/1687419373915?e=1721865600&v=beta&t=VQUDzHDkKE6e9FmDnJn80VRbrPTEYcia-ptnCMlQdcI)

I am a student at Missouri State University, pursuing a Bachelor of Science in Computer Science and Mathematics. I have a big passion for technology and a strong desire to make a meaningful impact. While anyone can learn to code, my goal is to become a problem solver who uses technology to address real-world challenges.
 ## "DO WHAT YOU LOVE, LOVE WHAT YOU DO."
## Skills
💻 C++ / python / HTML / CSS/Javascript

- 🔭 I’m currently working on  couple projects 


[<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/linkedin.svg' alt='linkedin' height='40'>](https://www.linkedin.com/in/bertrand-rusanganwa-433607276/)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/instagram.svg' alt='instagram' height='40'>](https://www.instagram.com/bertrand_rusa/)  

Here’s a focused cheat sheet for **Finite Automata** based on the difficult-to-remember parts from your slides:

---

Here’s the refined cheat sheet with **only answers**:

---

### **1. Key Differences: DFA vs NFA**
- In a DFA, for every state and every input symbol, there is **exactly one** transition.
- In an NFA, a state can have **multiple transitions** for the same input symbol, including ε-transitions that don’t consume input.
- An NFA accepts a string if **any one of the possible paths** leads to an accept state.
- A DFA can simulate an NFA using **subset construction**. Each DFA state represents a set of NFA states, and the DFA transitions reflect where the NFA could be after reading an input symbol.
### **2. Formal Definitions**
- **DFA Formal Definition**: 
  - \( DFA = (Q, Σ, δ, q_0, F) \)
    - \( Q \): Set of states.
    - \( Σ \): Input alphabet.
    - \( δ \): Transition function where every input symbol leads to exactly one state.
    - \( q_0 \): Start state.
    - \( F \): Set of accept states.
- **NFA Formal Definition**:
  - \( NFA = (Q, Σ, δ, q_0, F) \)
    - \( δ \): Transition function where each input can lead to **multiple states**, including ε-transitions.
- In a DFA, there can only be **one unique transition** for each input symbol from each state.
- The ε-transition in an NFA allows it to change states without consuming any input symbol.
### **3. Acceptance of a String**
- A DFA accepts a string if, after processing all symbols, it ends in an **accept state**.
- An NFA accepts a string if **any of the possible paths** leads to an accept state.
- The NFA explores all possible transitions for the input. It accepts the string if **any path** leads to an accept state, regardless of what happens on other paths.
- If an NFA doesn’t accept a string, it means **none** of the paths from the start state to the accept state are valid for that input string.
### **4. Handling Transitions**
- In a DFA, only **one transition** per input symbol is allowed from each state.
- NFAs can have **multiple transitions** for the same input symbol from the same state, as well as ε-transitions.
- DFAs do not allow ε-transitions. Every input symbol must trigger a defined transition.
- An NFA can always explore all possible paths, and if one of them leads to an accept state, it will accept the string.
### **5. Regular Language Recognition**
- The languages recognized by DFAs and NFAs are the same; they both recognize **regular languages**. Any NFA can be converted to an equivalent DFA.
- NFAs can be **more compact** and simpler to design for certain languages, even though they can be converted to DFAs lat
### **6. Transition Table and State Diagram**
- In a DFA transition table, each state has exactly one outgoing transition for each symbol in the alphabet.
- In an NFA transition table, each state can have multiple transitions for the same symbol or ε-transitions.
- When there are multiple states for a single input in an NFA transition table, it means the NFA can transition to **any of those states** upon reading the input, and all paths must be considered.
