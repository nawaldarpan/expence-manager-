<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Daily Expense Manager</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header class="header">
    <h1>Daily Expense Manager</h1>
  </header>

  <main class="container">
    <!-- Add Expense Section -->
    <section class="card">
      <h2>Add Expense</h2>
      <div class="form-group">
        <label for="description">Description</label>
        <input type="text" id="description" placeholder="Enter description">
      </div>
      <div class="form-group">
        <label for="amount">Amount</label>
        <input type="number" id="amount" placeholder="Enter amount" step="0.01">
      </div>
      <div class="form-group">
        <label for="category">Category</label>
        <select id="category">
          <option value="">Select category</option>
          <option value="food">Food</option>
          <option value="transport">Transport</option>
          <option value="entertainment">Entertainment</option>
          <option value="shopping">Shopping</option>
          <option value="other">Other</option>
        </select>
      </div>
      <button id="add-expense-btn">Add Expense</button>
    </section>

    <!-- Expenses List Section -->
    <section class="card">
      <h2>Expenses</h2>
      <div id="expenses-list">
        <p class="no-expenses">No expenses added yet.</p>
      </div>
    </section>

    <!-- Total Balance Section -->
    <section class="card">
      <h2>Total Balance</h2>
      <div class="total-balance">
        <p>Total: <span id="total-balance">$0.00</span></p>
      </div>
    </section>
  </main>

  <footer class="footer">
    <p>&copy; 2023 Daily Expense Manager. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
