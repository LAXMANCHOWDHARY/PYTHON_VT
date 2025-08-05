<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Power BI End-to-End Project</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 40px;
      max-width: 900px;
      background-color: #f9f9f9;
      color: #333;
    }
    h1, h2, h3 {
      color: #2e6c80;
    }
    pre {
      background: #f4f4f4;
      padding: 10px;
      border-left: 5px solid #ccc;
      overflow-x: auto;
    }
    code {
      background: #eee;
      padding: 2px 4px;
      font-family: Consolas, monospace;
    }
    a {
      color: #0366d6;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    ul {
      padding-left: 20px;
    }
    .badge {
      background-color: #0366d6;
      color: white;
      padding: 3px 8px;
      font-size: 12px;
      border-radius: 4px;
      margin-right: 5px;
    }
  </style>
</head>
<body>

  <h1>📊 Power BI End-to-End Project</h1>

  <p><strong>Author:</strong> Your Name<br>
  <strong>Last Updated:</strong> August 2025</p>

  <p>This repository contains a complete, end-to-end Power BI project—from raw data ingestion to final dashboards. It includes data cleaning, modeling, DAX measures, and interactive report creation using Power BI Desktop.</p>

  <h2>📌 Project Overview</h2>
  <p>The goal of this project is to build a fully functional Power BI dashboard using real-world data. It covers:</p>
  <ul>
    <li>Data sourcing</li>
    <li>Data cleaning and transformation (Power Query)</li>
    <li>Data modeling (relationships, star schema)</li>
    <li>DAX measures and KPIs</li>
    <li>Visualization and report building</li>
    <li>Deployment and sharing options</li>
  </ul>

  <h2>🛠️ Prerequisites</h2>
  <ul>
    <li><a href="https://powerbi.microsoft.com/desktop/">Power BI Desktop</a> installed</li>
    <li>Basic understanding of DAX and Power Query (M language)</li>
    <li>Data source (CSV, Excel, SQL Server, etc.)</li>
  </ul>



  <h2>📈 Features</h2>
  <ul>
    <li>Dynamic visuals with filters and slicers</li>
    <li>Custom DAX measures: YTD, MTD, YoY</li>
    <li>Drillthrough, bookmarks, and tooltips</li>
    <li>Well-structured data model using best practices</li>
  </ul>

  <h2>⚙️ Setup Instructions</h2>
  <ol>
    <li>Clone this repository:</li>
    <pre><code>git clone https://github.com/yourusername/powerbi-end-to-end.git</code></pre>

    <li>Open <code>FinalDashboard.pbix</code> in Power BI Desktop</li>
    <li>Ensure the data source path is correct (you may need to update it in Power Query)</li>
    <li>Refresh the data and explore the report</li>
  </ol>

  <h2>🧮 Key DAX Measures</h2>
  <pre><code>Sales YTD = TOTALYTD(SUM(Sales[Revenue]), 'Date'[Date])
Sales MTD = TOTALMTD(SUM(Sales[Revenue]), 'Date'[Date])
YoY Growth = 
VAR ThisYear = CALCULATE(SUM(Sales[Revenue]), 'Date'[Year] = YEAR(TODAY()))
VAR LastYear = CALCULATE(SUM(Sales[Revenue]), 'Date'[Year] = YEAR(TODAY()) - 1)
RETURN DIVIDE(ThisYear - LastYear, LastYear)</code></pre>

  <h2>🖼️ Screenshots</h2>
  <p>Dashboard preview:</p>
  <img src="Images/dashboard_screenshot.png" alt="Dashboard Screenshot" width="800"/>

  <h2>🚀 Deployment Options</h2>
  <ul>
    <li>Publish to <a href="https://app.powerbi.com/">Power BI Service</a></li>
    <li>Share with workspace members or via public embed (if allowed)</li>
    <li>Schedule refresh for data sources like SQL or Excel on OneDrive</li>
  </ul>

  <h2>📚 Learning Resources</h2>
  <ul>
    <li><a href="https://docs.microsoft.com/en-us/power-bi/">Power BI Documentation</a></li>
    <li><a href="https://www.sqlbi.com/">SQLBI - DAX and Data Modeling</a></li>
    <li><a href="https://www.youtube.com/user/GuyInACube">Guy in a Cube (YouTube)</a></li>
  </ul>

  <h2>📄 License</h2>
  <p>This project is licensed under the <strong>MIT License</strong>. You are free to use, modify, and distribute it with attribution.</p>

  <h2>🙌 Contributing</h2>
  <p>Feel free to open issues or submit pull requests if you'd like to improve this project. All contributions are welcome!</p>

  <h2>📫 Contact</h2>
  <p>If you have any questions, feel free to reach out via GitHub or email: <code>youremail@example.com</code></p>

  <hr>
  <p align="center">⭐️ Star this repo if you find it helpful!</p>

</body>
</html>
