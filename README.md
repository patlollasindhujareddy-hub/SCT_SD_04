# SCT_SD_04
A lightweight Python data extractor built with native modules to fetch e-commerce product names, prices, and ratings, automatically exporting them into a structured CSV file. Zero-dependency design fully compatible with online compilers. Final task for SkillCraft Technologies Software Development Internship.
# SkillCraft Technologies - Software Development Internship

## Task: E-Commerce Product Data Extractor

### Project Description
This project is a lightweight, zero-setup Python application designed to extract product information from an online e-commerce database. The program automatically retrieves essential data points—including product names, prices, and customer ratings—and structures the data cleanly into a standard CSV file format. 

To ensure complete portability and allow seamless execution inside constrained online runtime environments (such as Programiz, OnlineGDB, or OneCompiler), the script relies strictly on Python's built-in libraries. It demonstrates efficient remote data fetching, JSON parsing, file I/O operations, and dynamic terminal rendering without requiring external third-party dependencies like BeautifulSoup or Requests.

---

### Key Features
* **Zero Dependency Architecture:** Uses only native Python modules (`urllib`, `json`, `csv`) for universal compatibility across all online compilers.
* **Structured Data Export:** Generates a spreadsheet-compatible `products.csv` file, automatically handling data string parsing and proper field division.
* **Automated Console Previews:** Prints a real-time validation log and a snapshot of the resulting spreadsheet data straight to the execution terminal.
* **Robust Exception Handling:** Integrated safe-fail checks to catch and log errors during the HTTP handshake or file writing processes.

---

### Technical Architecture
* **Language:** Python 3.x
* **Data Stream Source:** FakeStore REST API (E-Commerce endpoint)
* **Core Standard Modules Used:**
  * `urllib.request` — Manages network handshakes and payload extraction.
  * `json` — Deserializes raw string payloads into manageable data objects.
  * `csv` — Formats and structures string text objects into rows and cells.

---

### Execution Instructions
1. Open any standard web browser.
2. Copy the script code into an online environment like the [Programiz Python Compiler](https://www.programiz.com/python-programming/online-compiler/).
3. Click the **Run** button to execute.
4. The console will display the tracking logs followed by the structured CSV output matrix.

---

### Expected Console Output
```text
Fetching product data from the e-commerce database...

SUCCESS!
A file named 'products.csv' has been created in the compiler's temporary memory.
--------------------------------------------------
HERE IS WHAT YOUR GENERATED CSV DATA LOOKS LIKE:

Product Name,Price,Rating
"Fjallraven - Foldsack No. 1 Backpack, Fits 15 Laptops",$109.95,3.9 / 5
Mens Casual Premium Slim Fit T-Shirts,$22.3,4.1 / 5
Mens Cotton Jacket,$55.99,4.7 / 5
Mens Casual Slim Fit,$15.99,2.1 / 5
... [truncated for preview] ...
