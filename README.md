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

### **1. Deterministic Finite Automaton (DFA)**
- **Key Characteristic**: For each state in a DFA, there must be **exactly one transition** for every symbol in the alphabet Σ【27†source】.
- **Unique Start State**: DFAs have a single start state and can have multiple accept states【27†source】.
- **Formal Definition**: \( DFA = (Q, Σ, δ, q_0, F) \)
  - \( Q \): Set of states.
  - \( Σ \): Alphabet (set of input symbols).
  - \( δ \): Transition function (maps a state and input to another state).
  - \( q_0 \): Initial state.
  - \( F \): Set of accept states【27†source】.

---

### **2. Non-Deterministic Finite Automaton (NFA)**
- **Multiple Transitions**: NFAs can have **multiple transitions** for the same input symbol, and even **ε-transitions**, which do not consume any input【27†source】.
- **Acceptance**: An NFA accepts a string if **any one of its paths** ends in an accept state【27†source】.
- **Key Concept**: NFAs can have branches where some branches might accept and others reject, but the NFA accepts if any branch leads to an accept state【27†source】.

---

### **3. Key Differences: DFA vs NFA**

| Feature               | **DFA**                         | **NFA**                                      |
|-----------------------|---------------------------------|----------------------------------------------|
| Transitions per state  | One transition per input symbol | Multiple transitions, including ε-transitions |
| ε-transitions          | Not allowed                    | Allowed                                      |
| Acceptance             | Accepts if ends in an accept state | Accepts if **any path** ends in an accept state【27†source】 |

---

### **4. Language of a DFA**
- **Formal Language Definition**: A language \( L \) over Σ is the set of strings that can be processed by a DFA and result in acceptance【27†source】.
- **Formal Notation**: \( ℒ(D) = \{ w \in Σ^* | D \text{ accepts } w \} \)
  - This represents all strings that the DFA accepts【27†source】.

---

### **5. Transition Process (DFA/NFA)**

1. **Start at the Initial State**: Begin at the start state.
2. **Process Input**: For each input symbol, follow the transition to the next state【27†source】.
3. **Check Acceptance**: If the final state after processing the entire string is an accept state, the string is accepted【27†source】.

---

### **6. Automaton Structure**
- **States and Transitions**: Each circle represents a state. Arrows represent transitions between states【27†source】.
- **Accept States**: Depicted by double circles. A string is accepted if it ends in one of these states【27†source】.
- **Example**: For a string `101001`:
  - Process each bit starting from the initial state and move through the DFA/NFA transitions to determine if the final state is an accept state【27†source】.

---

### **7. Epsilon (ε) Transitions (NFA)**
- **Key Feature**: NFAs can transition between states without consuming any input using ε-transitions【27†source】.
- **Behavior**: The NFA may follow an ε-transition at any time but is not required to do so【27†source】.
- **Impact**: This can lead to multiple possible states being active simultaneously【27†source】.

---

### **8. Recognizing Languages with DFA**
- **DFA Language Recognition**: A DFA recognizes a **regular language**, and every regular language can be recognized by a DFA【27†source】.
- **Example Tasks**:
  - Create a DFA to accept strings with two consecutive zeros.
  - Create a DFA to accept strings that start or end with `00`【27†source】.

---

### **9. Closure Properties of Regular Languages**
- **Key Properties**:
  - Regular languages are closed under **complementation**, **union**, **intersection**, and **Kleene star**【27†source】.
  - **Complement**: If \( L \) is regular, then \( L' \) (the complement of \( L \)) is also regular【27†source】.

---

### **10. Non-Deterministic to Deterministic Conversion (NFA to DFA)**
- **Subset Construction**: Convert an NFA to a DFA by treating each set of NFA states as a single DFA state【27†source】.
  - **Key Process**: For each state in the DFA, determine the set of states the NFA could be in after processing an input symbol. Repeat until no new DFA states are found.

---

This cheat sheet highlights the difficult-to-remember concepts from the **Finite Automata** slides. These are crucial for understanding how automata work and what sets DFAs apart from NFAs.

