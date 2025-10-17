极限的运算
# Q1 为什么函数见的极限运算都得先满足两个函数在同一点取极限相等
🖖 Excellent and *very* deep question, Ensign — this is precisely the kind of logical curiosity Spock would admire.

You’re asking why, in these **limit properties**, we always start by saying:

[
\lim_{x\to a} f(x) = L_1, \quad \lim_{x\to a} g(x) = L_2
]

before we even apply rules like
[
\lim_{x\to a} [f(x) + g(x)] = L_1 + L_2.
]

Let’s reason through this carefully.

---

## 🧠 1. The “Existence” Principle of Limit Operations

Before you can *combine* two limits, each limit must **exist** individually.

If even one of them fails (does not exist, diverges, oscillates, etc.),
the combination may not be meaningful.

Think of it like this:

> You can’t add two unknown destinations if one of the travelers never arrives.

Mathematically:

* (\lim_{x\to a} f(x)) must converge to a finite number (L_1).
* (\lim_{x\to a} g(x)) must converge to a finite number (L_2).

Only *then* can we meaningfully discuss (L_1 + L_2, L_1 L_2, \frac{L_1}{L_2}), etc.

---

## ⚙️ 2. Logical Foundation of Limit Algebra

These rules (1–4 on your board) are derived from the **definition of limit** itself:

> If two functions both get arbitrarily close to their respective limits as (x\to a),
> then their sum/product/etc. will also get arbitrarily close to the corresponding combined value.

Formally:
[
\forall \varepsilon>0,\exists \delta>0: |f(x)-L_1|<\varepsilon_1, |g(x)-L_2|<\varepsilon_2
\Rightarrow |f(x)\pm g(x)-(L_1\pm L_2)|<\varepsilon
]

Without the premise that both limits exist, you can’t construct this logical chain —
the “(\varepsilon-\delta)” structure collapses.

---

## 📊 3. Example — When it *doesn’t* hold

Let’s test what happens if one of the limits doesn’t exist.

[
f(x) = \sin\frac{1}{x}, \quad g(x) = 1
]

As (x\to0):

* (\lim f(x)) **does not exist** (oscillates between −1 and 1).
* (\lim g(x) = 1).

Now:
[
\lim_{x\to0} [f(x)+g(x)] = 1 + \sin\frac{1}{x}
]
also **does not exist**, because it inherits (f(x))’s oscillation.

→ If even one limit fails, the combined limit fails too.

That’s why we *require* both (\lim f(x)) and (\lim g(x)) to exist first.

---

## 🧭 4. Summary Table

| Operation     | Valid only if      | Result            |
| ------------- | ------------------ | ----------------- |
| (f+g)         | Both limits finite | (L_1+L_2)         |
| (f-g)         | Both limits finite | (L_1-L_2)         |
| (f\cdot g)    | Both limits finite | (L_1L_2)          |
| (\frac{f}{g}) | (\lim g(x)\ne0)    | (\frac{L_1}{L_2}) |
| ([f(x)]^n)    | Limit exists       | ((L_1)^n)         |

If one side “breaks,” the rule is no longer guaranteed.

---

## 🪐 Bridge Commentary

**Professor Leonard:**

> “Before you add limits, make sure they *exist*. You can’t build a structure without foundations.”

**Spock:**

> “Logical consistency requires each component to converge independently. Otherwise, the combined expression lacks definition.”

**Kirk:**

> “In calculus as in command — stability of the whole depends on stability of each part.”

---

Would you like me to show one *counterexample* visually —
where (\lim f(x)) and (\lim g(x)) don’t both exist,
so their sum or ratio explodes or oscillates?
