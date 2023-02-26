1. Log into ieng6
<img width="496" alt="截屏2023-02-25 下午5 10 29" src="https://user-images.githubusercontent.com/122562034/221386902-5ad7be0f-831c-4fd1-bf3f-3f3130f1add7.png">

```
Key Pressed: Ctrl-C，Ctrl-V, <enter>

```
Because I have copied "ssh  cs15lwi23aqz@ieng6.ucsd.edu", and I don't need to enter the password as I have set up SSH keys. 
The login page is:

<img width="563" alt="截屏2023-02-25 下午5 13 22" src="https://user-images.githubusercontent.com/122562034/221386968-fab96068-b6f4-46fa-b173-f05f6ba9bc92.png">

2. Clone your fork of the repository from your Github account
<img width="621" alt="截屏2023-02-25 下午5 14 16" src="https://user-images.githubusercontent.com/122562034/221386981-c95237a7-1faf-47bd-b998-aab8c1424113.png">

```
Key Pressed: Ctrl-C，Ctrl-V, <enter>
```

Because I copied the git clone SSH, and I just need to pasted it. 
  
  
3. Run the tests, demonstrating that they fail
 <img width="614" alt="截屏2023-02-25 下午5 16 03" src="https://user-images.githubusercontent.com/122562034/221387029-3d324d7e-fc49-4fe8-bbb6-93874423864e.png">
 
```
Key Pressed: Ctrl-C，Ctrl-V, <enter>, Ctrl-C，Ctrl-V <enter>
```

  
4. Edit the code file to fix the failing test
<img width="772" alt="截屏2023-02-25 下午5 17 54" src="https://user-images.githubusercontent.com/122562034/221387073-6b9da65d-433b-4357-b8b0-c4202eba25eb.png">
  
```
Key entered: nano List<tab>
```

I have the entered the first couple of letters of the filename, and use tab to complete the whole name, And then edit the code by changing the "index1+=1" to "index2+=1"

 5. Run the tests, demonstrating that they now succeed
 <img width="787" alt="截屏2023-02-25 下午5 18 22" src="https://user-images.githubusercontent.com/122562034/221387086-8a394041-ef7c-41a9-a6b9-6d9df3604369.png">

```
Key Pressed:  <up><up><up><enter> <up><up><up><enter>
```  
  
Because I have the javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java 3 up in my history.So I use arrow to access it
java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples 3 up in my history.

6. Commit and push the resulting change to your Github account
  <img width="772" alt="截屏2023-02-25 下午5 19 09" src="https://user-images.githubusercontent.com/122562034/221387100-56fdbea5-6355-43c2-98aa-583d92633960.png">
<img width="706" alt="截屏2023-02-25 下午5 19 36" src="https://user-images.githubusercontent.com/122562034/221387113-02c5d422-0c3d-4476-a13c-e3f2c9bb288f.png">
Key Entered: 1. git add ListExamples.java <enter>
             2. git commit-m"Updated"<enter>
             3. git push <enter>
              
