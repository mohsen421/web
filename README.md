# web
every code about web

# Windows Site Diagnostic Tool

A lightweight Windows Batch script that automates website and network diagnostics. It prompts the user for a target URL/domain, performs tests (DNS, Ping, Traceroute, HTTP Status), and exports a detailed time-stamped text report.

---

## 🚀 Features

* **URL Sanitization:** Automatically cleans inputs (removes `http://`, `https://`, and path suffixes).
* **DNS Resolution Check:** Uses `nslookup` to verify domain resolution.
* **Ping Connectivity:** Tests packet reachability and latency.
* **Traceroute Analysis:** Runs a capped `tracert` (15 hops) to detect network bottlenecks.
* **HTTP/HTTPS Status Check:** Executes a PowerShell web request to inspect HTTP response codes and server availability.
* **Automated Report Generation:** Saves all outputs into a `.txt` file with system and timestamp context.

---

## 🛠️ Usage

1. **Clone or Download** this repository.
2. Double-click **`site_diagnostics.bat`** to run the script.
3. Enter the website domain (e.g., `example.com` or `https://example.com/page`).
4. Wait for the tests to complete.
5. Choose whether to open the generated report in Notepad when finished.

---

## 📂 Output Example

The script creates a text file named: `report_<domain>_<timestamp>.txt` containing sections for:
* DNS Lookup Result
* Ping Statistics
* Traceroute Hops
* HTTPS Response Header / Error details
* Local DNS Cache context

---

## ⚖️ License

This project is licensed under the [MIT License](LICENSE).
