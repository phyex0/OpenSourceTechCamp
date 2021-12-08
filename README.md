# OpenSourceTechCamp
  Homework for the basic shell commands 
  
  Source of the questions : https://docs.liman.dev/sistem-yonetimi/temel-sistem-yonetimi/en-temel-komutlar
  
#Question 1: isim adlı bir değişlene bir isim tanımlanarak bunun ekrana yazdırılması

<code>
  
  name="Burak"
  
  echo $name
  
 </code>
 
 
#Question 2: isim ve soyisim değişkenleri tanımlanarak bunlara birer değeri verilmeli, bunların birleştirilmiş halleri bir kisi değişkenine eşitlenmeli ve kişi değişkeni ekrana yazdırılmalı.

  <code>
  
    name="Burak"
  
    surname="Yesildal"
  
    concatString="${name} ${surname}"
  
    echo $concat
  
  </code>
  
  
#Question 3: /home/ dizininde iken /etc/systemd/system dizinine tek komut ile gidilmeli.

  <code>
    cd /etc/systemd/
  </code>


  Sourcce of the quesitons : https://docs.liman.dev/sistem-yonetimi/temel-sistem-yonetimi/komut-nedir
  
  
#Question 1 : bash ve sh kabuklarının çevre değişkenlerini kıyaslama

  a) Bir uçbirim açın ve mevcut kabuğu ekrana yazdırın
  
    <code>
      echo $SHELL
    </code>
    
    
  b) bash kabuğuna geçerek çevre değişkenlerini ekrana yazdırın
  
    <code>
    
      cat /etc/shells
      
      chsh -s /bin/bash
      
      printenv
      
    </code>
    
    
  c) sh kabuğuna geçerek çevre değişkenlerini ekrana yazdırın
  
    <code>
      cat /etc/shells
      chsh -s /bin/sh
      printenv
    </code> 
    
    
#Question 2 : Python kabuğu üzerinde basit fonksiyon geliştirme

  a)Uçbirim üzerinde python kabuğu açılmalı, python kabuğu üzerinde fibo (fibınacci dizisi için) kütüphanesini içeri aktararak, dizinin ilk 10 sayısını döndüren 
  bir fonksiyon yazın.
  
  <code>
    nano fibo.py
    
    
           import sys

          def print_fibo(param):
              if param  <= 0:
                      print("Invalid paramter")
                      return

              list = []
              list.append(1)
              list.append(1)

              for i in range(param):
                      if i > 1:
                              list.append(list[i - 1] + list[i - 2])
                      print(list[i])

          if __name__ == "__main__":
                parameter = 10 #default value

                if len(sys.argv) > 1:
                        parameter = sys.argv[1]
          
                print_fibo(int(parameter)) 
    
   python3 fibo.py 10
    </code>
  
  
  
  #Question 3 : Kullanıcı bazlı değil, sistem genelinde kalıcı bir çevre değişkeni tanımlanmak istense, hangi sistem dosyası kullanılabilir.
  
    <code>
      export variable="value"
    </code>
  
  
  #Question 4 : Kullanıcı ana dizininde bulunan dosyalardan hangisi Bash geçmişini depolamak için kullanılır?
  
    <code>
      cat ~/.bash_history
  </code>
  
  
  
  
  
  
  
  
  
  
  
  
  
