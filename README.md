# Codeigniter-HMVC-Geosan
#### Codeigniter 3.0.6 em HMVC.
#### Geosan é uma ferramenta que auxilia na criação da base de modulos de forma automática.

 - modulo - Diretiva para criar modulos
 - controller -	Diretiva para criar controllers
 - model - Diretiva para criar models 

# Instalar:  

    Abra o terminal e execute ‘git clone https://github.com/Georde/Codeigniter-HMVC-Geosan.git’ ou faça o download.

  
  *Já está no ponto de usar, com o Codeigniter configurado no padrão HMVC.*
  
# Como usar:

*Para usar o Geosan, digite no terminal:*

    php index.php geosan

*Se preferir, você pode criar um comando para agilizar a criação dos módulos (Recomendado)*

    vim ~/.bash_profile
  *Depois aperte ESC*
  
*Adicione no final do arquivo:*

    alias geosan="php index.php geosan"

*Salve e feche o editor vim:*

    :wq!
  
*Depois digite:*

    source ~/.bash_profile

**Pronto!**

  *Agora você pode usar o comando geosan para criar seus módulos no Codeigniter.*


###Criar módulos
    geosan modulo [nomedomodulo]
    
**Exemplo:**

    geosan modulo usuarios 
    
  *(Cria o módulo usuarios e as pastas controllers, views e models)*

###Criar controllers
    geosan controller [nomedomodulo] [nomedocontroller]
    
  **Exemplo:**
  
    geosan modulo usuarios admin 
  *(Cria o controller admin no módulo usuarios)*
  
###Criar Models
    geosan controller [nomedomodulo] [nomedomodel] [tabela*] [chaveprimaria*]
    
  **Exemplo:**
 
    geosan model usuarios admin usuarios idUsuario 
  *(Cria o model admin no módulo usuarios e seta uma variável com o nome da tabela usuarios e seta uma variável como idUsuario)*
  
  **Exemplo2:**
 
    geosan model usuarios admin 
  *(Cria o model admin no módulo usuarios)*
