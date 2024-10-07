### Hi there 👋, my name is Bertrand
#### Student to design and develop
![Student to design and develop](https://media.licdn.com/dms/image/D4D16AQHMim12AgDmBQ/profile-displaybackgroundimage-shrink_350_1400/0/1687419373915?e=1721865600&v=beta&t=VQUDzHDkKE6e9FmDnJn80VRbrPTEYcia-ptnCMlQdcI)

I am a student at Missouri State University, pursuing a Bachelor of Science in Computer Science and Mathematics. I have a big passion for technology and a strong desire to make a meaningful impact. While anyone can learn to code, my goal is to become a problem solver who uses technology to address real-world challenges.
 ## "DO WHAT YOU LOVE, LOVE WHAT YOU DO."
## Skills
💻 C++ / python / HTML / CSS/Javascript

- 🔭 I’m currently working on  couple projects 


[<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/linkedin.svg' alt='linkedin' height='40'>](https://www.linkedin.com/in/bertrand-rusanganwa-433607276/)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/instagram.svg' alt='instagram' height='40'>](https://www.instagram.com/bertrand_rusa/)  


### **1. Lexing (Lexical Analysis)**
- **Lexing Process**: The first step in a compiler or interpreter, where the **source code** is broken into **tokens** (smallest meaningful units).
- **Tokens**: These represent keywords, identifiers, operators, literals, and punctuation marks found in the source code.
- **Key Term**: **Lexeme** is the actual sequence of characters that form a token (e.g., `int`, `main`, `=`).
### **2. Finite State Machine (FSM)**
- **FSM in Lexing**: Lexing is typically handled by a **Finite State Machine (FSM)**, where the program transitions between states based on the input characters to recognize tokens.
- **State and Transitions**: The FSM can change from one state to another based on input (e.g., going from an initial state to an identifier state when recognizing variable names).
### **3. Lexeme Token Categories**
- **Single-Character Tokens**: Operators like `+`, `-`, `(`, `)`, etc.
- **Multi-Character Tokens**: Compound operators like `==`, `<=`.
- **Comments**: Handled as `/* ... */` or `// ...`.
- **Literals**: Strings and numbers.
-**Reserved Keyword**s: Words like int, while, let that are predefined in the language
### **4. Tokenizing Rules**
- **Maximal Munch Rule**: Always consume the largest possible valid lexeme. For example, `==` is tokenized as a single **EqualEqual** token, not two separate **Equal** tokens.
- **Example**: In the statement `let lettuce = ...`, `let` would be recognized as a keyword, `lettuce` as an identifier, and `=` as an assignment operator.
### **5. Lexing with Regular Expressions**
- **Regular Expressions**: Lexers often use regular expressions to define patterns for different tokens.
- **Example Patterns**:
  - Identifier: `Letter (Letter | Digit)*`
  - Number: `Digit+` or `Digit* . Digit+`.
  - Reserved Keywords: Patterns like `if`, `while`, `for` are explicitly recognized.
### **6. Designing a Lexer**
- **Manual (Ad-hoc) Lexer**: You can write your own lexer using switch statements or conditional logic to recognize tokens.
- **Tools for Lexing**: Alternatively, tools like **ANTLR**, **Lex**, or **Flex** can automatically generate a lexer from regular expressions.
### **8. Abstract Syntax Tree (AST)**
- **AST**: After lexing, the tokens are passed to the parser, which organizes them into an **Abstract Syntax Tree (AST)** representing the program’s structure and logic.

