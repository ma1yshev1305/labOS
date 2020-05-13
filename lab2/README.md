# Лабораторная работа номер 2
**В рамках этой лабораторной работы были использованы:** <br>
| Тип диска  | Количество | Объем |
|:----------:|:---------:|:-----:|
| ssd | 2 | 5G | 
| ssd | 2 | 6.3G| 
| hdd | 2 | 10G |

**Part #1**  
Создаем виртуальную машину, накатываем туда deian 10.3, доходим до раздела "разметка дисков" и начинаем выполение нашей лабораторной работы.    

![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/1.1.png)  
первое разделение дисков.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/1.2.png)  
указание места для RAID.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/1.3.png)  
настроиваем RAID.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/1.4.png)  
начало установки и настройки LVM.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/1.5.png)  
середина настройки LVM.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/1.6.png)  
конечная настройка и установка LVM.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/1.7.png)  
результат настройки и установки LVM.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/1.8.png)  
установка GRUB на первый диск (sda).  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/1.9.png)  
первая информация о дисках.    
  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/1.10.png)  
первая информация о RAID.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/1.11.png)  
первая информация о pvs, vgs, lvs.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/1.12.png)  
  
**Part #2**  
По заданию отключается один SSD,по заданию мы заменяем его и с помощью LVM сохраняем все данные и копируем на новый диск.  
  
реакция ос на удаление ssd1.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/2.1.png)  
виртуальная машина работает.  

![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/2.2.png)  
проверка статуса RAID после удаление sdd1.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/2.3.png)  
добавление в RAID ssd3.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/2.5.png)
результат в mdstat.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/2.6.png)  
результат задания №2.  
  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/2.7.png)  

**Part #3**  
 В этой части по заданию отключается еще один SSD, мы заменяем его на новый sdd на 7 gb и добавляем 2 новых HDD.  
С помощью LVM и RAID спасаем данные и включаем новый SSD в VG.  
информация о дисках после удаления ssd2.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.1.png)  
информация в mdstat после удаления ssd2.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.2.png)  
информация после добавления ssd4.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.3.png)  
информация после копирования файлов в таблицу на ssd4.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.4.png)  
информация после монтирования boot на ssd4.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.5.png)  
информация после создания нового RAID массива.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.6.png)  
изменение pvs до и после создания нового zip тома.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.7.png)  
информация о дисках после создания zip тома.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.8.png)  
var, root, var находятся на md0.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.9.png)  
результаты после перемещения LV.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.10.png)  
информация о дисках только после добавления всех новых.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.11.png)  
информация о дисках после копирования таблицы файлов и sda1.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.12.png)  
информация после добавления ssd5 в RAID и увеличения размеров на общих дисках.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.13.png)  
размер  sda(e)2=md127.  

![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.14.png)  
размер VG увеличился.  

![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.15.png)  
информация об увеличении размеров root и var.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.16.png)  
конечный результат работы с ssd.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.17.png)  
информация о дисках после создания логического тома.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.18.png)  
информация о дисках после форматирования разделов.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.19.png)  
информация о дисках после переформатирования var-логов.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.20.png)  
изменение файла fstab.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.21.png)  
последняя проверка pvs, lvs, vgs.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.22.png)  
послежняя проверка и информация о дисках.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.23.png)  
последняя информация о RAID.  
![Изображение](https://raw.githubusercontent.com/ma1yshev1305/labOS/master/lab2/screenshot/3.24.png)  
