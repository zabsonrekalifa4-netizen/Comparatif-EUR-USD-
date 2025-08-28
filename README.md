<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Comparatif économique EUR vs USD</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
      margin: 0;
      padding: 20px;
    }
    h1 {
      text-align: center;
      color: #333;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 20px;
    }
    th, td {
      padding: 10px;
      text-align: center;
      border: 1px solid #ddd;
    }
    th {
      background-color: #4CAF50;
      color: white;
    }
    .arrow {
      font-size: 20px;
    }
    .up { color: green; }
    .down { color: red; }
    .neutral { color: gray; }
    .news {
      background: #fff;
      padding: 15px;
      margin: 15px 0;
      border-radius: 8px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }
    .news h2 {
      margin-top: 0;
      color: #4CAF50;
    }
    a {
      color: #1a73e8;
      text-decoration: none;
    }
  </style>
</head>
<body>

<h1>Comparatif économique EUR vs USD</h1>

<table>
  <thead>
    <tr>
      <th>Indicateur</th>
      <th>EUR</th>
      <th>USD</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>📊 Croissance du PIB</td>
      <td id="gdp-eur"></td>
      <td id="gdp-usd"></td>
    </tr>
    <tr>
      <td>👥 Taux de chômage</td>
      <td id="unemployment-eur"></td>
      <td id="unemployment-usd"></td>
    </tr>
    <tr>
      <td>📉 Inflation</td>
      <td id="inflation-eur"></td>
      <td id="inflation-usd"></td>
    </tr>
    <tr>
      <td>💱 Taux de change EUR/USD</td>
      <td id="exchange-rate"></td>
      <td></td>
    </tr>
  </tbody>
</table>

<div class="news">
  <h2>Actualités EUR 🇪🇺</h2>
  <p>Croissance économique : La zone euro a enregistré une croissance du PIB de 1,4 % au T2 2025, soutenue par l’expansion du secteur manufacturier. <a href="https://www.reuters.com/world/europe/euro-zone-business-activity-accelerates-august-new-orders-grow-pmi-shows-2025-08-21/?utm_source=chatgpt.com" target="_blank">Source</a></p>
  <p>Politique monétaire : La BCE signale une légère accélération des crédits aux ménages et entreprises. <a href="https://www.ecb.europa.eu/press/stats/md/html/ecb.md2507~b4fdc0d6f2.en.html?utm_source=chatgpt.com" target="_blank">Source</a></p>
</div>

<div class="news">
  <h2>Actualités USD 🇺🇸</h2>
  <p>Croissance économique : L’économie américaine a crû de 3,3 % au T2 2025, surpassant les prévisions. <a href="https://indiatimes.com/trending/us-economy-grows-33-in-q2-2025-beating-forecasts-can-this-rebound-hold-after-the-tariff-driven-slump-in-the-first-quarter-668217.html?utm_source=chatgpt.com" target="_blank">Source</a></p>
  <p>Politique monétaire : Le dollar est sous pression avec des attentes de baisse des taux par la Fed. <a href="https://www.reuters.com/world/middle-east/forex-dollar-defensive-september-fed-cut-bets-ramp-up-2025-08-28/?utm_source=chatgpt.com" target="_blank">Source</a></p>
</div>

<script>
  // Données économiques
  const data = {
    gdp: { eur: { value: 1.4, trend: 'up' }, usd: { value: 3.3, trend: 'up' } },
    unemployment: { eur: { value: 6.2, trend: 'down' }, usd: { value: 4.2, trend: 'down' } },
    inflation: { eur: { value: 2.0, trend: 'neutral' }, usd: { value: 2.8, trend: 'up' } },
    exchangeRate: { value: 1.1776 }
  };

  function getArrow(trend) {
    if (trend === 'up') return '<span class="arrow up">↑</span>';
    if (trend === 'down') return '<span class="arrow down">↓</span>';
    return '<span class="arrow neutral">→</span>';
  }

  document.getElementById('gdp-eur').innerHTML = `${data.gdp.eur.value}% ${getArrow(data.gdp.eur.trend)}`;
  document.getElementById('gdp-usd').innerHTML = `${data.gdp.usd.value}% ${getArrow(data.gdp.usd.trend)}`;
  document.getElementById('unemployment-eur').innerHTML = `${data.unemployment.eur.value}% ${getArrow(data.unemployment.eur.trend)}`;
  document.getElementById('unemployment-usd').innerHTML = `${data.unemployment.usd.value}% ${getArrow(data.unemployment.usd.trend)}`;
  document.getElementById('inflation-eur').innerHTML = `${data.inflation.eur.value}% ${getArrow(data.inflation.eur.trend)}`;
  document.getElementById('inflation-usd').innerHTML = `${data.inflation.usd.value}% ${getArrow(data.inflation.usd.trend)}`;
  document.getElementById('exchange-rate').innerHTML = `${data.exchangeRate.value} USD`;
</script>

</body>
</html># Comparatif-EUR-USD-
Site Comparatif économique EUR  Vs USD 
