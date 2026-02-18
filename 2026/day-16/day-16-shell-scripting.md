**Task :- 1**

Code :-

#!/bin/bash 
echo "Hello, Devops!"

Result :-

Hello, Devops!

Note:- As shebang tells the computer which brain need to use to read our code.
With Shebang--- We are giving a specific instruction.Like "Hey computer, use Bash to read this."
Without Shebang--- We are leaving it up to the computer to guess. "hey computer, just do this somehow". as it is small code it maximum time it does not through any error , when the code will be little heavy and system unable to predict the brain, it will send error.


**Task :- 2**

Code: 1

#!/bin/bash

Name="Uttam"
Role="Devops Engineer"

echo "Hello, I am $Name and I am a $Role"

Result:
 Hello, I am Uttam and I am a Devops Engineer

 Code: 2

 #!/bin/bash

Name="Uttam"
Role="Devops Engineer"

echo 'Hello, I am $Name and I am a $Role'

Result:
 Hello, I am $Name and I am a $Role

 1.Double Quotes (" ")

 these are used for interpolation. They tell this shell: "Look inside these quotes and see if there are any variable or commands to run."
 > it treats special character like $ to variables

2. Single Quotes(' ')

   These are used for literal strings. they tell the shell: "Take everything inside here exactly as it is written. Do not change any thing."

   > result: echo 'Hi $name' prints Hi $name.


**Task :- 3**

Code:

#!/bin/bash


echo "Enter your name: "

read name

echo "Enter favorite tool: "

read tool

echo " Hello $name, your favorite toll is $tool."

Input :

name : Uttam
tool : Docker

Result : 

Hello Uttam, your favorite toll is Docker.

**Task :- 4**

1-->

#!/bin/bash

echo "Enter a Number: "
read num

if [ $num -gt 0 ]

then
        echo "Number is enter by you is Positive"

elif [ $num -lt 0 ]

then
        echo "Number is enter by you is negative"
else

   echo "Number is enter by you is zero"

fi

2-->

#!/bin/bash


read -p "Enter file name"  file_name


if [ -f "$file_name" ]

then
        echo "File is exist...."

else
        echo "File doesn't exist!!!"

fi


**Task :- 5**

#!/bin/bash


read -p "Enter ther service name: " service


read -p "Do you want to check the $service status(y/n) ?" choice


if [ "$choice" = "y" ]

then
        systemctl is-active --quiet $service

         if [ $? -eq 0 ]

        then
                echo "$service is Active "
        else
                echo "$sevice is not running"
        fi
else
        echo "skipped.."

fi




   
   


 




