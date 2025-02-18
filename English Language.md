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
![Screenshot (88)](https://github.com/user-attachments/assets/57bd0978-6577-4181-84ca-0c3b545e2d5c)

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
![Screenshot (90)](https://github.com/user-attachments/assets/a6a6b90f-32ed-4a10-9fa2-1b17eb047915)

## ITEM SETTING

#### Example Config when Limit and Amount are not different

```lua
local itemList = {
    --- id item to move, limit item per-storage, minimum item amount at bot backpack to move
    {id = {4584, 3004}, limit = 10000, amount = 200}
}
```
![Screenshot (92)](https://github.com/user-attachments/assets/a0264fec-8954-452c-9d93-f21d7d1a3361)

#### Example Config when Limit and Amount are different
```lua
local itemList = {
    --- id item to move, limit item per-storage, minimum item amount at bot backpack to move
    {id = {4584, 3004}, limit = 10000, amount = 200},
    {id = {4585, 3005}, limit = 5000, amount = 100},
    {id = {242}, limit = 1000, amount = 50}
}
```
![Screenshot (95)](https://github.com/user-attachments/assets/df24fbff-95eb-4b42-ab35-8bad0fedf73e)

## WEBHOOK SETTING

#### Make sure to change createNewMessageID = false to createNewMessageID = true if there are no 3 .txt files below 
![Screenshot (97)](https://github.com/user-attachments/assets/7119a3c0-72a0-4e85-a9b9-0a449774abc0)
![Screenshot (101)](https://github.com/user-attachments/assets/c769cbdf-34dc-4bed-afe6-c62a580fbcad)