### Hi there 👋

##  <a name="subtask1">Subtask 1 - Kilka zadań związanych z SQLem c.d. 👩‍💻 </a>
### <a name="kropka1"><p align="justify">11. Znajdź i zastosuj funkcję, która poprawi nazwisko Ani Muler na Miler.<p align="justify"></p></a>

```sql
UPDATE customers
SET surname = 'Miler'
WHERE customer_id = 3
```

![zadanie 11](https://user-images.githubusercontent.com/122294284/219360740-ddc3b030-31ad-40bb-9b79-0089917eadb9.png)

### <a name="kropka2"><p align="justify">12. Korzystając z funkcji join sprawdź, jak ma na imię klient i jakiego ma maila, który kupił film o id 4.</p></a>

```sql
SELECT sale.movie_id, customers.name, customers.surname, customers.email
FROM customers
JOIN sale ON customers.customer_id=sale.customer_id
WHERE sale.movie_id = 4
```

![zadanie 12](https://user-images.githubusercontent.com/122294284/219366048-41769051-2835-4459-a7f8-42c1ac6c0613.png)
