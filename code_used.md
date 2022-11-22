# Here comes the common codes used during Edision projects.

---

### Git related issues

---

#### How to filter big files from pushed histories.
git filter-branch --force --index-filter 'git rm --cached --ignore-unmatch Adaptive_script/Porto/Onboard/Sigma_sal.h5' --prune-empty --tag-name-filter cat -- --all

git pull origin master --allow-unrelated-histories

git rm --cached -r **/.idea
git rm --cached -r **/__pycache__
git rm --cached -r *.DS_Store

### remote server related issues

scp -r target user@192.168.1.100:"/file\\ path\\ with\\ spaces/myfile.txt"
- black space is replaced by \\
