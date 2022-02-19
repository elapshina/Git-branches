1. На локальном репозитории сделать ветки для:
- Postman 
- Jmeter 
- CheckLists 
- Bag Reports 
- SQL 
- Charles
- Mobile testing

- `git branch Postman;git branch Jmeter;git branch CheckLists;git branch Bug_Reports;git branch SQL;git branch Charles;git branch Mobile_testing`

2. Запушить все ветки на внешний репозиторий

    `git push -u origin --all`

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта

 - `git checkout Bug_Reports`
 - `cat>bug_report.txt`
 ```
Project
Summary
Descriprion
- STR
- Actual result
- Expected result
Environment
Attachment
Lables
Severity
Priority
```
 
4. Запушить структуру багрепорта на внешний репозиторий
- `git add bug_report.txt`
- `git commit -m "add bug_report.txt"` ;` 
- `git push`

5. Вмержить ветку Bag Reports в Main
- `git checkout main`
- `git merge Bug_Reports`

6. Запушить main на внешний репозиторий

- `git push`

7. В ветке CheckLists набросать структуру чек листа
 - `git checkout CheckLists`
 - `cat>checklist.txt`
 ```
Buid
Environment
Test date
Tester
Test type
Checking
Result
```

8. Запушить структуру на внешний репозиторий
- `git add checklist.txt`
- `git commit -m "add checklist.txt"`
- `git push`

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
 - перейти во внешний репозиторий, нажать:
- `Compare & pull request`
- `Create pull request`


10. Синхронизировать Внешнюю и Локальную ветки Main
- `git checkout main`
- `git pull`
