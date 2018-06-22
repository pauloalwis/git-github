## Canceitos Básicos:

- #### Para verificar a versão instalada:
  
      ```git version```
  
- #### Criando um repositório vazio dentro da pasta escolhida:
  
      ```git init```

- #### Mostra a estrutura de pastas, onde o 'git' vai armazenar todo o projeto.
  
      ```tree .git```
  
   O Git armazena o conteúdo de um jeito muito 'diferente do outros'
     equanto os outros pensam em arquivos, o 'git' armazena o conteúdo de uma
     só vez.

	 O Git representa a evolução do código-fonte por meio de um grafo de 'commits'.
	 
	 *imagem do grafo*
	 	 
- #### Criando o 1º commite
  
     4.1 Adicionando 2 arquivos de textos na pasta.
         
		 ```echo a > a.txt
            echo a > b.txt```
	 
	 4.2 Informando a linha de comando,  
	     ele vai nos informar que não tem nada para commitar.
	 
	     ```git commit```
	 
	      
- #### As coisas que tem que ser commitadas tem que ser adicionadas
   primeiramente na 'STAGING AREA' ( pense 'STAGING AREA' como um container ), para 
   adicionar os arquivos para commite use a linha de comando:
     
	 **imagem do staging area**
	 
     ```git add```

- #### Para saber o que tem para commitar ou oque esta fora do container 
   use a linha de comando.	 
	 
	 ```git status```

    apresentando em vermelho oque esta fora do container.
	 
- #### Para adicionar todos os arquivos de uma só vez: 
	 
	 ```git add -A ou all```
	 
- #### Para commitar as alterações e inclusões na 'STAGING AREA'

   * git commit -m "mensagem de commite"	

- #### Para apresentar os log de commites use o comando:
  
  ```git log```

- ####  Criando um novo arquivos
   
   ```echo c > c.txt
      git status
      git add -A
      git commit -m "c.txt"```

- #### E se um arquivo for alterado?
    
	11.1 Alterando o arquivo.
	   
	   ```echo c2 > c.txt
          ecat c.txt```
	  
	11.2 Verificar mudanças, adicionar no 'STAGING AREA' e commitar 
	   
	   ```git status
          git add -A
          git commit -m "Alterando c.txt"```
	
- #### E se apenas o nome do arquivo for alterado?
    
	12.1 Alterando o nome do arquivo
	
	```mv c.txt c2.txt```
	
	12.2 Verificar mudanças, adicionar no 'STAGING AREA' e commitar 
	   
	   ```git status
	      git add -A
	      git commit -m "Alterando o nome do arquivo para c2.txt"```
	 
	 
- #### Para mostrar um lista de log bem mais organizada
    
	```git log --oneline```

- #### Comando utilizados nesta introdução:
    
    - version
    - init
    - add
    - status
    - commit
    - log
