# DevOps Internship - Task 6: Hosting Static Website with GitHub Pages

## 📋 Task Description  
**Objective:** Deploy a simple HTML/CSS website using GitHub Pages  
**Tools Used:** GitHub Pages, HTML, CSS  
**Key Requirements:**  
- Create `index.html` and `styles.css` files  
- Push code to a GitHub repository  
- Enable GitHub Pages in repository settings  
- Access live website via GitHub-provided URL  
- Answer interview questions about GitHub Pages  

---

## 🔗 Live Website  
**Access the deployed website here:**  
[https://anugrahmassey.github.io/Hosting-a-Static-Website-with-GitHub-Pages/](https://anugrahmassey.github.io/Hosting-a-Static-Website-with-GitHub-Pages/)  

![Host Static Website with GitHub Pages](https://github.com/user-attachments/assets/10e76a85-938c-4ea0-964a-ce7dfe606e3b)

*Screenshot showing live website with URL in address bar*

---

## 🛠 Implementation Details  

### Files Created  
1. **`index.html`** (Homepage):  
```html
<!DOCTYPE html>
<html>
<head>
  <title>My GitHub Pages Website</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <h1>Welcome to My GitHub Pages Site!</h1>
  <p>Successfully deployed via GitHub Pages.</p>
  <p>By Anugrah Massey</p>
</body>
</html>
```

2. **`styles.css`** (Styling):  
```css
body {
  font-family: Arial, sans-serif;
  text-align: center;
  background-color: #042b4b;
  margin: 50px;
}
h1 {
  color: #a2acb6;
}
p {
  color: #7f8c8d;
}
```

### Steps Performed  
1. Created repository `Hosting Static Website with GitHub Pages` on GitHub
2. Added HTML and CSS files to the repository
3. Enabled GitHub Pages in repository Settings:
   - Source branch: `main`
   - Source folder: `/ (root)`
4. Verified live website availability after deployment
5. Created this README with task documentation

---

## 📚 Interview Questions & Answers  

### 1. What is GitHub Pages?
GitHub Pages is a **free static site hosting service** provided by GitHub. It takes HTML, CSS, and JavaScript files directly from a repository, builds them, and publishes them as a website. Key features:
- Hosted on GitHub's infrastructure
- Supports custom domains
- Automatic deployment on Git push
- Supports Jekyll for static site generation
- Free SSL/TLS encryption (HTTPS)

### 2. Can you host dynamic applications on GitHub Pages?
**No**, GitHub Pages is designed exclusively for **static content**. Limitations include:
- No server-side processing (PHP, Python, Ruby, Node.js not supported)
- No database connectivity
- No user authentication systems
- No form processing (unless using third-party services)
- No server-side redirects or rewrites

For dynamic applications, consider alternatives like Heroku, AWS EC2, or Netlify Functions.

### 3. What are the technical limits of GitHub Pages?
GitHub Pages has several important limitations:
- **Repository Size:** Max 1GB
- **Bandwidth:** 100GB/month
- **Builds:** 10 builds per hour
- **File Size:** Individual files ≤ 100MB
- **Content Restrictions:**
  - No illegal content
  - No violent/defamatory material
  - No cryptocurrency mining scripts
- **Technical Restrictions:**
  - No `node_modules` directory
  - No `.env` files
  - No server configuration files
- **Soft Limits:**
  - Recommended ≤ 100,000 files
  - Recommended repository ≤ 5GB total

### 4. How do you update the website content?
To update a GitHub Pages site:
1. Modify files locally (`index.html`, CSS, etc.)
2. Commit changes to GitHub:
   ```bash
   git add .
   git commit -m "Update website content"
   git push origin main
   ```
3. GitHub automatically rebuilds and deploys the site:
   - Process takes 1-3 minutes
   - Build status visible in repository's "Actions" tab
4. Refresh browser to see changes (may require cache clear)

### 5. What happens when you delete the repository?
Deleting the repository has immediate consequences:
1. Website becomes inaccessible (returns 404 error)
2. All build history is permanently deleted
3. Custom domain settings are lost
4. Previous deployments are unrecoverable
5. If the repository was named `<username>.github.io`, the root domain becomes unavailable

**Note:** To temporarily disable without deleting:
- Go to Settings → Pages → Disable GitHub Pages

### 6. What is the default file that loads?
The default loading behavior follows this priority:
1. `index.html` in the root directory
2. `index.md` (converted to HTML via Jekyll)
3. `README.md` (if no index files present)

For custom paths:
- `domain.com/about` looks for `about/index.html`
- `domain.com/blog/post` looks for `blog/post/index.html`

### 7. How do you use a custom domain?
There are two methods to add a custom domain:

**Method 1: Using CNAME File**
1. Create a `CNAME` file in the repository root
2. Add your domain: `www.yourdomain.com`
3. Configure DNS with your registrar:
   ```
   Type: CNAME
   Name: www
   Value: <username>.github.io
   ```

**Method 2: DNS Configuration**
1. In GitHub: Settings → Pages → Add custom domain
2. Configure DNS records:
   ```
   Type: A
   Name: @
   Value: 185.199.108.153
   Value: 185.199.109.153
   Value: 185.199.110.153
   Value: 185.199.111.153
   ```

**Post-Setup:**
- GitHub automatically creates HTTPS certificates
- Enforces HTTPS redirects
- Propagation takes 24-48 hours

---

## 📂 Repository Structure  
```
github-pages-static-website/
├── index.html          # Homepage
├── styles.css          # Styling
└──README.md           # Project documentation
```

---
### Conclusion  

This task demonstrated the **simplicity and power of GitHub Pages** for hosting static websites. By completing this exercise, I:  
- ✅ Mastered the end-to-end deployment workflow: from local development to live production  
- ✅ Learned GitHub Pages' core capabilities and limitations for static content  
- ✅ Explored key concepts like custom domains and HTTPS enforcement  
- ✅ Verified that free tools can deliver professional results  

GitHub Pages is an **essential tool** for developers to showcase portfolios, documentation, and project demos quickly. While limited to static sites, its seamless integration with GitHub repositories makes it ideal for rapid prototyping and educational purposes.  

This foundation prepares me for more advanced DevOps concepts like containerization, infrastructure-as-code, and dynamic application deployment.  

**Final Outcome:** Successfully deployed static website accessible at:  
[https://anugrahmassey.github.io/Hosting-a-Static-Website-with-GitHub-Pages/](https://anugrahmassey.github.io/Hosting-a-Static-Website-with-GitHub-Pages/) 

---
