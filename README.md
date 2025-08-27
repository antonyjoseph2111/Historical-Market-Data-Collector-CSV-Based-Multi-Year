<h1 align="center">📊 Historical Market Data Collector (CSV-Based, Multi-Year)</h1>

<p align="center">
  <em>Lightweight Python tool to fetch and merge multi-year OHLCV cryptocurrency data directly into clean CSV files.</em>
</p>

<hr />

<h2>🚀 Overview</h2>
<p>
This project is a <strong>historical market data collector</strong> built in Python.  
It downloads OHLCV (Open, High, Low, Close, Volume) data across <strong>multiple years</strong> for crypto pairs 
like <code>BTC/USDT</code> or <code>ETH/USDT</code> from public archives and merges them into one 
well-structured CSV file for easy analysis, backtesting, or research.
</p>

<ul>
  <li>✅ No API keys required – avoids rate-limit issues.</li>
  <li>✅ Multi-timeframe support: daily, hourly, and minute data.</li>
  <li>✅ Data automatically merged into a single CSV.</li>
  <li>✅ Beginner-friendly and minimal dependencies.</li>
</ul>

<hr />

<h2>🛠️ Tech Stack</h2>
<ul>
  <li>Python 3.x</li>
  <li><code>pandas</code> for data manipulation</li>
  <li><code>requests</code> for downloading data</li>
  <li>Jupyter Notebook for demo & experimentation</li>
</ul>

<hr />

<h2>📂 Project Structure</h2>
<pre>
├── data/                # Folder for downloaded CSVs
├── main.ipynb           # Jupyter notebook (demo + workflow)
├── collector.py         # (Optional) Script version for CLI usage
├── README.html          # Project documentation
</pre>

<hr />

<h2>⚡ Usage</h2>

<h3>1. Clone the repository</h3>
<pre>
git clone https://github.com/antonyjoseph2111/Historical-Market-Data-Collector-CSV-Based-Multi-Year.git
cd Historical-Market-Data-Collector-CSV-Based-Multi-Year
</pre>

<h3>2. Install dependencies</h3>
<pre>
pip install -r requirements.txt
</pre>

<h3>3. Run the notebook</h3>
<pre>
jupyter notebook main.ipynb
</pre>

<h3>4. Example Output</h3>
<p>A merged CSV with clean OHLCV data:</p>

<pre>
timestamp,open,high,low,close,volume
2020-01-01 00:00:00,7200.5,7250.1,7190.0,7240.3,153.23
2020-01-01 01:00:00,7240.3,7280.5,7230.4,7265.8,98.45
...
</pre>

<hr />

<h2>🎯 Future Improvements</h2>
<ul>
  <li>Add retry & error handling for failed downloads.</li>
  <li>Convert notebook into a robust CLI tool.</li>
  <li>Automated tests + CI pipeline.</li>
  <li>Optional database integration (SQLite / PostgreSQL).</li>
</ul>

<hr />

<h2>📸 Screenshots</h2>
<p align="center">
  <img src="https://via.placeholder.com/800x400?text=Sample+CSV+Output" alt="CSV Output Example" />
</p>

<hr />

<h2>📜 License</h2>
<p>This project is licensed under the <a href="https://opensource.org/licenses/MIT">CC0-1.0 license</a>.</p>

<hr />

<h2>🙌 Acknowledgements</h2>
<ul>
  <li>Crypto exchanges & data archives for historical datasets</li>
  <li>Open-source Python community</li>
</ul>

<hr />

<p align="center"><em>Built with ❤️ by Antony Joseph</em></p>
