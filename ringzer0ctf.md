##Time to learn x86 ASM & gdb
- Đầu tiên mở file bằng IDA

![image](https://github.com/leviiec/r-em/assets/128345171/4692777e-a2e8-428e-874b-8e56258e2f40)

- Thấy chuỗi ``Where is the flag?`` bấm vào thử mà nó chẳng có cái gì =)) Debug thử thì tự dưng có mấy chuỗi đổi màu ngộ nha :DD

![image](https://github.com/leviiec/r-em/assets/128345171/7fce679c-c9b3-4b6b-8681-388b03855d42)

- Thử chuyển các chuỗi hex này thành cái gì thử thui nào
- ``47414C46h`` ->``GALF`` ồ ra chữ ``FLAG`` in ngược nè. Mình suy đoán là những chuỗi này sẽ in ngược maybe
  ``47414C46h`` ->``GALF``->``FLAG``
  ``3930342Dh``->``904-``->``-409``
  ``32h``->``2``
  ``75393438h``->``u948``->``849u``
  ``6A326F69h``->``j2oi``->``io2j``
  ``66h``->``f``
  ``6A736C6Bh``->``jslk``->``klsj``
  ``6C6B34h``->``lk4``->``4kl``
- Ghép các chuỗi ta được flag: ``FLAG-4092849uio2jfklsj4kl``
