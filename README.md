# ProofWork Working Model — ThinkForge

A static, GitHub Pages-friendly concept prototype for the ProofWork skills-assessment idea.

## Run on your Mac
1. Download and unzip `ProofWork_Working_Model.zip`.
2. Open the extracted folder.
3. Double-click `index.html` to open it in a browser.
4. Connect to the internet for the first assessment run: Pyodide (Python in WebAssembly) loads from jsDelivr CDN.
5. Scroll to **Try a Python assessment**, edit the function, and click **Run tests & generate report**.
6. Inspect the live test results and rubric breakdown. Use **Download report (.json)** or **Print report**.

## Publish through GitHub Pages
1. Create/open your GitHub repository.
2. Upload `index.html` and `README.md` to the repository root (or upload the extracted folder contents).
3. In the repository, open **Settings → Pages**.
4. Under Build and deployment, select **Deploy from a branch**, choose `main` and `/ (root)`, then Save.
5. Wait for GitHub Pages to publish the site. It will show the public URL in Settings → Pages.

## What works in this prototype
- Responsive landing page and workflow overview.
- Interactive Python task.
- Real Python execution in the browser through Pyodide.
- Six test cases with expected outputs.
- Transparent demo rubric breakdown (correctness, edge cases, basic readability signals).
- Evidence-linked results panel.
- Downloadable JSON report and browser print option.
- No server, account, or database needed; submissions are processed in the browser.

## Important limitations
- This is a prototype, not a production hiring product.
- The rubric's readability signals are deliberately simple and do not measure professional code quality.
- Browser-side execution is suitable for a demo but is not a hardened, adversarially secure sandbox for untrusted code. Do not use it for real hiring decisions or sensitive candidate data.
- No candidate information is transmitted or saved by this page. Python runtime is downloaded from a CDN when first used, so an internet connection is needed.
- Scores are illustrative prototype signals, not validated measures of job performance. A human reviewer must remain involved.
