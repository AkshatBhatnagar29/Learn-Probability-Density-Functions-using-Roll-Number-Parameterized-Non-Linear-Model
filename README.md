# Learn-Probability-Density-Functions-using-Roll-Number-Parameterized-Non-Linear-Model

#  Learning about Probability Density Functions and NO₂ Data
 
Learn to estimate the parameters of a Probability Density Function (PDF) from a Non-Linear Roll-Number based NO₂ data.

###  Data set
**Air Quality Data for India from Kaggle**  
Feature used:    **Concentration of NO₂ (X)** 
 
--- 

###  Goals

1. Transform the NO₂ (X) using non-linear transformations relative to the roll number.
2. Learn the parameters of a Gaussian PDF.
3. Estimate and submit:
a.  µ (mean) 
b.  λ (lambda) 
c.  C (normalization constant) 
 
---
 
#  Step 1 - Data Transformation

Each value of **X (NO₂)** is transformed to a new value of **Z** via the following formula.

Z = X + aR sin(bR X) 

Where:
- aR = 0.05 × (R mod 7)
- bR = 0.3 × ((R mod 5) + 1)
- R = university roll number, 
- mod = remainder operation. 

This transformation produces our transformed dataset of Z. 

---
 
# 📊 Step 2 - Parameter Estimation

We can use the following equations to estimate the parameters of a PDF (Probability Distribution Function).

p̂(Z) = C.exp( -λ.( Z-µ)²) 

#### Estimated Parameters:

**Mean (µ)** = 25.80

** Variance (σ²)** = 342.59

** Lambda (λ)** = 1 / (2σ² ) = 0.001459

** Constant (C)** = 1 / √(2πσ²) = 0.0215

These equations come from the equations of the Gaussian Distribution. 

---
 
# 📈 Graphical Validation of Model

<img width="731" height="540" alt="image" src="https://github.com/user-attachments/assets/9848f47f-3ad7-46aa-b6ff-4f35ef81bf92" />


---
