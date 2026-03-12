# SQL Mastery Practice Set (Backend Interview Level)

A single structured problem set is the best way to check whether the concepts actually stuck.

This set covers everything you learned so far:

- GROUP BY
- HAVING
- Subqueries
- CTE
- Window functions
- ROW_NUMBER / RANK / DENSE_RANK
- LAG / LEAD
- Row comparisons
- Time-series logic

⚠️ Do not rush. Solve them properly.

---

# Table 1 — Orders

| order_id | user_id | amount | order_date |
|--------|--------|--------|-----------|
| 1 | 101 | 500 | 2024-01-01 |
| 2 | 101 | 400 | 2024-01-02 |
| 3 | 101 | 300 | 2024-01-03 |
| 4 | 102 | 700 | 2024-01-01 |
| 5 | 102 | 700 | 2024-01-02 |
| 6 | 102 | 600 | 2024-01-03 |
| 7 | 103 | 200 | 2024-01-01 |
| 8 | 103 | 300 | 2024-01-02 |
| 9 | 104 | 900 | 2024-01-01 |

---

# Section 1 — Aggregation

## Q1
Find total order amount per user.

---

## Q2
Find users whose **total spending > 1000**.

---

## Q3
Find users whose **total spending is above average spending across users**.

Hint: aggregation + subquery

---

## Q4
Return the **user who spent the most**.

---

# Section 2 — CTE

## Q5
Using a **CTE**, return users whose **total spending is above average user spending**.

---

# Section 3 — Window Functions (Ranking)

## Q6
Assign **ROW_NUMBER per user ordered by amount descending**.

Output:


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

