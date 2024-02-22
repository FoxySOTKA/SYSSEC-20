# Домашнее задание к занятию «Уязвимости и атаки на информационные системы»

## Выполнил Савицкий Андрей

### Задание 1

Скачайте и установите виртуальную машину Metasploitable: https://sourceforge.net/projects/metasploitable/.

Это типовая ОС для экспериментов в области информационной безопасности, с которой следует начать при анализе уязвимостей.

Просканируйте эту виртуальную машину, используя **nmap**.

Попробуйте найти уязвимости, которым подвержена эта виртуальная машина.

Сами уязвимости можно поискать на сайте https://www.exploit-db.com/.

Для этого нужно в поиске ввести название сетевой службы, обнаруженной на атакуемой машине, и выбрать подходящие по версии уязвимости.

Ответьте на следующие вопросы:

1) Какие сетевые службы в ней разрешены?
2) Какие уязвимости были вами обнаружены?
  
#### Ответ:
1) Список разрешенных служб:
```
PORT     STATE  SERVICE     VERSION
21/tcp   open   ftp         ProFTPD 1.3.5
22/tcp   open   ssh         OpenSSH 6.6.1p1 Ubuntu 2ubuntu2.13 (Ubuntu Linux; protocol 2.0)
80/tcp   open   http        Apache httpd 2.4.7
445/tcp  open               Samba smbd 4.3.11-Ubuntu (workgroup: WORKGROUP)
631/tcp  open   ipp         CUPS 1.7
3306/tcp open   mysql       MySQL (unauthorized)
8080/tcp open   http        Jetty 8.1.7.v20120910
```
2) Ссылки на обнаруженые уязвимости:
```
PORT     STATE  SERVICE     VERSION                                                         lINK
21/tcp   open   ftp         ProFTPD 1.3.5                                                   https://www.exploit-db.com/exploits/37262
22/tcp   open   ssh         OpenSSH 6.6.1p1 Ubuntu 2ubuntu2.13 (Ubuntu Linux; protocol 2.0) https://www.exploit-db.com/exploits/45233
445/tcp  open               Samba smbd 4.3.11-Ubuntu (workgroup: WORKGROUP)                 https://www.exploit-db.com/exploits/42084
```




---

### Задание 2

Проведите сканирование Metasploitable в режимах SYN, FIN, Xmas, UDP.

Запишите сеансы сканирования в Wireshark.

Ответьте на следующие вопросы:

- Чем отличаются эти режимы сканирования с точки зрения сетевого трафика?
- Как отвечает сервер?

#### Ответ:
-
-



---

