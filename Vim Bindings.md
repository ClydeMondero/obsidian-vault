[[Vim]]

# Vim Bindings
#resource 

## Bindings Anatomy
**Command** > **Count** > **Motion**

## Modes
- Esc - normal mode 
- i - insert mode 
- a - insert mode (append)
- v - visual 
- : - command line 

## Motions
- h - move left
- j - move down
- k - move up
- l - move right

### Words
- w - start of the next word
- e - end of the next word

### Line
- 0 - start of the line
- _ - start of the first word of the line
- $ - end of the line

### Horizontal
- f - forward to the occurrence of the character/word
- F - backward to the occurrence of the character/word
- t - forward on top of the occurrence of the character/word
- T - backward on top of the occurrence of the character/word
- ; - forward 
- , - backward 

#### Page 
- CTRL + U - move up of the page
- CTRL + D - move down of the page

### Line Creation/Insertion
- I - insert at the start of a line
- A - append at the end of a line
- o - new line below
- O - new line above

### File 
- gg - go to start of the file
- G - go to end of the file

## Commands 

### Navigation
- CTRL + P - go up/previous 
- CTRIL + N - go down/next

### Selecting
- viC - C as character, selects the text inside the paired character
- vaC - C as character, selects the text and the paired character

### Saving and Exiting
- :q - quit
- :qa - quit all
- :q! - exit without saving
- :w - save
- :wq - save and exit

### Redo or Undo Changes
- u - undo
- CTRL + r - redo

### Delete 
- d - delete 
- dw - delete next word
- db - delete previous word 
- dd - delete whole line
- d0 - delete to the start of line
- d$ - delete to the end of line
- d#k - delete # line number up 
- d#j - delete # line number down
- dgg - delete to the start of the file
- dG -  to the end of the file . - repeats the last change 

### Change 
- c - change
- ciC - C as character, changes the text between the character 
- caC - C as character, changes the text and the character

### Erase and Replace
- x - erase character
- r - replace character
- :s/old/new - replace first occurrence
- :s/old/new/g - replaces first occurrence globally 
- :%s/old/new - replace all occurrence 

### Copy and Paste
- y - copy
- yw - copy  word
- yy - copy line
- y#k - copy # line number up 
- y#j - copy #  line number down
- p - paste

### Search  
- / - search
- n - next occurrence 
- N - previous  occurrence 
- % - Go to matching open
- CTRL + O - Go back 
- CTRL + I - Go Forward

### External Commands
- :! - use external commands
- :Ex - explore file
- :so - source file

### Buffer/Window
- CTRL + W - change window

### File 
- % - create file when in netrw
- d - create a directory