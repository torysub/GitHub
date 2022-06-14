# GitHub

1. На локальном репозитории сделать ветки для:

- Postman 

`git branch Postman`

- Jmeter 

`git branch Jmeter`
			
- CheckLists 

`git branch CheckLists`

- Bag Reports 

`git branch BugReports`

- SQL 

`git branch SQL`

- Charles 

`git branch Charles`

- Mobile testing 

`git branch MobileTesting`


2. Запушить все ветки на внешний репозиторий 

`git push -u origin --all`

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта 

```
git checkout BugReports

vim Bug_Reports.txt
```

```
Bug-ID: 
  Title: 
  Project: Сайт магазина 'Malina'
  STR: 
    1. 
    2. 
    3. 
  AR: 
  ER: 
  Environment:
    OS : 
    Browser : 
  Severity: 
  Priority:
  Status: 
  Author:
  ```
  
  *Нажимаем **"ESC"** :wq **"Enter"***

4. Запушить структуру багрепорта на внешний репозиторий 

`git add . && git commit -m "Added Bug_Reports.txt" && git push`

5. Вмержить ветку Bag Reports в Main 

```
git checkout main 

git merge BugReports
```

6. Запушить main на внешний репозиторий. 

`git push`

7. В ветке CheckLists набросать структуру чек листа. 

```
git checkout CheckLists 

vim Check_List.txt
```

```
Environments:				
Test date:				
Tester:				
№ | Checking | expected result | Status | Comment |
1
2
3
```

 *Нажимаем **"ESC"** :wq **"Enter"***

8. Запушить структуру на внешний репозиторий 

`git add . && git commit -m "Added Check_list.txt" && git push`

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main 

![image](https://user-images.githubusercontent.com/105368491/173565507-a91a27f5-0ad4-4b75-99f9-ccc298b69d13.png)

*Compare & pull request*

![image](https://user-images.githubusercontent.com/105368491/173565582-1feebd74-250b-4d93-a021-e4898464186e.png)

![image](https://user-images.githubusercontent.com/105368491/173565900-60708b62-17b0-4f71-8ced-99776b25a621.png)

*Create pull request*

![image](https://user-images.githubusercontent.com/105368491/173565941-2de03d05-433d-4e0a-8a47-8caeaf4b9fdf.png)

*Merge pull request*

![image](https://user-images.githubusercontent.com/105368491/173566224-3af3adb3-dd53-49fc-92d3-005dc309560f.png)

*Confirm merge*

![image](https://user-images.githubusercontent.com/105368491/173566415-0e5f585f-6214-4aef-96f5-3fb330bb963c.png)

10. Синхронизировать Внешнюю и Локальную ветки Main 

```
git checkout main 

git pull
```
