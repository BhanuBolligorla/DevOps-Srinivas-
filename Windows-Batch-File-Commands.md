## Basic Commands :

* **Display a Message :**

        echo Hello, World!
**Output :**

Hello, World!

* **Clear Screen :**

       cls

* **Display Current Directory Contents:**

       dir

* **Create a Directory :**

       md NewFolder

* **Change Directory:**

      cd NewFolder

* **Delete a File:**

      del file.txt

* **Copy a File:**

      copy file.txt D:\Backup

* **Check if a File Exists:**

      if exist file.txt echo File exists!

* **Get User Input:**

      set /p name=Enter your name: 
      echo Hello, %name%!

* **List Running Processes:**

      tasklist

* **Shutdown the Computer (in 60 seconds):**

      shutdown /s /t 60

* **Ping a Website:**

       ping google.com

* **Loop Through Files:**

      for %%f in (*.txt) do echo %%f
* **Loops:**

      for %%f IN (apple banana cherry) do echo %%f

**Output:**
   
   apple
   
   banana

   cherry

* **Numbers:**

      FOR /L %N IN (1 1 5) DO ECHO Number: %N

**Output:**

1

2

3

4

5










