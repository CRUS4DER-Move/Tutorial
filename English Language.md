# AUTO MOVE v0.2 TUTORIAL

## STORAGE

#### Example of World Writing that does not use File.txt
```lua
local storage = {
    take = {
        world = {'asfwa2g:asgsag2', 'awsgas:sagawg', 'safawg:xsagwag'},      
        useFile = {
            enabled = false,                                                 
            filePath = 'C:\\Users\\Administrator\\Desktop\\Lucifer\\take.txt'
        }
    },
    drop = {
        world = {'j21i412:askfkaw', 'ahwwab:asfkwg', 'awfsfas:kfhwakg'},     
        useFile = {
            enabled = false,                                                 
            filePath = 'C:\\Users\\Administrator\\Desktop\\Lucifer\\drop.txt'
        }
    }
}
```
![Screenshot (88)](https://github.com/user-attachments/assets/f9315968-bc2d-4ceb-b9e2-406184c57285)

#### Example of Using File.txt, Make Sure You Change enabled = false to enabled = true and Also Make Sure the File Location is Correct.
```lua
local storage = {
    take = {
        world = {'x:x', 'x:x', 'x:x'},      
        useFile = {
            enabled = true,                                                 
            filePath = 'C:\\Users\\Administrator\\Desktop\\Lucifer\\take.txt'
        }
    },
    drop = {
        world = {'x:x', 'x:x', 'x:x'},  
        useFile = {
            enabled = true,                                                 
            filePath = 'C:\\Users\\Administrator\\Desktop\\Lucifer\\drop.txt'
        }
    }
}
```
#### World Format in File.txt
![Screenshot (90)](https://github.com/user-attachments/assets/717da7d1-534f-4787-9c4c-21390fca9dd0)

## ITEM SETTING

#### Example Config when Limit and Amount are not different

```lua
local itemList = {
    --- id item to move, limit item per-storage, minimum item amount at bot backpack to move
    {id = {4584, 3004}, limit = 10000, amount = 200}
}
```
![Screenshot (92)](https://github.com/user-attachments/assets/fcb05cc7-a21c-419e-9a7a-43fc692d49d0)

#### Example Config when Limit and Amount are different
```lua
local itemList = {
    --- id item to move, limit item per-storage, minimum item amount at bot backpack to move
    {id = {4584, 3004}, limit = 10000, amount = 200},
    {id = {4585, 3005}, limit = 5000, amount = 100},
    {id = {242}, limit = 1000, amount = 50}
}
```
![Screenshot (95)](https://github.com/user-attachments/assets/4a273a60-3dfd-47d4-b523-8f4a83afc71c)

## WEBHOOK SETTING

#### Make sure to change createNewMessageID = false to createNewMessageID = true if there are no 3 .txt files below 
![Screenshot (97)](https://github.com/user-attachments/assets/159a37ec-1cfa-4195-adbf-8cf10909d9ff)

![Screenshot (101)](https://github.com/user-attachments/assets/29eccef2-9dad-4cc5-895e-86182634dd50)
