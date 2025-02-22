# Expected Value
## Contingency Table Example

Consider the following contingency table, which represents the sales data for two products (A and B) across two stores (X and Y).

|        | Store X | Store Y | Total |
|--------|--------|--------|-------|
| Product A | 40     | 60     | 100   |
| Product B | 30     | 70     | 100   |
| **Total** | 70     | 130    | 200   |

### Step 1: Compute Expected Value Formula

The expected value for a cell is given by:

$$
E = \frac{(\text{Row Total}) \times (\text{Column Total})}{\text{Grand Total}}
$$

### Step 2: Compute Expected Value for Product A in Store X

$$
E_{A, X} = \frac{(100) \times (70)}{200} = \frac{7000}{200} = 35
$$

### Step 3: Compute Expected Value for Product A in Store Y

$$
E_{A, Y} = \frac{(100) \times (130)}{200} = \frac{13000}{200} = 65
$$

### Step 4: Compute Expected Value for Product B in Store X

$$
E_{B, X} = \frac{(100) \times (70)}{200} = 35
$$

### Step 5: Compute Expected Value for Product B in Store Y

$$
E_{B, Y} = \frac{(100) \times (130)}{200} = 65
$$

### Step 6: Expected Value Table

|        | Store X | Store Y | Total |
|--------|--------|--------|-------|
| Product A | **35**  | **65**  | 100   |
| Product B | **35**  | **65**  | 100   |
| **Total** | 70     | 130    | 200   |

These expected values can then be used in a **chi-square test** to check for independence between product sales and store location.
$$\textcolor{yellow}{\text{-----------------------------end-----------------------------}}$$
# Chi-Square Test Example

## Step 1: Contingency Table

Let's assume we have a study on whether gender affects preference for two movie genres: Action and Comedy.

|            | Action | Comedy | Total |
|------------|--------|--------|-------|
| **Male**   | 40     | 30     | 70    |
| **Female** | 20     | 50     | 70    |
| **Total**  | 60     | 80     | 140   |

## Step 2: Compute Expected Values

The expected value for each cell is calculated as:

$$
E = \frac{(\text{Row Total}) \times (\text{Column Total})}{\text{Grand Total}}
$$

- **Expected for Male (Action)**  
  $$
  E = \frac{(70) \times (60)}{140} = \frac{4200}{140} = 30
  $$

- **Expected for Male (Comedy)**  
  $$
  E = \frac{(70) \times (80)}{140} = \frac{5600}{140} = 40
  $$

- **Expected for Female (Action)**  
  $$
  E = \frac{(70) \times (60)}{140} = \frac{4200}{140} = 30
  $$

- **Expected for Female (Comedy)**  
  $$
  E = \frac{(70) \times (80)}{140} = \frac{5600}{140} = 40
  $$

|            | Action (Expected) | Comedy (Expected) | Total |
|------------|------------------|-------------------|-------|
| **Male**   | **30**           | **40**           | 70    |
| **Female** | **30**           | **40**           | 70    |

## Step 3: Compute Chi-Square Statistic

The formula for Chi-Square is:

$$
\chi^2 = \sum \frac{(O - E)^2}{E}
$$

where:
- \( O \) = observed value
- \( E \) = expected value

#### **Calculate for each cell:**
$$
\frac{(40 - 30)^2}{30} = \frac{100}{30} = 3.33
$$

$$
\frac{(30 - 40)^2}{40} = \frac{100}{40} = 2.5
$$

$$
\frac{(20 - 30)^2}{30} = \frac{100}{30} = 3.33
$$

$$
\frac{(50 - 40)^2}{40} = \frac{100}{40} = 2.5
$$

### **Step 4: Compute Final Chi-Square Value**

$$
\chi^2 = 3.33 + 2.5 + 3.33 + 2.5 = 11.66
$$

## Step 5: Degrees of Freedom (DOF)
$$
\text{DOF} = (\text{Rows} - 1) \times (\text{Columns} - 1) = (2-1) \times (2-1) = 1
$$

