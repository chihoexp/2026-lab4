# Отчет по лабораторной работе №4
**Тема:** STP
**Выполнил:** Кочеров Евгений, Денисенко Максим, Зеленцова Варвара. гр. 539  

## Топология

![Alt text](image-12.png)

## Ответы на вопросы

1. SW1 рутовый т.к у него меньше priority ![Alt text](image-13.png)
2. 
```
configure terminal
spanning-tree mode rapid-pvst
end
copy running-config startup-config
```
3. STP работает в rapid-pvst ![Alt text](image-3.png)
4. SW1![Alt text](image-4.png)
SW2![Alt text](image-5.png)
SW3![Alt text](image-6.png)
5. FastEthernet 0/1
Root Path Cost — наименьшая
При равенстве — Bridge ID вышестоящего коммутатора — наименьший
При равенстве — Port ID вышестоящего — наименьший
При равенстве — локальный Port ID — наименьший
6. Для VLAN 10 - SW1 Fa0/2,
для VLAN 20 - Fa0/3,.
Для VLAN 1 корневой порт определяется стандартным сравнением стоимости пути.
![Alt text](image-8.png)
7.  ![Alt text](image-9.png) чтобы перевести магистральный интерфейс в режим Portfast - spanning-tree portfast trunk
8.  ![Alt text](image-10.png) интерфейс работает исправно
9.  ![Alt text](image-11.png) Нету никаких интерфейсов