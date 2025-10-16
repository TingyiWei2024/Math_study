# Q1 为什么倒数里常用的是弧度？

“为什么弧度更自然”这一点，正是三角函数进入微积分体系的核心逻辑。
让我们逐层展开。

---

## 🧭 一、几何定义层面

在圆中：
[
\text{弧长 } s = r \theta
]

其中

* (s)：弧长
* (r)：半径
* (\theta)：角的弧度值

> **关键：** 这条公式只在“弧度制”下成立。
> 若用角度（degrees），还得额外乘上换算因子 (\pi/180)。

也就是说——
弧度让“角度 = 弧长/半径”这一关系**直接成立，不需换算常数**。
它把几何变成了“纯比例关系”。

---

## ⚙️ 二、微积分层面（自然单位的体现）

微积分的根本在于“极限”。
若函数是 (f(x)=\sin x)，
我们要研究其导数：

[
\lim_{h\to0}\frac{\sin(x+h)-\sin x}{h}
]

计算过程中用到的核心极限是：

[
\lim_{x\to0}\frac{\sin x}{x}=1
]

> ✅ 只有当 (x) 是**用弧度**表示时，这个极限等于 1。
> 若用角度（degree），它会变成
> (\lim_{x\to0}\frac{\sin x}{x} = \frac{\pi}{180})。

于是所有导数公式都必须额外多乘常数，变得复杂。
例如：

| 函数            | 若用弧度            | 若用角度                           |
| ------------- | --------------- | ------------------------------ |
| (f(x)=\sin x) | (f'(x)=\cos x)  | (f'(x)=\frac{\pi}{180}\cos x)  |
| (f(x)=\cos x) | (f'(x)=-\sin x) | (f'(x)=-\frac{\pi}{180}\sin x) |

> 🚀 因此，弧度制是“让数学公式最简化、最自然”的选择。

---

## 🌍 三、全局比喻

> “Degrees are human — they came from sailors and compasses.
> Radians are universal — they came from the circle itself.”

弧度是“**从圆出发**”的自然度量单位：
它不依赖于人为定义的“360°”，
而是直接由圆自身的比例定义的。
它使所有关于旋转、周期、导数、振荡的公式都不需要校正因子。

---

**Professor Leonard：**

> “Radians measure how far around you go, not how many degrees you count.”

> “Mathematical elegance emerges when constants vanish.”

> “In short, Ensign — radians are the *native language* of calculus.”

---
# Q2  三角函数定义中常见的**三边英文缩写**：

---

| 缩写       | 全写           | 含义                                                | 中文 |
| -------- | ------------ | ------------------------------------------------- | -- |
| **Opp.** | *Opposite*   | the side **opposite** the given angle θ           | 对边 |
| **Adj.** | *Adjacent*   | the side **adjacent** (next to) the given angle θ | 邻边 |
| **Hyp.** | *Hypotenuse* | the **longest side**, opposite the right angle    | 斜边 |

---

于是三角函数的定义为：

[
\sin \theta = \frac{\text{Opp.}}{\text{Hyp.}}, \quad
\cos \theta = \frac{\text{Adj.}}{\text{Hyp.}}, \quad
\tan \theta = \frac{\text{Opp.}}{\text{Adj.}}
]

---

**Professor Leonard：**

> “Every trig ratio is just a *relationship* between these three sides.”
> “Remember the triangle as a coordinate system of logic — each function is a ratio of relation.”


---

# Q3 四象限与函数符号关系
| 象限      | 常用记忆           | 正值的函数                      | 其他均为负 |
| ------- | -------------- | -------------------------- | ----- |
| **I**   | A → *All*      | 所有三角函数都为正                  | —     |
| **II**  | S → *Students* | $\sin\theta$, $\csc\theta$ | 其余负   |
| **III** | T → *Take*     | $\tan\theta$, $\cot\theta$ | 其余负   |
| **IV**  | C → *Calculus* | $\cos\theta$, $\sec\theta$ | 其余负   |

| 象限  | $x$ | $y$ | $\sin$ | $\cos$ | $\tan$ |
| --- | --- | --- | ------ | ------ | ------ |
| I   | +   | +   | +      | +      | +      |
| II  | –   | +   | +      | –      | –      |
| III | –   | –   | –      | –      | +      |
| IV  | +   | –   | –      | +      | –      |

# Q4 y= Asin(Bx)图像变化

| 参数  | 名称                         | 控制的性质              | 计算方法                     |   |   |
| --- | -------------------------- | ------------------ | ------------------------ | - | - |
| (A) | **Amplitude（振幅）**          | 决定波的“高度”，也就是波峰的最大值 | (                        | A | ) |
| (B) | **Frequency factor（频率因子）** | 决定波的“快慢”或周期长短      | 周期 (T = \dfrac{2\pi}{B}) |   |   |


