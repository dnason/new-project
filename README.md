Init text
mkdir new-project
cd new-project
git init --initial-branch=master
echo "# New Project" > README.md
git add README.md
git commit -m "init"
git checkout -b development
echo "Це інструкція до проєкту." >> README.md
git add README.md
git commit -m "KEY-123 #comment Додано інструкцію до README.md #done"
git checkout main
git merge development

