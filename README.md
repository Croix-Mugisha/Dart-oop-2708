
# Dart OOP Assignment: Kigali Bus Card

**Name:** MUGISHA JEAN De La Croix

**Student ID:** 27087

## My Numbers

- D = 87
- L = 7
- Starting balance = 1870 RWF
- Bus fare = 287 RWF
- Student discount = 17%

## Output of main.dart

```text
Error: name too short
Owner: Ama | Balance: 1870 RWF
Owner: MUGISHA JEAN De La Croix | Balance: 1870 RWF
Error: top-up must be 500 to 50000 RWF
Topped up 2000 RWF
Paid 287 RWF
Paid 287 RWF
Owner: MUGISHA JEAN De La Croix | Balance: 3296 RWF
Student discount: 48 RWF
Paid 239 RWF
Owner: MUGISHA JEAN De La Croix | Balance: 1631 RWF
Student card: 17% off
```

## Part 1: Why no setter for balance?

There is no setter for balance because the balance should not be changed directly. It should only change through methods like topUp() and pay(). This helps protect the balance from incorrect values.

## Part 2: What does ~/ do?

The ~/ operator performs integer division. It returns a whole number and removes the decimal part.

For example:

- 287 * 17 / 100 = 48.79
- 287 * 17 ~/ 100 = 48

## Part 4: Bug table

| Bug | Why it is wrong | My fix |
|---|---|---|
| 1 | Non-nullable fields were not initialized. | Give the fields initial values. |
| 2 | The SmartPhone constructor did not call the parent constructor. | Use super(brand, battery). |
| 3 | The override method did not exist in the parent class. | Add restart() to Phone. |
| 4 | The battery had no setter. | Add a setter accepting values from 0 to 100. |
| 5 | The getter was called with parentheses. | Use p.battery instead of p.battery(). |

### Not a bug

The line Phone p = new Phone('Tecno', 50); is correct because using new is allowed in Dart.

## Part 5: Prediction

### My prediction

```text
1
5
```

### Real output

```text
1
5
```

### Was I right?

Yes, I was right. The first Bag has 1 item. The BigBag adds two items each time add() is called, so after two calls and adding one more item, it has 5 items.