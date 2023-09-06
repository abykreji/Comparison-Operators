#### EXERCISE:
##### How many female customers do we have from the state of Oregon (OR)?

```python
SELECT COUNT(firstName)
FROM customers
WHERE gender = 'F' and state = 'OR';
```

##### Who over the age of 44 has an income of 100 000 or more? (excluding 44)

```python
SELECT COUNT(income)
FROM customers
WHERE age > 44 and income >= 100000;
```

##### Who between the ages of 30 and 50 has an income less than 50 000?


```python
SELECT COUNT(income)
FROM customers
WHERE age >= 30 and age <= 50 AND income < 50000;
```

##### What is the average income between the ages of 20 and 50? 

```python
SELECT AVG(income)
FROM customers
WHERE age > 20 and age < 50;
```