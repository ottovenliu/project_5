<<<<<<< HEAD
使用 INSERT 指令新增一筆資料到 user 資料表中，這筆資料的 username 和password 欄位必須是 ply。接著繼續新增至少 4 筆隨意的資料。<br>
INSERT INTO table_name (name, username, password)
VALUES (游旻婷,游旻婷,123)(謝瑞蓮,小蓮花,456),(劉顓豪,阿豪,789),(GM,ply,ply),(劉建國,國哥);
使用 SELECT 指令取得所有在 user 資料表中的使用者資料。<br>
"select * from user;"<br>
![1](https://user-images.githubusercontent.com/76770643/112414860-c4e8d400-8d5d-11eb-8fdd-20735c34f9c2.JPG)

使用 SELECT 指令取得 user 資料表中總共有幾筆資料。<br>
select count(*) from user;<br>
![2](https://user-images.githubusercontent.com/76770643/112414864-c6b29780-8d5d-11eb-97d1-0ae63dc15291.JPG)

使用 SELECT 指令取得所有在 user 資料表中的使用者資料，並按照 time 欄位，由近到遠排序。<br>
select * from user<br>
    order by time desc;<br>
![3](https://user-images.githubusercontent.com/76770643/112414867-c74b2e00-8d5d-11eb-8983-bfb7d9d90f7b.JPG)

使用 SELECT 指令取得 user 資料表中第 2 ~ 4 共三筆資料，並按照 time 欄位，由近到遠排序。<br>
select * from user<br>
    order by time desc<br>
    limit 1,3;<br>
![4](https://user-images.githubusercontent.com/76770643/112414869-c7e3c480-8d5d-11eb-8553-6a4176085cf4.JPG)

使用 SELECT 指令取得欄位 username 是 ply 的使用者資料。<br>
select * from user<br>
    where username = 'ply';<br>
![5](https://user-images.githubusercontent.com/76770643/112414871-c87c5b00-8d5d-11eb-81db-b8ea90cbad2f.JPG)

使用 SELECT 指令取得欄位 username 是 ply、且欄位 password 也是 ply 的資料。<br>
select * from user<br>
    where username = 'ply'<br>
    and password = 'ply';<br>
![6](https://user-images.githubusercontent.com/76770643/112414874-c914f180-8d5d-11eb-99e0-ca756320a7b4.JPG)

使用 UPDATE 指令更新欄位 username 是 ply 的使用者資料，將資料中的 name 欄位改成【丁滿】。<br>
update user<br>
    set name = '丁滿'<br>
![7](https://user-images.githubusercontent.com/76770643/112414878-c9ad8800-8d5d-11eb-91f6-35bd13ce4005.JPG)

使用 DELETE 指令刪除所有在 user 資料表中的資料。<br>
![8](https://user-images.githubusercontent.com/76770643/112414879-cadeb500-8d5d-11eb-8c1b-75dca1f91232.JPG)

使用 SELECT 搭配 JOIN 的語法，取得所有留言，資料中須包含留言會員的姓名。
![option-1](https://user-images.githubusercontent.com/76770643/112507884-057e3700-8dca-11eb-93c4-f016522e8f54.JPG)

使用 SELECT 搭配 JOIN 的語法，取得 user 資料表中欄位 username 是 ply 的所有留言，資料中須包含留言會員的姓名。
![option-2](https://user-images.githubusercontent.com/76770643/112507922-0dd67200-8dca-11eb-9c4f-12ff8f2cc724.JPG)
