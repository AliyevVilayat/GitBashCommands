# GitBash & Linux Commands

### <a href="https://git-scm.com/downloads" target="_blank"> GIT-i Endirmək üçün klikləyin</a>

--------
### Hazırdaki path-i əldə etmək üçün:
```pwd``` 
>:bulb:**Not:** pwd-in açılımı Print Working Directory-dir.

---------
### Hazırda olduğumuz folder daxilində yer alan folder-ə daxil olmaq üçün:
```cd <folderName> ```
>:bulb:**Not:** cd-in açılımı Change Directory-dir.

---------
### Hazırda olduğumuz folder-dən bir üst folder-ə qayıtmaq üçün:
```cd ..```
>:bulb:**Not:** Sadəcə cd command yazaraq olduğumuz path-dən aslılı olmayaraq User-ə qayıda bilərik.

---------
### Yeni folder yaratmaq üçün
```mkdir <folderName>```
>:bulb:**Not:** mkdir-in açılımı Make Directory-dir.

---------
### Yeni folder yaratdıqdan sonra bir başa o folder-ə keçid etmək üçün
```mkdir <folderName> && cd "$_"```
>:bulb:**Not:** Burada $_ sonuncu istifadə edilən arqumenti təmsil edir.

---------
### Verilən folder-i silmək üçün
```rmdir <folderName>``` və ya ```rm -d folderName>``` və ya ```rm --dir folderName>```

>:bulb:**Not:** Nəzərə alınmalıdır ki, bu əmr sadəcə daxili boş olan folder-ləri silmək üçün nəzərdə tutulmuşdur.

---------
### Hazırdaki folder daxilində fayl silmək üçün:
```rm <fileName>```
>:bulb:**Not:** Birdən çox fayl silmək üçün isə rm fileName1 fileName2 fileNameN şəklində command yazılmalıdır.

---------
### Hazırdaki folder daxilində sorğusuz şəkildə(force) fayl silmək üçün:
```rm -f <fileName>```

---------
### Verilən folder-i və onun daxilindəki fayları silmək üçün:
```rm -r <folderName>```

---------
### Hazırdaki folder daxilində sorğusuz şəkildə(force) folder silmək üçün:
```rm -rf <folderName>```

---------
### Git-in hansı versiyada olduğunu öyrənmək üçün: 
```git -v & git --version```

---------
### Git Repository-lər(.git file-ın yer aldığı folder-lər) daxilində edilən dəyişikliklərin(commit-lərin) hansı istifadəçi tərəfindən edildiyi məlumatlarının saxlanması üçün: 
```git config --global user.name “username”```

```git config --global user.email “email”```

>:bulb:**Not:** Qeyd etdiyimiz kimi --global keyword ilə biz informasiyaları sistemdə olan bütün Repository-lər üçün təyin edirik, Spesifik bir Repository üçün isə --global yazmadan bu command-ı işə salmalıyıq.

---------
### Unstaged mərhələsində olan fayllar(və ya folder) stage mərhələsinə göndərmək üçün:
```git add <fileName> ```
>:bulb:**Not:** Bu command vasitilə biz spesifik bir faylı(və ya folder) unstaged mərhələsindən stage mərhələsinə göndərmiş oluruq. Bütün edilmiş dəyişiklikləri göndərmək üçün (git add .) , spesifik extensiona sahib olan faylları göndərmək üçün isə (git add *.extension).

>:bulb:**Not:** Unstaged yəni track olunan lakin stage mərhələsinə göndərilməmiş faylların yer aldığı mərhələdir.

---------
### Stage mərhələsinə add olunmuş faylları(və ya folder) yenidən unstage mərhələsinə göndərmək üçün:
```git restore --staged <fileName>```

---------
### Stage mərhələsinə əlavə olunan local-daki dəyişiklikləri remote-a göndərmək üçün hazırlamaq və bu dəyişikliyi qısa izzah edərək rəy yazmaq üçün:
```git commit -m "message"```
>:bulb:**Not:** Bir neçə sətr rəy yazmaq üçün isə git commit -m "message1" -m "message2" 

---------
### Indiyədək local-da olan commit-ləri göstərmək üçün:
```git log```

---------
### Commit olunmuş dəyişiklikləri remote-a göndərmək üçün:
```git push```

---------
### Remote-da olan dəyişiklikləri Local-a gətirmək üçün:
```git pull```

--------




[Vilayat Aliyev](https://www.linkedin.com/in/vilayataliyev/)







