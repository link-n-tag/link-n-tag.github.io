# Deploying to GitHub Pages

## Automatic Deployment (Recommended)

This project uses GitHub Actions to automatically deploy to GitHub Pages whenever you push to the `main` branch.

### Setup (One-time)

1. **Enable GitHub Pages in your repository**:
   - Go to your GitHub repository: https://github.com/danielsussa/link-n-tag
   - Click on **Settings** → **Pages**
   - Under **Source**, select **GitHub Actions**
   - Click **Save**

2. **Push your code to GitHub**:
   ```bash
   git add .
   git commit -m "Add GitHub Actions deployment"
   git push origin main
   ```

3. **That's it!** The GitHub Action will automatically:
   - Build your React app
   - Deploy it to GitHub Pages
   - Your site will be available at: `https://danielsussa.github.io/link-n-tag`

### How it works

- Every time you push to the `main` branch, the workflow automatically runs
- The workflow builds the React app and deploys it to GitHub Pages
- No manual steps needed!

## Manual Deployment (Alternative)

If you prefer to deploy manually, you can still use the `gh-pages` package:

### Prerequisites
1. Make sure you have `gh-pages` installed (run `npm install` in the client directory)

### Steps

1. **Install dependencies**:
   ```bash
   cd client
   npm install
   ```

2. **Deploy to GitHub Pages**:
   ```bash
   npm run deploy
   ```

   Or from the root directory:
   ```bash
   npm run deploy
   ```

## Notes
- The homepage is configured in `client/package.json`: `"homepage": "https://danielsussa.github.io/link-n-tag"`
- GitHub Pages may take a few minutes to update after deployment
- The GitHub Actions workflow is located in `.github/workflows/deploy.yml`

