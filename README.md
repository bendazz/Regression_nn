Linear Regression MSE Practice App
=================================

This is a small front-end web app for students to practice computing Mean Squared Error (MSE) for linear regression.

Features
- Generates a random dataset (1–20 rows) with features `X1..Xk` and target `Y`.
- Provides weights `w1..wk` and a bias `b` for predictions.
- Shows a copyable CSV for each question.
- Students compute the MSE by hand, then click “Reveal Answer” to check.
- `Y` is generated from the model (`w·X + b`) with moderate noise so the fit isn’t perfect.

Quick Start
1. Open the app by serving the root folder and visiting it in a browser.
	Example using Python’s simple HTTP server:

	```bash
	cd /workspaces/Regression_nn
	python3 -m http.server 8000
	```

2. Visit http://localhost:8000 and open `index.html`.

Usage
- Use the controls to choose number of rows (1–20) and features (2–5).
- Choose the value range for `X`. `Y` is derived from `w·X + b` with moderate noise.
- Click “New Question” to regenerate.
- Copy the CSV, compute predictions using the shown weights and bias, then compute the MSE.
- Click “Reveal Answer” to see the MSE.

Notes
- The CSV header is `X1,...,Xk,Y` and the last column is always the target `Y`.
- Numbers are small integers or one-decimal floats to make calculations manageable.
- Datasets are randomly generated; results will vary per question. With built-in noise, MSE is generally non-zero.

File
- [index.html](index.html)

# Regression_nn