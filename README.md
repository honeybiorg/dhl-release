# dhl-release
dhl-release for big files
# 📌 Ladda upp stora filer med Git LFS

Denna guide visar hur man laddar upp stora filer (t.ex. `.zip`) till GitHub med **Git Large File Storage (LFS)**.

---
```bash
## Installera GIT LFS. Bara första gången
git lfs install
## Lägg till nytt filformat (t.ex. .zip)
git lfs track "*.zip"
git add .gitattributes
## Lägg till filerna och pusha
git add bigfile.zip
git commit -m "bigfile.zip"
git push origin main

## Klona ett nytt repo (hämtar automatiskt LFS-filer)
git clone https://github.com/<user>/<repo>.git

## Om du redan klonat repot, hämta LFS-filer manuellt:
git lfs pull
