<!DOCTYPE html>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Budget Tracker</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

```
<!-- Page Heading -->
<h1>My Budget Tracker</h1>

<!-- Add Expense Form -->
<form>
    <h2>Add Expense</h2>

    <label for="expense-name">Expense Name:</label>
    <input 
        type="text" 
        id="expense-name" 
        name="expense-name"
        placeholder="Enter expense name"
    >

    <label for="amount">Amount:</label>
    <input 
        type="number" 
        id="amount" 
        name="amount"
        placeholder="Enter amount"
    >

    <label for="category">Category:</label>
    <select id="category" name="category">
        <option value="">Select category</option>
        <option value="food">Food</option>
        <option value="transport">Transport</option>
        <option value="school">School</option>
        <option value="shopping">Shopping</option>
        <option value="other">Other</option>
    </select>

    <button type="submit">Add Expense</button>
</form>

<!-- Expense Table -->
<table>
    <thead>
        <tr>
            <th>Expense Name</th>
            <th>Amount</th>
            <th>Category</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td>Bus Fair</td>
            <td>KSh 100</td>
            <td>Transport</td>
        </tr>

        <tr>
            <td>Lunch</td>
            <td>KSh 250</td>
            <td>Food</td>
        </tr>

        <tr>
            <td>School Books</td>
            <td>KSh 500</td>
            <td>School</td>
        </tr>

        <tr>
            <td>Shopping</td>
            <td>KSh 800</td>
            <td>Shopping</td>
        </tr>

        <tr>
            <td>Mobile Data</td>
            <td>KSh 200</td>
            <td>Other</td>
        </tr>
    </tbody>
</table>

<!-- Budgeting Tips -->
<section class="budgeting-tips">

    <h2>Budgeting Tips</h2>

    <img 
        class="budget-icon"
        src="https://cdn-icons-png.flaticon.com/512/3135/3135706.png"
        alt="Budgeting and money icon"
    >

    <p>
        Learn simple and practical ways to manage your money,
        control your spending, and build better financial habits.
    </p>

    <div class="video-container">
        <iframe
            src="https://www.youtube.com/embed/-xdDTCQObGo"
            title="Budgeting Tips"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen>
        </iframe>
    </div>

</section>
```

</body>
</html>
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: linear-gradient(135deg, #f1f7f2 0%, #e8f3ff 100%);
    color: #1f2937;
    line-height: 1.6;
    padding: 40px 20px;
}

h1 {
    text-align: center;
    color: #0f172a;
    font-size: 2.5rem;
    margin-bottom: 30px;
    font-weight: 700;
    letter-spacing: 1px;
}

form {
    max-width: 550px;
    margin: 0 auto 30px;
    background: #ffffff;
    border: 1px solid #dfe7ee;
    border-radius: 18px;
    padding: 25px 22px;
    box-shadow: 0 12px 30px rgba(15, 23, 42, 0.08);
}

form h2 {
    text-align: center;
    font-size: 1.6rem;
    margin-bottom: 20px;
    color: #0f766e;
}

label {
    display: block;
    font-weight: 600;
    margin-bottom: 8px;
    color: #334155;
}

input,
select,
button {
    width: 100%;
    border-radius: 10px;
    font: inherit;
}

input,
select {
    padding: 12px 14px;
    margin-bottom: 18px;
    border: 1px solid #cbd5e1;
    background: #f8fafc;
    transition: border-color 0.2s ease, box-shadow 0.2s ease;
}

input:focus,
select:focus {
    outline: none;
    border-color: #14b8a6;
    box-shadow: 0 0 0 3px rgba(20, 184, 166, 0.15);
}

button {
    border: none;
    background: linear-gradient(135deg, #14b8a6, #0ea5e9);
    color: white;
    font-weight: 700;
    cursor: pointer;
    padding: 14px 18px;
    box-shadow: 0 10px 20px rgba(14, 165, 233, 0.25);
    transition: transform 0.2s ease, box-shadow 0.2s ease;
}

button:hover {
    transform: translateY(-1px);
    box-shadow: 0 14px 24px rgba(14, 165, 233, 0.3);
}

button:active {
    transform: translateY(0);
}

table {
    width: min(900px, 100%);
    margin: 0 auto 35px;
    border-collapse: collapse;
    background: #fff;
    border-radius: 18px;
    overflow: hidden;
    box-shadow: 0 10px 28px rgba(15, 23, 42, 0.07);
}

thead {
    background: #0f172a;
    color: white;
}

th,
td {
    text-align: left;
    padding: 16px 18px;
    border-bottom: 1px solid #e2e8f0;
}

th {
    font-size: 0.95rem;
    letter-spacing: 0.04em;
    text-transform: uppercase;
}

tbody tr:nth-child(even) {
    background: #f8fafc;
}

tbody tr:hover {
    background: #ecfeff;
}

.budgeting-tips {
    max-width: 900px;
    margin: 0 auto;
    background: #ffffff;
    border-radius: 18px;
    padding: 28px 24px;
    box-shadow: 0 10px 28px rgba(15, 23, 42, 0.08);
    text-align: center;
}

.budgeting-tips h2 {
    color: #0f172a;
    margin-bottom: 18px;
    font-size: 1.9rem;
}

.budget-icon {
    display: block;
    width: 90px;
    margin: 0 auto 18px;
    filter: drop-shadow(0 10px 15px rgba(14, 165, 233, 0.18));
}

.budgeting-tips p {
    max-width: 680px;
    margin: 0 auto 25px;
    color: #475569;
    font-size: 1.02rem;
}

.video-container {
    position: relative;
    width: 100%;
    max-width: 720px;
    margin: 0 auto;
    aspect-ratio: 16 / 9;
    border-radius: 14px;
    overflow: hidden;
    box-shadow: 0 10px 25px rgba(15, 23, 42, 0.12);
}

.video-container iframe {
    width: 100%;
    height: 100%;
    border: none;
}

@media (max-width: 640px) {
    body {
        padding: 24px 14px;
    }

    h1 {
        font-size: 2rem;
    }

    form {
        padding: 20px 16px;
    }

    th,
    td {
        padding: 12px 10px;
        font-size: 0.92rem;
    }

    .budgeting-tips {
        padding: 22px 14px;
    }
}
