## **Stash** 

- #### É uma área, onde é possível armazenar código, sem a necessidade de ralizar um commit, permitindo
mudar de branch ou realizar outras operações de forma organizada.

    git checkout -b feature4
    git status
    echo h > h.txt
    git status

- #### Vamos supor que não queremos mais essa alteração, mas não
queremos descarta-la, isso tipicamente iriamos mover para o desktop,
mas no git podemos usar o stash para armazenar.

    git stash save "h.txt"
