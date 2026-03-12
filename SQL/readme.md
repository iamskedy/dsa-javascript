order_id
user_id
amount
row_number


---

## Q7
Return **highest order per user**.

Hint: `ROW_NUMBER`

---

## Q8
Return **highest order per user including ties**.

Hint: `RANK`

---

## Q9
Return **Top 2 orders per user**.

---

# Section 4 — Row Comparison

## Q10
Using `LAG()`, show:


order_id
user_id
amount
previous_amount


---

## Q11
Return rows where **amount increased compared to previous order of that user**.

---

# Section 5 — Time Series Logic

Table:

| day | sales |
|----|------|
| 1 | 100 |
| 2 | 150 |
| 3 | 120 |
| 4 | 200 |
| 5 | 180 |
| 6 | 220 |

---

## Q12
Return rows where **sales increased compared to previous day**.

---

## Q13
Return rows where **sales decreased compared to previous day**.

---

## Q14
Return **local peaks**.

Condition:


sales > previous_sales
AND
sales > next_sales


Hint: `LAG + LEAD`

---

## Q15
Show:


day
sales
previous_sales
next_sales


---

# Section 6 — Harder Window Problem

## Q16
Find the **second highest order per user**.

---

# Submission Format

Reply like this:


Q1:
<SQL>

Q2:
<SQL>

...

Q16:
<SQL>


---

# Evaluation

Your queries will be:

- Reviewed
- Corrected if needed
- Scored for mastery
- Weak areas will be identified

---

# Why This Set Is Important

If you can solve these **without help**, you have mastered:

- aggregation logic
- window functions
- row comparison
- ranking patterns

These are **core SQL concepts for backend interviews**.

---
