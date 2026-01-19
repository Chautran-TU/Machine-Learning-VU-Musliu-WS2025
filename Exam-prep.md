# Perceptron, k-NN, Decision Trees (intro)

## 🧠 Perceptron 

## What it is ?
A **Perceptron** is the simplest model of a neuron.  
It decides **yes (1)** or **no (0)** based on inputs.

---

## How it works
1. Take inputs (features).  
2. Multiply each input by a weight (importance).  
3. Add them all together + bias (baseline shift).  
4. Apply a rule (step function):  
   - If result > 0 → output = 1  
   - If result ≤ 0 → output = 0  


---

# 🧠 Perceptron Example 

## Scenario
Deciding whether a student **passes** or **fails** based on two inputs:
- Exam score (x₁)  
- Homework completion (x₂)

---

## Step-by-Step
1. **Inputs**:  
   - Exam score = 80 (x₁)  
   - Homework completion = 1 (x₂, where 1 = done, 0 = not done)

2. **Weights**:  
   - Exam score weight = 0.5  
   - Homework weight = 1.0  

3. **Bias (b)**: -40 (baseline requirement)

4. **Calculation**:  
   

\[
   \text{score} = (0.5 \cdot 80) + (1.0 \cdot 1) - 40
   \]

  
   

\[
   \text{score} = 40 + 1 - 40 = 1
   \]



5. **Activation**:  
   - If score > 0 → output = 1 (Pass)  
   - If score ≤ 0 → output = 0 (Fail)

---

## Result
- Output = 1 → **Student passes**

---

## Analogy
The perceptron is like a **teacher’s grading rule**:
- Exam score matters a lot (weight 0.5).  
- Homework matters too (weight 1.0).  
- Bias sets the minimum requirement (-40).  
- If the combined score crosses the threshold → Pass, otherwise → Fail.

---

## Key Points
- ✅ Simple and fast  
- ✅ Basis of modern neural networks  
- ❌ Only works if data can be split by a straight line (linearly separable)  
