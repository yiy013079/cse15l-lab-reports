Installing VScode: Go to Visual Code studio website  https://code.visualstudio.com/, and choose the right version for your computer system. 
Screenshot: ![Image](https://github.com/yiy013079/cse15l-lab-reports/blob/main/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8A%E5%8D%8811.11.28.png)

Remotely Connecting: First find your account name and change your passwords through this link: https://sdacs.ucsd.edu/~icc/index.php
After you successfully reset your password, you need to wait a few minutes for it to take effect.
Then open terminal in your visual code studio, and type ssh  <your username>@ieng6.ucsd.edu
Screenshot:![Image](https://github.com/yiy013079/cse15l-lab-reports/blob/main/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8A%E5%8D%8811.19.29.png)
After you type in your password, it will show:
![Image](https://github.com/yiy013079/cse15l-lab-reports/blob/main/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8A%E5%8D%8811.20.11.png)
That means you have successfully connected remotely

Trying Some Commands: If you want to try some commends. You can type in the following commend in the terminal:
cd ~
cd
ls -lat
ls -a
ls <directory> where <directory> is /home/linux/ieng6/cs15lwi23/cs15lwi23abc, where the abc is one of the other group members’ username
cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/
cat /home/linux/ieng6/cs15lwi23/public/hello.txt
Something like this will show:
![Image](https://github.com/yiy013079/cse15l-lab-reports/blob/main/%E6%88%AA%E5%B1%8F2023-01-12%20%E4%B8%8A%E5%8D%8811.23.30.png)



