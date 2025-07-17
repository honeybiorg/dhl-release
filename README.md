# dhl-release
dhl-release for big files
# 📌 Ladda upp stora filer med Git LFS

Denna guide visar hur man laddar upp stora filer (t.ex. `.zip`) till GitHub med **Git Large File Storage (LFS)**.

---

## ✅ Första gången (installera Git LFS)

Installera Git LFS på din dator (endast första gången):

```bash
git lfs install
## ✅ Första gången (installera Git LFS)

Installera Git LFS på din dator (endast första gången):
## ✅ Lägg till nytt filformat (t.ex. .zip)
git lfs track "*.zip"
git add .gitattributes
## ✅ Lägg till filerna och pusha
git add Postman-win64-Setup.zip
git commit -m "Postman-win64-Setup.zip"
git push origin main

# Klona ett nytt repo (hämtar automatiskt LFS-filer)
git clone https://github.com/<user>/<repo>.git

# Om du redan klonat repot, hämta LFS-filer manuellt:
git lfs pull
