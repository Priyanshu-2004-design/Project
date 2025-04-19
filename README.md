# Project
This project is about the website(Transaction) which i have been given to modify

Html code

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Expense Tracker</title>
  <link rel="stylesheet" href="style.css"/>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
</head>
<body>
  <div class="container">
    <h1>Expense Tracker</h1>
    <div class="balance">
      <p>Balance</p>
      <h2>€432.00</h2>
    </div>
    <div class="summary">
      <div class="income">
        <p>Income</p>
        <span>+950</span>
      </div>
      <div class="expense">
        <p>Expense</p>
        <span>−558</span>
      </div>
    </div>

    <div class="transaction-section">
      <div class="add-transaction">
        <h3>Add New Transaction</h3>
        <input type="text" placeholder="Text" />
        <input type="number" placeholder="Amount" />
        <p class="hint">(negative - expense, positive - income)</p>
        <button class="add-btn">Add Transaction</button>
        <button class="delete-btn">DELETE</button>
      </div>

      <div class="history">
        <h3>History</h3>
        <ul>
          <li>
            <span class="icon income-icon"><i class="fas fa-euro-sign"></i></span>
            <span class="text">Cash</span>
            <span class="amount income">+500</span>
          </li>
          <li>
            <span class="icon expense-icon"><i class="fas fa-cart-shopping"></i></span>
            <span class="text">Groceries</span>
            <span class="amount expense">−25</span>
          </li>
          <li>
            <span class="icon expense-icon"><i class="fas fa-bag-shopping"></i></span>
            <span class="text">Rent</span>
            <span class="amount expense">−500</span>
          </li>
          <li>
            <span class="icon income-icon"><i class="fas fa-euro-sign"></i></span>
            <span class="text">Salary</span>
            <span class="amount income">+950</span>
          </li>
        </ul>
      </div>
    </div>
  </div>
</body>
</html> 


CSS Code

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: #062020;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #fff;
  display: flex;
  justify-content: center;
  padding: 30px;
}

.container {
  background-color: #0c2c2c;
  border-radius: 16px;
  padding: 40px;
  width: 360px;
  box-shadow: 0 0 20px rgba(0, 255, 191, 0.05);
}

h1 {
  text-align: center;
  margin-bottom: 30px;
}

.balance {
  background: radial-gradient(circle, #0a3838 40%, #061c1c);
  padding: 20px;
  border-radius: 50%;
  width: 180px;
  height: 180px;
  margin: auto;
  text-align: center;
}

.balance p {
  color: #57d3ba;
  font-size: 16px;
}

.balance h2 {
  font-size: 32px;
  margin-top: 10px;
}

.summary {
  display: flex;
  justify-content: space-around;
  margin: 25px 0;
}

.income p,
.expense p {
  font-size: 14px;
  margin-bottom: 5px;
}

.income span {
  color: #57d3ba;
  font-weight: bold;
}

.expense span {
  color: #ff5a5a;
  font-weight: bold;
}

.transaction-section {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  margin-top: 20px;
}

.add-transaction,
.history {
  flex: 1;
}

.add-transaction input {
  width: 100%;
  padding: 8px;
  margin-top: 10px;
  border: none;
  border-radius: 6px;
  background: #103636;
  color: #fff;
}

.hint {
  font-size: 11px;
  margin: 5px 0;
  color: #888;
}

.add-btn {
  width: 100%;
  background-color: #57d3ba;
  padding: 10px;
  margin-top: 10px;
  border: none;
  border-radius: 8px;
  font-weight: bold;
  color: #062020;
  cursor: pointer;
}

.delete-btn {
  width: 100%;
  background-color: #ff5a5a;
  padding: 10px;
  margin-top: 10px;
  border: none;
  border-radius: 8px;
  font-weight: bold;
  cursor: pointer;
}

.history ul {
  list-style: none;
  margin-top: 10px;
}

.history li {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: #103636;
  padding: 10px;
  border-radius: 8px;
  margin-bottom: 10px;
}

.icon {
  margin-right: 10px;
  font-size: 16px;
}

.income-icon {
  color: #57d3ba;
}

.expense-icon {
  color: #ff5a5a;
}

.text {
  flex: 1;
}

.amount {
  font-weight: bold;
}

.amount.income {
  color: #57d3ba;
}

.amount.expense {
  color: #ff5a5a;
}
