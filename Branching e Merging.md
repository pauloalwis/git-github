## Branching e Merging:

- #### O que é um branch e o que eu ganho em utilizá-lo?
    
     - Um 'branch' é uma nova linha de desenvolvimento que permite isolar o código de uma nova funcionalidade, mantendo a linha base 'estável', evitando o represamento de código.
  
- Para verificar uma *branch*
   
      git branch

- #### Para criar uma *branch*
  
      git branch umanovabranch
  
- #### No *Git*, uma *branch* é apenas um ponteiro uma referência para um *commit*.

     - Podendo ser verificada com o comando:

      car .git/refs/heads/master
      car .git/refs/heads/umanovabranch

- #### Para verificar no log:
   
      git log --oneline --decorate
  
- #### HEAD?
   
     - É onde se esta trabalhando no momento:
   
      cat .git/HEAD
  
- #### Trocando de *branch*
    
      git checkout umanovabranch
  
- #### Criando um commite no *branch*
  
      echo d > d.txt
      git add -A
      git commit -m "d.txt" 
  
- #### Para mostrar todas os *branchs*
   
      git log --oneline --decorate --all
  
- #### Realizando um *merge* no master.
    
      git merge umanovabranch
  
     - A estratégia *FAST-FORWARD* é apenas uma atualização da referência e só é possível quando não existe divergência entre os *branchs*. 

      git log --oneline --decorate --all
  
      Agora verificamos que esta tudo no mesmo commite.

- #### Deletando uma branch:

      git branch -d umanovabranch
  
      Se olharmos novamente o log, vamos ver que só temos o master novamente:
      
	  git log --oneline --decorate --all    
    
- #### Criando uma 'divergência' entre o *master* e o *branch*

     - Criar branch:
	  
	  git branch feature2
	  git checkout feature2
      
	  ou
      
	  git checkout -b feature2 'Faz o checkout e cria a branch'
  
	  ech e > e.txt
	  git add -A
	  git commit -m "e.txt"
  
   
    
