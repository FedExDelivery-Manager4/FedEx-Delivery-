<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>FedEx Delivery - Ghana (+233)</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #fefefe;
      color: #ccc;
    }
  h1{
    color: #4d148c;
    font-size: 26px
  }
  
    h6 {
      color: white;
      border: 1px solid #ff6600;
      padding: 5px;
      display: inline-block;
    }

    header {
      background-color: #b76e79;
      color: white;
      padding: 20px;
      text-align: center;
      position: relative;
    }

    .transaction-btn {
      position: absolute;
      right: 20px;
      top: 20px;
      padding: 10px 16px;
      background-color: #ffa500;
      color: white;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      font-weight: bold;
    }

    .container {
      max-width: 800px;
      margin: 30px auto;
      background: #fff;
      border: 1px solid #ccc;
      border-radius: 8px;
      overflow: hidden;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    .section {
      padding: 20px;
      border-bottom: 1px solid #ddd;
    }

    .section h2 {
      margin-top: 0;
      color: #ffA500;
    }

    .field-group {
      display: flex;
      justify-content: space-between;
      margin-bottom: 12px;
    }

    .field-group div {
      flex: 1;
      margin-right: 10px;
    }

    .field-group div:last-child {
      margin-right: 0;
    }

    .readonly-box {
      background-color: #f9f9f9;
      border: 1px solid #ccc;
      padding: 10px;
      border-radius: 4px;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 20px;
    }

    table thead {
      background-color: #ffa500;
      color: white;
    }

    table, th, td {
      border: 1px solid #ddd;
    }

    th, td {
      padding: 10px;
      text-align: center;
    }

    .total-box {
      background-color: #b76e79;
      color: white;
      font-size: 1.5em;
      text-align: center;
      padding: 20px;
      margin-top: 30px;
      border-radius: 0 0 8px 8px;
    }

    .footer {
      text-align: center;
      font-size: 12px;
      padding: 10px;
      color: #666;
    }

    #transactionList {
      display: none;
      margin: 30px auto;
      max-width: 800px;
      background: #fefefe;
      border: 1px solid #ccc;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.05);
      padding: 20px;
    }

    #transactionList h3 {
      color: #b76e79;
    }

    .transaction-entry {
      border-bottom: 1px solid #ddd;
      padding: 10px 0;
    }
  </style>
</head>
<body>

  <header>
    <h1>FedEx Delivery</h1>
    <h3>Ghana (+233)</h3>
    <br>
    <h6>Home -> International Delivery ->  Customer Page </h6>
    <button class="transaction-btn" onclick="toggleTransactions()">Transactions</button>
  </header>

  <!-- Transaction List Section -->
  <div id="transactionList">
    <h3>Recent Transactions</h3>
    <div class="transaction-entry">
      <strong>ID:</strong> TXN001 <br>
      <strong>Date:</strong> 2025-06-10 <br>
      <strong>Amount:</strong> GHS 2240 <br>
      <strong>Status:</strong> Delivered
    </div>
    <div class="transaction-entry">
      <strong>ID:</strong> TXN002 <br>
      <strong>Date:</strong> 2025-06-12 <br>
      <strong>Amount:</strong> GHS 1550 <br>
      <strong>Status:</strong> In Transit
    </div>
  </div>

  <div class="container">
    <div class="section">
      <h2>Sender Details</h2>
      <div class="field-group">
        <div>
          <label>Full Name</label>
          <div class="readonly-box">John Doe</div>
        </div>
        <div>
          <label>Phone Number</label>
          <div class="readonly-box">+233 24 000 0000</div>
        </div>
      </div>
      <div class="field-group">
        <div>
          <label>Location</label>
          <div class="readonly-box">Accra, Ghana</div>
        </div>
        <div>
          <label>Email</label>
          <div class="readonly-box">john@example.com</div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>Recipient Details</h2>
      <div class="field-group">
        <div>
          <label>Full Name</label>
          <div class="readonly-box">Ama Serwaa</div>
        </div>
        <div>
          <label>Phone Number</label>
          <div class="readonly-box">+233 20 000 0001</div>
        </div>
      </div>
      <div class="field-group">
        <div>
          <label>Location</label>
          <div class="readonly-box">Kumasi, Ghana</div>
        </div>
        <div>
          <label>Email</label>
          <div class="readonly-box">ama@example.com</div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>Package Summary</h2>
      <table>
        <thead>
          <tr>
            <th>No:</th>
            <th>Quantity</th>
            <th>Description</th>
            <th>Amount (GHS)
