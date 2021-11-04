task 1.1 result (git work history):  

 1934  mkdir m1  
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