### **Final Answer:**
$$
\chi^2 = 11.66, \quad \text{DOF} = 1
$$
$$\textcolor{yellow}{\text{-----------------------------end-----------------------------}}$$
# Expected Frequency Calculation Using Contingency Table

Given that the total box-office collection follows a **uniform distribution** with:
- **Minimum value (a)** = 11 Million INR
- **Maximum value (b)** = 30 Million INR
- **Bins**: [11-15], [16-20], [21-25], [26-30]
- **Total number of observations (N)** = Assume **95** for this example.

### **Step 1: Contingency Table (Observed Frequencies)**
| Bins     | Observed Frequency (O) |
|----------|------------------------|
| 11 - 15  | 20                     |
| 16 - 20  | 25                     |
| 21 - 25  | 30                     |
| 26 - 30  | 20                     |
| **Total** | **95**                 |

### **Step 2: Compute Probability for Each Bin**
Since the distribution is **uniform**, each bin has an equal probability:

$$
P(\text{bin}) = \frac{\text{Bin Width}}{\text{Total Range}} = \frac{4}{19} \approx 0.2105
$$

### **Step 3: Compute Expected Frequency (E)**
The expected frequency for each bin is given by:

$$
E = N \times P(\text{bin})
$$

For **N = 95**,

$$
E = 95 \times 0.2105 = 20.00
$$

### **Step 4: Expected Frequency Table**
| Bins     | Observed Frequency (O) | Expected Frequency (E) |
|----------|------------------------|------------------------|
| 11 - 15  | 20                     | 20.00                  |
| 16 - 20  | 25                     | 20.00                  |
| 21 - 25  | 30                     | 20.00                  |
| 26 - 30  | 20                     | 20.00                  |
| **Total** | **95**                 | **95**                 |

Since the **expected frequency** is calculated as **20.00** for each bin, this is the value to use in a chi-square test if needed.

---

This table format makes it easy to compare **observed vs. expected values** and proceed with hypothesis testing.

Hope this helps! 🚀 Let me know if you need further clarification. 😊
$$\textcolor{yellow}{\text{-----------------------------end-----------------------------}}$$
# **Degrees of Freedom (DOF) Calculation for a Chi-Square Test**

## **Problem Statement**
We are testing whether the **total box-office collection** (in Million INR) on **different dates** follows a **uniform distribution** with:
- **Minimum value (a)** = 11 Million INR
- **Maximum value (b)** = 30 Million INR
- **Bins** considered for the test:
  - [11 - 15]
  - [16 - 20]
  - [21 - 25]
  - [26 - 30]

## **Step 1: Formula for Degrees of Freedom**
For a **Chi-Square Goodness-of-Fit Test**, the degrees of freedom (\( df \)) is calculated as:

$$
df = \text{(Number of bins)} - 1 - \text{(Number of estimated parameters)}
$$

## **Step 2: Identify Given Information**
- **Number of bins** = **4**
- A uniform distribution is fully defined by its **minimum and maximum values**.
- Since **minimum (11)** and **maximum (30)** are given, we **do not estimate** any parameters.
  - Thus, the **number of estimated parameters** = **0**.

## **Step 3: Compute DOF**   
$$
df = 4 - 1 - 0 = 3
$$

## **Example Contingency Table (Observed vs. Expected)**
Assume we collected box-office data for 100 different days.

| Bins      | Observed Frequency (O) | Expected Frequency (E) |
|-----------|------------------------|------------------------|
| 11 - 15   | 22                     | 25.00                 |
| 16 - 20   | 30                     | 25.00                 |
| 21 - 25   | 28                     | 25.00                 |
| 26 - 30   | 20                     | 25.00                 |
| **Total** | **100**                 | **100**                |

The **degrees of freedom for this test is 3**.

## **Final Answer:**
$$
\mathbf{df = 3}
$$

