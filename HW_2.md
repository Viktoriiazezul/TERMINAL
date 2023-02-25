На локальном репозитории сделать ветки для:
Postman - git branch Postman
Jmeter - git branch Jmeter
CheckLists - git branch CheckList
Bag Reports - git branch Bag_Reports
SQL - git branch SQL
Charles - git branch Charles
Mobile testing - git branch Mobile testing
Запушить все ветки на внешний репозиторий
git push -u origin Postman
git push -u origin Jmeter
git push -u origin CheckList
git push -u origin Bag_Reports
git push -u origin SQL
git push -u origin Charles
git push -u origin Mobile_testing
В ветке Bag Reports сделать текстовый документ со структурой баг репорта

git checkout Bag_Reports
cat > structure.txt
Bug Summary
Severity
Steps to reproduce
Actual Result
Expected Result
ctrl+C

Запушить структуру багрепорта на внешний репозиторий

git add structure.txt
git commit -m structure.txt
git push -u origin Bag_Reports
Вмержить ветку Bag Reports в Main

git checkout main
git merge Bag_Reports
Запушить main на внешний репозиторий.
git push -u origin Bag_Reports
В ветке CheckLists набросать структуру чек листа.
git checkout CheckList
cat > structure_Checklist.txt
passed
failed
blocked
skipped
no run
ctrl+C
Запушить структуру на внешний репозиторий
git add structure_Checklist.txt
git commit -m structure_Checklist.txt
git push -u origin structure_Checklist.txt
На внешнем репозитории сделать Pull Request ветки CheckLists в main
create pull request
merge pull request
confirm merge
Синхронизировать Внешнюю и Локальную ветки Main git clone https://github.com/Viktoriiazezul/TERMINAL.git
