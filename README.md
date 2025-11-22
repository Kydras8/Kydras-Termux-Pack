<!-- Kydras Repo Header -->
<p align="center">
  <strong>Kydras Systems Inc.</strong><br/>
  <em>Nothing is off limits.</em>
</p>

---

# Kydras Termux Custom Banner
🎨 Personal custom Termux banner with GitHub identity splash and operator mode activation.
## 🟣 Installation
```bash
cd ~/Kydras-Termux-Pack/tools/custom-banner
bash install-banner.sh
🟣 Features
Kydras ASCII Banner on Termux start
Displays GitHub Username (Kydras8)
Operator-ready terminal experience
✅ Just paste this into your `tools/custom-banner/README.md` and commit.
---
###✅ **Step 2: Auto-loader for `.bashrc`**
In Termux:
```bash
echo 'bash ~/Kydras-Termux-Pack/tools/custom-banner/install-banner.sh' >> ~/.bashrc
✅ This makes Termux auto-load your banner on every new session.
---
✅ Step 3: Git Push Script
Create a helper file:
nano push-banner.sh
Paste:
#!/data/data/com.termux/files/usr/bin/bash
cd ~/Kydras-Termux-Pack
git add .
git commit -m "Banner updates 🚀"
git push
echo "✅ Banner updates pushed to GitHub."
chmod +x push-banner.sh
✅ Now you can update and push banner changes in one command:
bash push-banner.sh

