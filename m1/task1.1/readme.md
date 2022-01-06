## task 1.1 result:  
1. Install GIT: 	`sudo apt install git`, `git --version` //git version 2.25.1  
2.  add name and email:	 `git config --global user.name "Viacheslav Shevtsov"`, `git config --global user.email "MY_NAME@example.com"`  
	setup core text editor:	 `git config --global core.editor nano`  
Output: `cat /home/ubuntu/.gitconfig`

```
[user]
        name = Viacheslav Shevtsov
        email = shevtsho.v@gmail.com
[core]
        editor = nano
```

3. Create account on GitHub: https://github.com/shevtshov  
4. Create new private repo on GitHub: https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4   


5-6. 
 `git clone git@github.com:shevtshov/DevOps_online_Dnipro_2021Q4.git`

### 7-26. git history in the terminal:
``` 1934  mkdir m1  
 1935  mkdir m1/task1.1  
 1936  cd m1/task1.1  
 1937  touch readme.txt  
 1938  git checkout -b develop  
 1939  touch index.html  
 1940  git commit  
 1941  git add index.html  
 1942  git commit -m "added index.html"  
 1943  git checkout -b images  
 1944  mkdir images  
 1945  cp ~/Desktop/logo.png ~/Downloads/courses/devops/DevOps_online_Dnipro_2021Q4/m1/task1.1/  
 1946  nano index.html  
 1947  ls  
 1948  mv logo.png images  
 1949  cat index.html  
 1950  git add .  
 1951  git commit -m "added images"  
 1952  ls  
 1953  ls -l  
 1954  git checkout develop  
 1955  git checkout -b styles  
 1956  mkdir styles  
 1957  nano styles/styles.css  
 1958  git add styles/styles.css  
 1959  git commit -m "added styles.css"  
 1960  nano index.html  
 1961  git add .  
 1962  git commit -m "changes index.html"  
 1963  git checkout develop  
 1964  git merge images  
 1965  git merge styles  
 1966  git status  
 1967  git mergetool  
 1968  git merge styles  
 1969  cat index.html  
 1970  nano index.html  
 1971  git add index.html  
 1972  git commit -m "Merged main fixed conflict"  
 1973  git status  
 1974  git checkout main  
 1975  git merge develop  
 1976  git log  
 1977  git push origin --all  
 1978  git reflog  
 1979  git reflog >> ~/Desktop/task1.1_GIT.txt  
 1980  cat ~/Desktop/task1.1_GIT.txt  
 1981  mv ~/Desktop/task1.1_GIT.txt ~/Downloads/courses/devops/DevOps_online_Dnipro_2021Q4/m1/task1.1  
 1982  touch readme.md  
 1983  git push origin --all  
 1984  git add readme.md  
 1985  git commit -m "added readme.md"  
 1986  git push origin --all 
 ```

## what DevOps is
Devops is a specialist who interacts between all teams, automates the processes of development, testing, deployment of the product and delivery to the production
