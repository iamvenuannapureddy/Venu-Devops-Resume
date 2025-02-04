## To attach your **GoDaddy domain (`venuresume.pro`)** to your **GitHub Pages URL (`https://iamvenuannapureddy.github.io/Venu-Devops-Resume/`)**, follow these steps:

---

### **Step 1: Add the Custom Domain in GitHub**
1. Go to your **GitHub repository**:  
   👉 [https://github.com/iamvenuannapureddy/Venu-Devops-Resume](https://github.com/iamvenuannapureddy/Venu-Devops-Resume)  
2. Click **Settings** → **Pages** (left sidebar).  
3. Under **Custom domain**, enter:  
   ```
   venuresume.pro
   ```
4. Click **Save**.  
5. This will create a `CNAME` file inside your repository with `venuresume.pro`.

---

### **Step 2: Configure DNS Settings in GoDaddy**
1. **Log in to GoDaddy** → Go to **My Products** → Click on your domain (`venuresume.pro`).  
2. **Go to DNS Settings** and look for the section **Records**.  
3. **Delete any existing A or CNAME records pointing elsewhere** (if any).  
4. **Add the following DNS records:**

#### **For Root Domain (`venuresume.pro`)**
| Type  | Name  | Value                     |
|-------|-------|---------------------------|
| A     | @     | `185.199.108.153`         |
| A     | @     | `185.199.109.153`         |
| A     | @     | `185.199.110.153`         |
| A     | @     | `185.199.111.153`         |

#### **For Subdomain (`www.venuresume.pro`)**
| Type  | Name  | Value                                  |
|-------|-------|----------------------------------------|
| CNAME | www   | `iamvenuannapureddy.github.io` |

5. **Save the changes.**  

---

### **Step 3: Enable HTTPS in GitHub**
1. After **DNS changes propagate** (may take a few minutes to hours), go back to **GitHub Pages Settings**.  
2. Check the box **Enforce HTTPS** (if it's available).  

---

### **Step 4: Verify the Setup**
1. Open a browser and go to:  
   👉 **https://venuresume.pro**  
   👉 **https://www.venuresume.pro**  

If everything is set up correctly, it should display your GitHub Pages website. 🚀  

---

### **Troubleshooting**
- If the domain doesn’t work immediately, wait **30 minutes to 24 hours** for DNS changes to propagate.  
- Check the DNS settings using this tool: [https://dnschecker.org/](https://dnschecker.org/)  
- If there's an issue, ensure you removed old DNS records and only have the correct A and CNAME records.  

Would you like me to verify your DNS setup? 😊
