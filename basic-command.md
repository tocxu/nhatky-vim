#Review
Đại khái là một tool dùng để exit file text trong ubuntu, giống vi/nano/..

Theo ý kiển chủ quan là tổng hợp ưu điểm của mấy cái trên và dễ dùng+thuận tiện. Cái chính nữa là mn chỗ mình làm dùng nó là chính :v
#Command line
Để biết nhiều hơn về vim có thể sử dụng: 
> vimtutor

##1.1 Moving the cursor (di chuyển con trỏ)
* h: left
* j: right
* k: up
* l: down
##1.2 Exit vim 
> <ESC> --> :q! <Enter> // trash all changes

> <ESC> --> :wq <Enter> // save the changes

> x //delete the character at the cursor type

##1.3 Editing - insertion
press "i" 

or

press <insert> //insert before the cursor


press: A <Enter> //append after the line
> <ESC> to return Normal mode

##1.4 Deletion
> <x> //delete the unwanted character 

> type d$ //delete to the end of the line

other 
> d number motion

where:

d - is the delete operator

motion - is what the operator will operate on (listed below)

a short list of motions:
* w - until the start of the next word , EXCLUDING its first character * e - to the end of the current word, INCLUDING the last character 
* $ - to the end of the line, INCLUDING the last character 

number - to delete more

1. move the cursor to the first UPPER CASE word in the line marked

2. type d2w to delete the two UPPER CASE words 

to delete more line:

1. move the cursor to the first of the line

2. type		2dd	to delete two lines


##1.5 Using a count for a motion
Typing a number before a motion repeats it that many times.

1. move the cursor to the start of the line marked

2. type 	2w 	to move the cursor two words forward

3. type 	3e 	to move the cursor to the end of the third word forward

4. type 	0	to move to the start of the line

##1.6 Undo

Press 	u	to undo the last commands
	U	to fix a whole line
1. move the cursor to the line below marked ---> and place it on the first error

2. Type 	x 	to delete the first unmarted character 

3. Now type 	u 	to undo the last command executed

4. This time fix all the errors on the line using the x command

5. Now type a capital 	U	to return the line to its original state

6. Now type 	u	 a few times to undo the U and preceding commands

7. Now type 	CTRL-R	 a few times to redo the commands (undo the undo's)

##1.7 The Put command
* Type 	p	to put previously deleted text after the cursor
* Type	rx	to replace the character at the cursor with x
* to change util the end of a word, type	ce	

##1.8 More changes using c
the change operator is used with the same  motions as delete
c [number] motion

the motion are the same, such as w (word ) and $ (end of line)

##1.9 Cursor location and file status
type CTRL-G to show your location in the file and the file status

type G to move to a line in the file

1. Hold down the Ctrl key and press g. We call this CTRL-G. A mesage will appear at the bottom of the page with the file name and the position in the file. Remember the line number for step 3

2. press	G	to move you to the bottom of the file

3. press 	gg	to move you to the start of the file

##1.10 Search && Matching parentheses search
Type 	/ 	followed by a phrase to search for the phrase 

Type 	%	to find a matching ), ], or } 

1. Place the cursor on any (, [, or { in the line bellow marked --->

2. now type the % character 

3. the cursor will move to the matching parenthesis or bracket

4. type 	%	 to move the cursor to the other matching bracket 

5. move the cursor to another (,),[,], {or} and see what % does





