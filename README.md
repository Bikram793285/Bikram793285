/* Question 1 : Return the customer IDs of customers who have spent at least $110 with the staff member who has an ID of 2. */

SELECT customer_id, SUM(amount) FROM PAYMENT
WHERE staff_id =2
HAVING SUM(amount) >= 110
ORDER BY customer_id

