# Сергей Есенин — Ты меня не любишь, не жалеешь

*Ты меня не любишь, не жалеешь,*

Разве я немного не красив?

Не смотря в лицо, от страсти млеешь,

Мне на плечи руки опустив.  


Молодая, с чувственным оскалом,

Я с тобой не нежен и не груб.

Расскажи мне, скольких ты ласкала?

Сколько рук ты помнишь? Сколько губ?  


Знаю я — они прошли, как тени,

Не коснувшись твоего огня,

Многим ты садилась на колени,

А теперь сидишь вот у меня.  


Пусть твои полузакрыты очи

И ты думаешь о ком-нибудь другом,

Я ведь сам люблю тебя не очень,

Утопая в дальнем дорогом.  


Этот пыл не называй судьбою,

Легкодумна вспыльчивая связь,—

Как случайно встретился с тобою,

Улыбнусь, спокойно разойдясь.  


Да и ты пойдешь своей дорогой

Распылять безрадостные дни,

Только нецелованных не трогай,

Только негоревших не мани.  


И когда с другим по переулку

Ты пойдешь, болтая про любовь,

Может быть, я выйду на прогулку,

И с тобою встретимся мы вновь.  


Отвернув к другому ближе плечи

И немного наклонившись вниз,

Ты мне скажешь тихо: «Добрый вечер…»

Я отвечу: «Добрый вечер, miss».  


И ничто души не потревожит,

И ничто ее не бросит в дрожь,—

Кто любил, уж тот любить не может,

Кто сгорел, того не подожжешь.  


```
bes@bes-virtualbox:~$ echo $PWD

/home/bes

bes@bes-virtualbox:~$ cd projects

bes@bes-virtualbox:~/projects$ cd project1/

bes@bes-virtualbox:~/projects/project1$ ls -la

итого 12

drwxr-xr-x 3 bes bes 4096 сен 10 01:25 .

drwxr-xr-x 3 bes bes 4096 сен 10 01:24 ..

drwxr-xr-x 8 bes bes 4096 сен 10 01:31 .git

-rw-r--r-- 1 bes bes    0 сен 10 01:25 README.md

bes@bes-virtualbox:~/projects/project1$ git remote add origin git@github.com:bes91100/repository_dz.git

error: внешний репозиторий origin уже существует

bes@bes-virtualbox:~/projects/project1$ git push origin main

The authenticity of host 'github.com (140.82.121.4)' can't be established.

ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.

This key is not known by any other names.

Are you sure you want to continue connecting (yes/no/[fingerprint])? yes

Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.

git@github.com: Permission denied (publickey).

fatal: Не удалось прочитать из внешнего репозитория.

Удостоверьтесь, что у вас есть необходимые права доступа
и репозиторий существует.

bes@bes-virtualbox:~/projects/project1$ ssh-keygen -t ed25519

Generating public/private ed25519 key pair.

Enter file in which to save the key (/home/bes/.ssh/id_ed25519): /home/m/.ssh/linux^[[D^[[D^[[D^[[D^[[D^[[D^[[D^[[D^[[D^[[D^[[D^[[D^[[D^Z

[1]+  Остановлен    ssh-keygen -t ed25519

bes@bes-virtualbox:~/projects/project1$ ssh-keygen -t ed25519

Generating public/private ed25519 key pair.

Enter file in which to save the key (/home/bes/.ssh/id_ed25519): /home/bes/.ssh/linux_project_dz

Enter passphrase (empty for no passphrase): 

Enter same passphrase again: 

Your identification has been saved in /home/bes/.ssh/linux_project_dz

Your public key has been saved in /home/bes/.ssh/linux_project_dz.pub

The key fingerprint is:

SHA256:mbdaUyGPIYKuu2ehVnL0ReCY9HP18D1c3/9RUplT5UI bes@bes-virtualbox

The key's randomart image is:

+--[ED25519 256]--+

|    . ..  o   E X|

|   . *  .. + + Bo|

|    + =.o o + * *|

|   ..  +.+ = . +o|

|   ... .S o o  ..|

|  ..+ .  . o    o|

|  .= .    +     .|

|  o.o    o .     |

| .o+    .        |

+----[SHA256]-----+

bes@bes-virtualbox:~/projects/project1$ ls ~/.ssh -la

итого 20

drwx------  2 bes bes 4096 сен 10 01:41 .

drwxr-xr-x 17 bes bes 4096 сен 10 01:38 ..

-rw-r--r--  1 bes bes  142 сен 10 01:38 known_hosts

-rw-------  1 bes bes  411 сен 10 01:41 linux_project_dz

-rw-r--r--  1 bes bes  100 сен 10 01:41 linux_project_dz.pub

bes@bes-virtualbox:~/projects/project1$ cat ~/.ssh/linux_project_dz.pub 

ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIDGuxAyKujYUQtRG/tNdMYmrAspP7RvPsgXmzPhNH2AI bes@bes-virtualbox

bes@bes-virtualbox:~/projects/project1$ cat ~/.ssh/linux_project_dz

bes@bes-virtualbox:~/projects/project1$ ^C

bes@bes-virtualbox:~/projects/project1$ cd ~/.ssh

bes@bes-virtualbox:~/.ssh$ touch config

bes@bes-virtualbox:~/.ssh$ ls -la

итого 20

drwx------  2 bes bes 4096 сен 10 01:47 .

drwxr-xr-x 17 bes bes 4096 сен 10 01:38 ..

-rw-r--r--  1 bes bes    0 сен 10 01:47 config

-rw-r--r--  1 bes bes  142 сен 10 01:38 known_hosts

-rw-------  1 bes bes  411 сен 10 01:41 linux_project_dz

-rw-r--r--  1 bes bes  100 сен 10 01:41 linux_project_dz.pub

bes@bes-virtualbox:~/.ssh$ nano config

bes@bes-virtualbox:~/.ssh$ cd ~/projects/project1/

bes@bes-virtualbox:~/projects/project1$ git push -u origin main

Перечисление объектов: 3, готово.

Подсчет объектов: 100% (3/3), готово.

Запись объектов: 100% (3/3), 200 байтов | 50.00 КиБ/с, готово.

Всего 3 (изменений 0), повторно использовано 0 (изменений 0), повторно использовано пакетов 0

To github.com:bes91100/repository_dz.git

 * [new branch]      main -> main
b

ranch 'main' set up to track 'origin/main'.

bes@bes-virtualbox:~/projects/project1$ 
```