This means our chi-square test statistic will be compared to a critical value from the chi-square table with **3 degrees of freedom** at a chosen significance level (e.g., 0.05).

---

Let me know if you need any modifications! 🚀
$$\textcolor{yellow}{\text{-----------------------------end-----------------------------}}$$
# **Chi-Square Test Statistic Calculation**

## **Problem Statement**
We are testing whether the **total box-office collection** (in Million INR) on **different dates** follows a **uniform distribution** with:
- **Minimum value (a)** = 11 Million INR
- **Maximum value (b)** = 30 Million INR
- **Bins** considered for the test:
  - [11 - 15]
  - [16 - 20]
  - [21 - 25]
  - [26 - 30]
- **Total Observations (N)** = 100 (Assumed)

## **Step 1: Formula for Chi-Square Test Statistic**
The **Chi-Square test statistic** is calculated as:

$$
\chi^2 = \sum \frac{(O_i - E_i)^2}{E_i}
$$

where:
- \( O_i \) = Observed frequency for each bin
- \( E_i \) = Expected frequency for each bin

## **Step 2: Compute Expected Frequency**
Since the distribution is assumed to be **uniform**, each bin has equal probability:

$$
P_{\text{each bin}} = \frac{1}{4} = 0.25
$$

Thus, the expected frequency for each bin:

$$
E_i = 0.25 \times 100 = 25
$$

## **Step 3: Compute Chi-Square Statistic**
Assume the observed frequencies:

| Bins      | Observed Frequency (\( O_i \)) | Expected Frequency (\( E_i \)) |
|-----------|------------------------|------------------------|
| 11 - 15   | 22                     | 25                     |
| 16 - 20   | 30                     | 25                     |
| 21 - 25   | 28                     | 25                     |
| 26 - 30   | 20                     | 25                     |
| **Total** | **100**                 | **100**                |

Now, apply the Chi-Square formula:

$$
\chi^2 = \frac{(22 - 25)^2}{25} + \frac{(30 - 25)^2}{25} + \frac{(28 - 25)^2}{25} + \frac{(20 - 25)^2}{25}
$$

$$
\chi^2 = \frac{(-3)^2}{25} + \frac{(5)^2}{25} + \frac{(3)^2}{25} + \frac{(-5)^2}{25}
$$

$$
\chi^2 = \frac{9}{25} + \frac{25}{25} + \frac{9}{25} + \frac{25}{25}
$$

$$
\chi^2 = 0.36 + 1 + 0.36 + 1
$$

$$
\chi^2 = 2.72
$$

## **Final Answer:**
$$
\mathbf{\chi^2 = 2.72}
$$

This value will be compared to a critical value from the chi-square table with **degrees of freedom (df = 3)** at a chosen significance level (e.g., 0.05) to determine whether to reject the null hypothesis.

---

Let me know if you need any modifications! 🚀
$$\textcolor{yellow}{\text{-----------------------------end-----------------------------}}$$
# **Price Elasticity of Demand Calculation**

## **Problem Statement**
The **linear demand response** for product-A is modeled as a simple linear regression:

$$
D(P) = 4500 - 30P
$$

where:
- \(D(P)\) is the **demand** at price \(P\)
- We need to compute the **elasticity of demand** at **\(P = 50\)**.

## **Step 1: Formula for Price Elasticity of Demand**
The price elasticity of demand is given by:

$$
E_d = \frac{dD}{dP} \times \frac{P}{D}
$$

where:
- \( \frac{dD}{dP} \) is the derivative of the demand function with respect to price \(P\).
- \( D(P) \) is the demand at the given price \(P\).

## **Step 2: Compute $  \frac{dD}{dP}  $ **
Given:

$$
D(P) = 4500 - 30P
$$

Differentiating with respect to \(P\):

$$
\frac{dD}{dP} = -30
$$

## **Step 3: Calculate Demand at \(P = 50\)**
$$
D(50) = 4500 - 30(50)
$$

