
# 🧮 Calculus 0.2 – Introduction to Functions

> Author: Tingyi Wei  
> Reviewed by: Prof. Leonard 
> Log: Math Bridge Protocol Active

---

## 🚀 Core Idea

A **function** describes *how an input variable corresponds to a unique output variable.*

\[
f: x \mapsto y
\]

It is not just a formula or a graph — it’s a **rule of correspondence**.

---

## 💡 Key Concepts

### 1. Definition

- Every input \( x \) produces **exactly one** output \( y \).
- The function defines *dependence*:  
  - **Independent variable:** the chosen input  
  - **Dependent variable:** output determined by the rule

---

### 2. Function Examples

| Example | Description |
|----------|--------------|
| \( f(x) = x^2 \) | Maps every number to its square |
| \( f(x) = \sin x \) | Maps angles to their sine value |
| *Real-world:* “One student → one final grade” | Function-like mapping (Input → Output) |

---

### 3. Function vs Equation

- Equation (e.g., \(x^2 + y^2 = 1\)) describes a *relation* between variables.  
- Function (e.g., \(y = \sqrt{1-x^2}\)) picks *one side* of that relation — one output for each input.

---

## ⚙️ Piecewise Functions

A **piecewise function** combines several rules under different domains:

\[
f(x) =
\begin{cases}
x^2, & x < 0 \\
x + 1, & x \ge 0
\end{cases}
\]

### Key steps to analyze:

1. Identify each **domain interval**.  
2. Check **continuity** at the boundaries:  
   \[
   \lim_{x\to0^-} f(x) \text{ vs } \lim_{x\to0^+} f(x)
   \]

If limits match → continuous.  
If not → discontinuity (a “hole” or “jump”).

---

## 🧠 Knowledge Threshold Summary

| Zone | Description | Example |
|------|--------------|----------|
| ✅ **Solid Knowledge** | Function = rule; 1 input → 1 output | Student → Grade analogy |
| ⚪ **Grey Zone** | Piecewise definition and continuity at junctions | Needs practice |
| ❌ **Blind Spot** | Understanding discontinuity types (to be covered in next lesson) | — |

---

## 🌍 Big Picture 

> “Every ML model is a piecewise function in disguise.”

The **ReLU activation**  
\[
f(x) = \max(0, x)
\]
is a perfect example — two simple rules define a complex behavior.

Understanding piecewise continuity prepares you for learning **limits, derivatives, and gradient-based learning** later.

---

## 📚 Next Mission

→ Proceed to **0.3 Continuity and Limits**  
Objective: Understand what it means for a function to “connect smoothly.”

---

### 🪐 Remarks

“Causality verified. Functional mapping stable.”  
“Rules before graphs — always.”  
“You’ve seen correspondence. Next, you’ll see connection.”

---