| 符号变化                   | 对应变换        | 对波形影响     |
| ---------------------- | ----------- | --------- |
| (A \to -A)             | 垂直反射（绕x轴）   | 波峰波谷对调    |
| (B \to -B) 且函数是 (\sin) | 水平反射 + 垂直反射 | 相当于左右反向传播 |
| (B \to -B) 且函数是 (\cos) | 关于y轴对称      | 图像不变      |
| (A,B) 同时为负             | 双重反射        | 效果与原函数相同  |



# Notes: 🧮 Calculus 0.3 – Review of Trigonometry and Graphing

> Author: Ensign Tingyi Wei  
> Reviewed by: Prof. Leonard · Spock · Capt. Kirk  
> Ship Log: Math Bridge Protocol Active

---

## 🚀 Core Idea

Trigonometric functions describe **how the sides of a triangle vary with its angle** —  
and when extended to the coordinate plane, they become **periodic waves** that repeat over time.

---

## 🎯 Key Equations

### 1. General Form

\[
y = A\sin(Bx + C) + D \quad \text{or} \quad y = A\cos(Bx + C) + D
\]

| Parameter | Name | Geometric Effect |
|------------|------|------------------|
| \(A\) | Amplitude | Controls wave height; if \(A<0\), flips vertically |
| \(B\) | Frequency factor | Controls horizontal stretch or compression; \(T = \frac{2\pi}{B}\) |
| \(C\) | Phase shift | Shifts graph horizontally |
| \(D\) | Vertical shift | Moves graph up or down |

---

### 2. Periodicity

- \(\sin x\) and \(\cos x\): Period \(= 2\pi\)
- \(\tan x\): Period \(= \pi\)

\[
\text{Period} = \frac{2\pi}{B}
\]

---

### 3. Odd and Even Properties

| Function | Type | Verification |
|-----------|------|---------------|
| \(\sin x\) | Odd | \(\sin(-x) = -\sin x\) |
| \(\cos x\) | Even | \(\cos(-x) = \cos x\) |
| \(\tan x\) | Odd | \(\tan(-x) = -\tan x\) |

---

## ⚙️ Transformation Summary

| Parameter Change | Transformation Type | Graph Effect |
|-------------------|----------------------|---------------|
| \(|A|>1\) | Vertical stretch | Taller wave |
| \(0<|A|<1\) | Vertical shrink | Flatter wave |
| \(A<0\) | Vertical reflection | Flip over x-axis |
| \(B>1\) | Horizontal compression | Faster oscillations |
| \(0<B<1\) | Horizontal stretch | Slower oscillations |
| \(B<0\) | Horizontal reflection | Mirror along y-axis (sin flips, cos unchanged) |
| \(C>0\) | Shift right | Delay phase |
| \(C<0\) | Shift left | Advance phase |
| \(D\neq 0\) | Vertical shift | Up or down movement |

---

## 📊 Example

\[
y = -3\cos(0.5x)
\]

| Parameter | Meaning | Result |
|------------|----------|---------|
| \(A = -3\) | Amplitude = 3, flipped vertically | Peak ±3 |
| \(B = 0.5\) | Period \(T = \frac{2\pi}{0.5} = 4\pi\) | Stretched horizontally |
| \(C = 0, D = 0\) | No phase/vertical shift | Standard centered wave |

**Graph Behavior:** Starts at –3, rises to 0, peaks at +3, returns to –3 over \([0, 4\pi]\).

---

## 🧠 Conceptual Understanding

- Trigonometric functions **link triangles and waves**.  
- Changing \(A, B, C, D\) corresponds to **reshaping or timing** the wave, like adjusting amplitude and frequency in a signal.

---

## 🪐 Global Insight (Kirk’s View)

> “When you manipulate A, B, C, you’re doing what engineers and AI models do —  
> controlling amplitude, frequency, and phase.”

In signal processing and neural networks, these same transformations control how oscillations, activations, or periodic features behave.

---

## 🧩 Knowledge Threshold Summary

| Zone | Description | Example |
|------|--------------|----------|
| ✅ **Solid Knowledge** | Periodicity and side ratios understood | Correctly described cycles and wave repetition |
| ⚪ **Grey Zone** | Transformations using A, B, C parameters | Needs more visual and hands-on practice |
| ❌ **Blind Spot** | Misclassification of tangent’s symmetry | Corrected: tan is also odd |

---

### 🧭 Practice Mission

1. Start from \(y = \sin x\).  
2. Change one parameter at a time (A, then B, then C).  
3. Plot 3–5 variations and describe each transformation in words.

---

### 🪐 Crew Commentary

**Spock:** “A and B encode scaling symmetries; C and D control translation.”  
**Prof. Leonard:** “Every trig wave is just the original, stretched or shifted.”  
**Kirk:** “Master these transformations, Ensign — and the whole frequency domain will make sense to you.”

---
