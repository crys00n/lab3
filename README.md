# Лабораторная работа 3
Итак, сначала я настроил виртуальную машину А с Ubuntu и обеспечил ей доступ в интернет.

![VirtualBoxVM_KtbZTiSv9Z](https://github.com/user-attachments/assets/f1e227ed-c5e2-46b1-b7c9-2f3880b3fdbd)
![VirtualBoxVM_X1xjW8wn1v](https://github.com/user-attachments/assets/70d56782-8c6b-4037-9977-e10807fdd921)

>На примере с [vk.ru](https://vk.ru/) видно, что пакеты передаются и принимаются, потерь нет.

Далее, с помощью *снимков* я клонировал машину А, чтобы было проще создать машины Б и В.

![VirtualBox_B1cyOrkv72](https://github.com/user-attachments/assets/92c51429-721b-46d7-980d-29e251b61a21)

## Работа с сетевым доступом
Чтобы обеспечить доступ от одних машин к другим, я создал NAT сеть.

![VirtualBox_WbFT824z0n](https://github.com/user-attachments/assets/3a0e4149-5fb0-46d2-9d30-eaf1ba1b66c9)

Для того, чтобы узнать IP-адреса каждой из машин, мне нужно было воспользоваться командой `ifconfig`.

Чтобы сделать это, я установил `net-tools`.

![VirtualBoxVM_3EGyOK00oi](https://github.com/user-attachments/assets/fd9db38e-9134-4143-9818-e85aa089fe24)

Ну а затем, я выполнил и само задание с сетевым доступом.

Организовал сетевой доступ из машины А в машину Б, из машины А в машину В, но запретил доступ из машины Б в машину В.

IP - адреса машин:

A - 10.0.2.15

Б - 10.0.2.4

В - 10.0.2.5

![J6Tt7DNyI9](https://github.com/user-attachments/assets/5c0e2d04-56b2-47ef-968d-a3c41079f429)

По потере пакетов видно, где доступ есть, а где он запрещён.
