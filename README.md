# AquaDrone Website

This is the static frontend for the AquaDrone underwater environmental monitoring dashboard.

## Publish with GitHub Pages

1. Create a **public** GitHub repository named `AquaDrone-AI`.
2. Upload `index.html`, `.nojekyll`, and this README to the repository root.
3. Open **Settings → Pages**.
4. Under Build and deployment, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then Save.
6. Wait for GitHub Pages to publish. The URL will look like:
   `https://YOUR-GITHUB-USERNAME.github.io/AquaDrone-AI/`

## Important: connect the AI backend

The dashboard's AI prediction request has been changed to this placeholder:

`https://YOUR-RENDER-SERVICE.onrender.com/predict`

After deploying the Flask API to Render, replace `YOUR-RENDER-SERVICE` in `index.html` with your actual Render service hostname, commit the change, and push it to GitHub.

The local URL `127.0.0.1:5000` is only reachable on the computer running the API; it cannot be used by a public website visitor.

Deploy the Flask API separately. Ensure its CORS configuration permits your GitHub Pages website origin.

## Demo-data notice

The dashboard contains simulated/example sensor readings and demo visualizations. Live GPS, real sensor telemetry, underwater camera analysis, and confirmed microplastic identification require the corresponding hardware, backend, calibration, and validation. Optical anomaly screening alone does not confirm that a particle is plastic.
