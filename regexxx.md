# ^https:\/\/[a-z]+.fptu-ech.io$
Khi đọc ta thấy [a-z]+ tức là các kí tự từ a đến z không giới hạn độ dài

![image](https://github.com/NamDT5125/regex/assets/69895129/6abf58f1-d968-4da8-8290-4dac30a9741e)

# ^[+-]?((\d+(\.\d*)?)|(\.\d+))$
Dấu + hoặc - có thể có hoặc không, phải có số (có thể có dấu . và số đằng sau) hoặc dấu . và số đằng sau

![image](https://github.com/NamDT5125/regex/assets/69895129/33baee7f-fc2a-4ec1-b497-6da3625ce65f)

# ^[0-9a-fA-F]+$
Lấy các kí tự từ 0 đến 9 hoặc a đến f hoặc A đến F và độ dài bất kì

![image](https://github.com/NamDT5125/regex/assets/69895129/ad4a7a21-eca0-49cc-a196-2ac7afd664d9)

# ^(((0?[1-9]|1[012])\/(0?[1-9]|1\d|2[0-8])|(0?[13456789]|1[012])\/(29|30)|(0?[13578]|1[02])\/31)\/(19|[2-9]\d)\d{2}|0?2\/29\/((19|[2-9]\d)(0[48]|[2468][048]|[13579][26])|(([2468][048]|[3579][26])00)))$
Cái này dùng để xét ngày, tháng/ngày/năm, đầu tiên là tháng từ 1 đến 9 hoặc có thể ghi là 01 đến 09 và 10 đến 12,sau đó là /, từ 0 đến 9, có thể có 0 ở trước, 1 và 1 số bất kì(10 đến 19), 20 đến 28, sao đó là dấu hoặc, trừ tháng 2 ra, các tháng đều có ngày 29 và 30, với tháng 13578 10 12 có 31 ngày, sau đó là / bắt đầu từ năm 1920 đến 9999
Tiếp theo là với tháng 2 có 29 ngày vào năm 19xx đến 99xx và xx là 04,08,[2468] ghép với [048] hoặc [13579] với [26](chia hết cho 4), hoặc các năm [2468][048] hoặc [3579][26] có đuôi 00

![image](https://github.com/NamDT5125/regex/assets/69895129/67ef4739-26f7-4db7-9cf5-d241d2b5c614)

# ^(([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])\.){3}([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])$
Cái này tìm số thỏa mãn điều kiện ([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5]) kèm theo . và lặp lại 3 lần, lần cuối cũng yêu cầu như kia nhưng không có .

![image](https://github.com/NamDT5125/regex/assets/69895129/f1de7936-99f3-4a92-a290-3f3c685df680)

# ^(0|\+84)(\s|\.)?((3[2-9])|(5[689])|(7[06-9])|(8[1-689])|(9[0-46-9]))(\d)(\s|\.)?(\d{3})(\s|\.)?(\d{3})$
Cái này yêu cầu form số điện thoại với +84 là Việt Nam và bị yêu cầu về 2 số đầu

![image](https://github.com/NamDT5125/regex/assets/69895129/b5c0122e-7b81-4a76-8c57-a3aea4ff3a9b)

# ^(?=.*[a-z])(?=.*[A-Z])(?=.*[0-9])(?=.*[!@#\$%\^&\*]).{8,}$
Cái này yêu cầu 1 chuỗi phải có ít nhất kí tự thường, viết hoa, số, kí tự thuộc !@#$%^&* và độ dài là 8 trở lên

![image](https://github.com/NamDT5125/regex/assets/69895129/1a111e24-59d0-4c12-90ad-6711c2201c3d)

# ^[^\s@]+@[^\s@]+\.[^\s@]+$
[^\s@] phủ định của khoảng trống và @, tức là lấy các kí tự ngoại trừ khoảng trống và @

![image](https://github.com/NamDT5125/regex/assets/69895129/dc501f32-4818-4dc7-bed2-987d1857857d)