$$
D(50) = 4500 - 1500 = 3000
$$

## **Step 4: Compute Elasticity**
$$
E_d = (-30) \times \frac{50}{3000}
$$

$$
E_d = -30 \times 0.0167
$$

$$
E_d = -0.50
$$

## **Final Answer:**
$$
\mathbf{E_d = -0.50}
$$

### **Interpretation:**
- Since **\( |E_d| < 1 \)**, the demand is **inelastic** at \(P = 50\).
- This means that a 1% increase in price leads to a **less than 1%** decrease in demand.

---

Let me know if you need further clarification! 🚀
$$\textcolor{yellow}{\text{-----------------------------end-----------------------------}}$$
# **Satiating Price Calculation**

## **Problem Statement**
The **linear demand response** for product-A is modeled as:

$$
D(P) = 4500 - 30P
$$

The **satiating price** is the price at which demand becomes **zero**. That is, we solve for \( P \) when:

$$
D(P) = 0
$$

## **Step 1: Set Demand to Zero**
$$
0 = 4500 - 30P
$$

## **Step 2: Solve for \( P \)**
$$
30P = 4500
$$

$$
P = \frac{4500}{30} = 150
$$

## **Final Answer:**
$$
\mathbf{P = 150}
$$

### **Interpretation:**
- The **satiating price** is **Rs. 150**.
- At **\( P = 150 \)**, demand becomes **zero**, meaning no one is willing to purchase the product at this price.

---

Let me know if you need any modifications! 🚀



# **Market Size Calculation**

## **Problem Statement**
The **linear demand response** for product-A is modeled as:

$$
D(P) = 4500 - 30P
$$

The **market size** refers to the **maximum possible demand**, which occurs when the price is **zero** (\( P = 0 \)).

## **Step 1: Compute Demand at \( P = 0 \)**
$$
D(0) = 4500 - 30(0)
$$

$$
D(0) = 4500
$$

## **Final Answer:**
$$
\mathbf{Market \ Size = 4500 \ \text{units}}
$$

### **Interpretation:**
- The **market size** is **4500 units**.
- This means that if the product were **free** (\( P = 0 \)), the **maximum possible demand** would be **4500 units**.

---

Let me know if you need any modifications! 🚀
$$\textcolor{yellow}{\text{-----------------------------end-----------------------------}}$$



## Contingency Table for Student Visa Applications

To determine the best application center for applying for a student visa, we analyze the probability of applying through each center and the probability of being granted a visa.

### Given Data:
- **Application Probability (\(P(X)\))**:
  - \( P(A) = 0.15 \) (15%)
  - \( P(B) = 0.10 \) (10%)
  - \( P(C) = 0.25 \) (25%)
  - \( P(D) = 0.25 \) (25%)
  - \( P(E) = 0.25 \) (25%)

- **Visa Grant Probability (\(P(G|X)\))**:
  - \( P(G|A) = 0.60 \), so \( P(\neg G|A) = 0.40 \)
  - \( P(G|B) = 0.80 \), so \( P(\neg G|B) = 0.20 \)
  - \( P(G|C) = 0.50 \), so \( P(\neg G|C) = 0.50 \)
  - \( P(G|D) = 0.50 \), so \( P(\neg G|D) = 0.50 \)
  - \( P(G|E) = 0.50 \), so \( P(\neg G|E) = 0.50 \)

### Contingency Table:
| Application Centre | Probability of Applying (P) | Granted ($P(G/X) \times P(X)$) | Not Granted ( $P(\neg G/X) \times P(X)$) |
|-------------------|----------------------------|----------------------------------|------------------------------------|
| A               | 0.15                         | $0.15 \times 0.60 = 0.09$    | $0.15 \times 0.40 = 0.06$      |
| B               | 0.10                         | $0.10 \times 0.80 = 0.08$    | $0.10 \times 0.20 = 0.02$      |
| C               | 0.25                         | $0.25 \times 0.50 = 0.125$   | $0.25 \times 0.50 = 0.125$    |
| D               | 0.25                         | $0.25 \times 0.50 = 0.125$   | $0.25 \times 0.50 = 0.125$    |
| E               | 0.25                         | $0.25 \times 0.50 = 0.125$   | $0.25 \times 0.50 = 0.125$    |
| **Total**       | **1.00**                     | **0.555**                      | **0.445**                        |

