# AUTO MOVE v0.2 TUTORIAL

## STORAGE

#### Contoh Penulisan World yang tidak menggunakan File.txt
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
![Screenshot (88)](https://github.com/user-attachments/assets/27f52c28-e2be-4fd4-a2b7-e54a41ba955e)

#### Contoh Penggunaan File.txt, Pastikan Kamu Mengubah enabled = false Menjadi enabled = true dan Pastikan Juga Lokasi Filenya Sesuai.
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
#### Format World didalam File.txt
![Screenshot (90)](https://github.com/user-attachments/assets/ed931caf-175f-4800-8b72-6c869e38ccb0)


## ITEM SETTING

#### Contoh Config ketika Limit dan Amount tidak berbeda

```lua
local itemList = {
    --- id item to move, limit item per-storage, minimum item amount at bot backpack to move
    {id = {4584, 3004}, limit = 10000, amount = 200}
}
```
![Screenshot (92)](https://github.com/user-attachments/assets/610ba9c7-1845-49b6-83db-87871ddd13a8)

#### Contoh Config ketika Limit dan Amount berbeda
```lua
local itemList = {
    --- id item to move, limit item per-storage, minimum item amount at bot backpack to move
    {id = {4584, 3004}, limit = 10000, amount = 200},
    {id = {4585, 3005}, limit = 5000, amount = 100},
    {id = {242}, limit = 1000, amount = 50}
}
```
![Screenshot (95)](https://github.com/user-attachments/assets/dd743e57-d871-442c-9ed0-877c1f0aa8ef)

## WEBHOOK SETTING

#### Pastikan untuk mengubah createNewMessageID = false Menjadi createNewMessageID = true Jika Tidak Ada 3 File.txt dibawah ini 
![Screenshot (97)](https://github.com/user-attachments/assets/78dcfd50-92a4-462b-8ee3-052312a2c926)

![Screenshot (101)](https://github.com/user-attachments/assets/1bcb5733-9d72-48c2-a054-74780696f3cb)
