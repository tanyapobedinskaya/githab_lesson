1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing

git branch Postman; git branch Jmeter; git branch CheckList; git branch Bag_Report; git branch SQL; git branch Charles; git branch Mobile_testing;

2. Запушить все ветки на внешний репозиторий
 git push origin --all

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
git checkout Bag_Report
cat > bug_report.txt
1) ID
2) Severity
3) Priority
4) Enviroment
5) Preconditions
6) Summary
7) Steps
8) Actual_result
9) Expected_result
10) Attachments
11) Notes

Enter 
Ctrl +c

4. Запушить структуру багрепорта на внешний репозиторий
git add .
git commit -m "bag report structure"
git push -u origin Bag_Report

5. Вмержить ветку Bag Reports в Main
git checkout main
git merge Bag_Report

6. Запушить main на внешний репозиторий.
git push

7. В ветке CheckLists набросать структуру чек листа.
git checkout CheckList
cat > checklist.txt
1) ID
2) Action
3) Result
4) Comment

Enter
Ctrl +c

8. Запушить структуру на внешний репозиторий
git add checklist.txt
git commit -m "checklist structure"
git -u push origin CheckList

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
go to Checklist branch
Click "Compare & pull request"
Click "Create pull request"
Click "Merge pull request"
Click "Confirm merge"

10. Синхронизировать Внешнюю и Локальную ветки Main
git pull
