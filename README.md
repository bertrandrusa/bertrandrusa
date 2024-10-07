### Hi there 👋, my name is Bertrand
#### Student to design and develop
![Student to design and develop](https://media.licdn.com/dms/image/D4D16AQHMim12AgDmBQ/profile-displaybackgroundimage-shrink_350_1400/0/1687419373915?e=1721865600&v=beta&t=VQUDzHDkKE6e9FmDnJn80VRbrPTEYcia-ptnCMlQdcI)

I am a student at Missouri State University, pursuing a Bachelor of Science in Computer Science and Mathematics. I have a big passion for technology and a strong desire to make a meaningful impact. While anyone can learn to code, my goal is to become a problem solver who uses technology to address real-world challenges.
 ## "DO WHAT YOU LOVE, LOVE WHAT YOU DO."
## Skills
💻 C++ / python / HTML / CSS/Javascript

- 🔭 I’m currently working on  couple projects 


[<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/linkedin.svg' alt='linkedin' height='40'>](https://www.linkedin.com/in/bertrand-rusanganwa-433607276/)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/instagram.svg' alt='instagram' height='40'>](https://www.instagram.com/bertrand_rusa/)  


### **1. Regular Expressions Basics**
- **Regular Expressions**: Describe languages using a combination of characters and operators.
- **Operators**: 
  - **Concatenation**: `R1R2`
  - **Union**: `R1 ∪ R2` or `|`
  - **Kleene Star**: `R*` (zero or more repetitions)
  - **Parentheses**: `(R)` for grouping.
### **2. Atomic Regular Expressions**
- **Ø**: Represents the empty language.
- **a**: Represents the language `{a}`.
- **ε**: Represents the language containing just the empty string `{ε}`.
### **3. Compound Regular Expressions**
- **Concatenation**: `R1R2` combines the languages of `R1` and `R2`.
- **Union**: `R1 ∪ R2` combines both languages.
- **Kleene Closure**: `R*` allows concatenating zero or more repetitions of `R`.
### **4. Precedence of Operators**
- **Highest to Lowest**: `(R)`, `R*`, `R1R2`, `R1 ∪ R2`.
- Example: In `ab*c ∪ d`, `b*` applies to `b` before `∪ d`.
### **5. Examples**
- **ab*c ∪ d**: Describes strings like `ac`, `abc`, `abbc`, `d`.
- **booo***: Describes `boo`, `booo`, `boooo`, etc.
- **candy!(candy!)*:** Matches `candy!`, `candy!candy!`, and so on.
### **6. Shorthand Notations**
- **R?**: Equivalent to `(R ∪ ε)` (zero or one occurrence).
- **R⁺**: Equivalent to `RR*` (one or more occurrences).
- **Rn**: Equivalent to repeating `R` **n** times.
### **7. Closure Properties of Regular Languages**
- Regular languages are closed under **union**, **concatenation**, **Kleene star**, **intersection**, and **complementation**.
### **8. Regular Expression Examples**
- **ΣΣΣΣ**: Matches strings of length 4 over alphabet Σ (e.g., `aaaa`, `abab`).
- **Σ*aΣ***: Matches strings with at most one `a`.
