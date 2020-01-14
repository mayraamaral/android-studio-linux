# Android Studio no Linux
Repositório simples para servir como guia para instalação do Android Studio no Linux Ubuntu, a versão que estou utilizando é a 18.04.  
  
## Guia
* [1. Baixando o arquivo](#1-baixando-o-arquivo)
* [2. Descompactando](#2-descompactando)
* [3. Instalando](#3-instalando)
* [4. Adicionando ao launcher](#4-adicionando-ao-launcher)
* [5. Adicionando à Área de Trabalho](#5-adicionando-a-area-de-trabalho)
  
## 1. Baixando o arquivo
Baixe o arquivo .tar.gz no [site do Android Studio](https://developer.android.com/studio).  
  
## 2. Descompactando
Descompacte esse arquivo .tar.gz dentro da pasta /usr/local conforme instrui no site do Androi Studio, para isso, use o seguinte código:  
  
Para facilitar, renomeie antes o arquivo baixado para "android-studio".  
  
```sudo tar -zxvf android-studio.tar.gz -C /usr/local```  
  
## 3. Instalando
Agora acesse a pasta **bin** dentro da pasta android-studio que foi criada:  
  
```cd /usr/local/android-studio/bin```  
  
Execute o código a seguir para instalar:  
  
```./studio.sh```  
  
Depois disso é só instalar de acordo com as suas preferências.  
  
## 4. Adicionando ao launcher
Para criar um "atalho" do Android Studio permitindo que seja possível acessá-lo através do buscador de programas, entre no Android Studio e crie um projeto, depois vá em Tools (no menu superior) e clique em "Create desktop entry" ou algo parecido com isso. Pronto, está feito, um arquivo chamado **jetbrains-studio.desktop** foi adicionado ao /usr/share/applications.
  
## 5. Adicionando à Área de Trabalho
Depois de ter adicionado ao launcher, para adicionar à Área de Trabalho, execute os seguintes códigos:  
  
```sudo chmod +x /usr/share/applications/jetbrains-studio.desktop```  
  
Depois esse código:  
  
```cp /usr/share/applications/jetbrains-studio.desktop ~/Área\ de\ Trabalho/```  
  
Espero que tenha sido útil.