### Explanation:
1. Each row represents an application center (A, B, C, D, E).
2. The **Probability of Applying** column (\( P(X) \)) shows the percentage of total applications coming from each center.
3. The **Granted** column calculates the probability of getting a visa, given that an applicant applies from a particular center:
   $$
   P(G \cap X) = P(G|X) \times P(X)
   $$
4. The **Not Granted** column calculates the probability of not getting a visa from a given center:
   $$
   P(\neg G \cap X) = P(\neg G|X) \times P(X)
   $$
5. The **Total row** confirms that the sum of all probabilities is consistent:
   - **Total Probability of Getting a Visa**: **0.555**
   - **Total Probability of Not Getting a Visa**: **0.445**
   - **Total Applications**: **1.00** (100%)

### Conclusion:
- The highest chance of getting a visa is from **center B (80% acceptance rate)**, even though it only handles 10% of applications.
- The lowest chance is from **center A (60% acceptance rate)**, which only handles 15% of applications.
- Centers C, D, and E have an equal **50-50** probability of granting a visa.

This table helps in deciding which center to apply through for a higher chance of visa approval.


## Expected Number of Granted Applications from Centres C, D, and E

We are given that **500 applications** have been granted a visa. We need to determine how many of these applications came from centres **C, D, and E combined**.

### Step 1: Find the Probability of a Granted Visa from Centres C, D, and E
From the contingency table, the total probability of getting a visa from these three centres is:

$$
P(G \cap C) + P(G \cap D) + P(G \cap E) = 0.125 + 0.125 + 0.125 = 0.375
$$

### Step 2: Calculate the Expected Number of Applications from C, D, and E
Since the total number of granted visas is **500**, the expected number from these three centres is:

$$
500 \times 0.375 = 187.5
$$

Since the number of applications must be a whole number, we can approximate this to **188 applications**.

### Final Answer:
Thus, the expected number of granted applications from **centres C, D, and E combined** is **188**.

$$\textcolor{yellow}{\text{-----------------------------end-----------------------------}}$$
## Probability that Dr. MS Applied Through Centre C Given the Visa Was Not Granted

We are given that Dr. MS's application **was not granted**, and we need to find the probability that Dr. MS applied through **centre C**.

### Step 1: Use Bayes’ Theorem
We need to compute:

$$
P(C | \neg G)
$$

Using Bayes' theorem:

$$
P(C | \neg G) = \frac{P(\neg G \cap C)}{P(\neg G)}
$$

where:
- \( P(\neg G \cap C) \) is the probability of applying through **centre C** and not getting a visa.
- \( P(\neg G) \) is the total probability of **not getting a visa**.

### Step 2: Use Values from the Contingency Table
From our contingency table:

$$
P(\neg G \cap C) = P(C) \times P(\neg G | C) = 0.25 \times 0.50 = 0.125
$$

Total probability of not getting a visa:

$$
P(\neg G) = P(\neg G \cap A) + P(\neg G \cap B) + P(\neg G \cap C) + P(\neg G \cap D) + P(\neg G \cap E)
$$

$$
= 0.06 + 0.02 + 0.125 + 0.125 + 0.125 = 0.445
$$

### Step 3: Compute the Probability
$$
P(C | \neg G) = \frac{0.125}{0.445} = 0.28
$$

### Final Answer:
The probability that Dr. MS applied through **centre C**, given that the visa was **not granted**, is **0.28** (or **28%**). 🚀
