# 🏢 Placement Drive Merit Ranking System

## 📌 Project Overview
A data-processing Python script built for college Training and Placement Cells. It ingests raw aptitude scores, filters candidates based on a cutoff, and ranks them using a custom implementation of the Selection Sort algorithm.

## 🚀 Features
- **Automated Data Parsing:** Reads text files and safely typecasts string data into evaluable integers.
- **Custom Sorting Logic:** Uses an in-place Selection Sort algorithm to rank 2D lists dynamically.
- **Report Generation:** Automatically generates a formatted `merit_list.txt` for easy printing or mailing.

## ⚙️ How to Run
1. Clone the repository and navigate to the folder.
2. Create a file named `aptitude_results.txt` and add scores (e.g., `Rohit, 65`).
3. Run the script:
   ```bash
   python ranker.py
   ```
4. Check the newly generated merit_list.txt for the final rankings.
5. UI Idea: HTML Frontend (TPO Portal)
*Save as `tpo_portal.html`*
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>TPO Merit Generator</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-secondary p-5">
    <div class="container bg-white p-4 rounded shadow" style="max-width: 600px;">
        <h2 class="text-center text-dark border-bottom pb-3">🏢 Placement Cell Portal</h2>
        
        <div class="mt-4">
            <label class="form-label fw-bold">1. Upload Raw Aptitude Scores (.txt)</label>
            <input class="form-control mb-3" type="file">
            
            <label class="form-label fw-bold">2. Set Company Cutoff Marks</label>
            <input type="number" class="form-control mb-4" value="60">
            
            <button class="btn btn-dark w-100 fs-5">Process & Generate Merit List</button>
        </div>

        <div class="mt-4 p-3 bg-light border rounded text-center text-muted">
            <p class="mb-0"><em>Merit list will appear here after processing...</em></p>
        </div>
    </div>
</body>
</html>
