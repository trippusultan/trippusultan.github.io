# Deploy to GitHub Pages

## Steps

1. Create a new GitHub repository named `trippusultan.github.io`
   ```bash
   gh repo create trippusultan.github.io --public --homepage https://trippusultan.github.io
   ```

2. Push the portfolio files
   ```bash
   cd portfolio
   git init
   git add .
   git commit -m "Initial commit — portfolio site"
   git branch -M main
   git remote add origin git@github.com:trippusultan/trippusultan.github.io.git
   git push -u origin main
   ```

3. Enable GitHub Pages
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` / `/ (root)`
   - Save

4. Site goes live at **https://trippusultan.github.io** (within 2 minutes)

## Custom Domain (Optional)

Add a `CNAME` file with your custom domain and configure DNS:
- Type: A
- Value: 185.199.108.153 (and the other 3 GitHub IPs)
