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
   


 




