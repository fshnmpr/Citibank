<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Banking Demo - Login</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="login-container">
    <h2>Login to Your Account</h2>
    <form action="dashboard.html" method="GET">
      <div class="form-group">
        <label for="username">Username:</label>
        <input type="text" id="username" name="username" required>
      </div>
      <div class="form-group">
        <label for="password">Password:</label>
        <input type="password" id="password" name="password" required>
      </div>
      <button type="submit">Login</button>
    </form>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Banking Demo - Dashboard</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="dashboard-container">
    <h1>Welcome, [Username]</h1>
    <h2>Account Balance: $100,000,000</h2>

    <div class="transactions">
      <h3>Recent Transactions</h3>
      <table>
        <thead>
          <tr>
            <th>Date</th>
            <th>Description</th>
            <th>Amount</th>
            <th>Balance</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>2024-09-01</td>
            <td>Transfer to Savings</td>
            <td>- $10,000</td>
            <td>$99,990,000</td>
          </tr>
          <tr>
            <td>2024-08-30</td>
            <td>Salary Deposit</td>
            <td>+ $20,000</td>
            <td>$100,000,000</td>
          </tr>
        </tbody>
      </table>
    </div>
    <a href="transactions.html">View Full Transaction History</a>
  </div>
</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Banking Demo - Transaction History</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="transactions-history-container">
    <h1>Transaction History</h1>
    <table>
      <thead>
        <tr>
          <th>Date</th>
          <th>Description</th>
          <th>Amount</th>
          <th>Balance</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>2024-09-01</td>
          <td>Transfer to Savings</td>
          <td>- $10,000</td>
          <td>$99,990,000</td>
        </tr>
        <tr>
          <td>2024-08-30</td>
          <td>Salary Deposit</td>
          <td>+ $20,000</td>
          <td>$100,000,000</td>
        </tr>
        <!-- Add more rows for a more detailed history -->
      </tbody>
    </table>
  </div>
</body>
</html>
/* General Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, sans-serif;
}

/* Login Page */
.login-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background-color: #f5f5f5;
}

h2 {
  margin-bottom: 20px;
}

.form-group {
  margin-bottom: 15px;
}

input {
  width: 100%;
  padding: 10px;
  margin: 5px 0;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button {
  padding: 10px 20px;
  background-color: #007bff;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

button:hover {
  background-color: #0056b3;
}

/* Dashboard & Transaction Pages */
.dashboard-container,
.transactions-history-container {
  margin: 50px auto;
  width: 80%;
}

h1, h2, h3 {
  margin-bottom: 20px;
}

table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 20px;
}

table, th, td {
  border: 1px solid #ccc;
}

th, td {
  padding: 15px;
  text-align: left;
}

th {
  background-color: #f8f8f8;
}
