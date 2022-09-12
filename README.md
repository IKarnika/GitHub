GitHub. HW_2
1. На локальном репозитории сделать ветки для:  
- Postman  
```git branch Postman```    
- Jmeter  
```git branch Jmeter```  
- CheckLists  
```git branch Checklists```  
- Bag Reports  
```git branch Bug_reports```  
- SQL  
```git branch SQL```  
- Charles  
```git branch Charles```
- Mobile testing  
```git branch Mobile_testing```

2. Запушить все ветки на внешний репозиторий  
```git push -u origin Postman```  
```git push -u origin Jmeter```  
```git push -u origin Checklists```  
```git push -u origin Bug_reports```  
```git push -u origin SQL```  
```git push -u origin Charles```  
```git push -u origin Mobile_testing```  

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта  
```git chekout Bug_reports```  
```vim bug_report.txt```  
:--:
	ID  
	Summary  
	STR  
	Actual_result  
	Expected_result  
	Environment  
	Build  
	Severity  
	Priority  
	Attachments  
```Esc, :wq, enter```

4. Запушить структуру багрепорта на внешний репозиторий
git add bug_report.txt
git commit -m "Added new file Bug_report"
git push

5. Вмержить ветку Bag Reports в Main
git checkout main
git merge bug_report

6. Запушить main на внешний репозиторий.
git push

7. В ветке CheckLists набросать структуру чек листа.
git checkout checklists
vim checklist.txt
	Title
	Actual_result
	Expected_result
	Attachments

8. Запушить структуру на внешний репозиторий
git add checklist.txt
git commit -m "Added new checklist"
git push

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
github.com
click on "Compare & pull request"

10. Синхронизировать Внешнюю и Локальную ветки Main
git checkout main
git pull
