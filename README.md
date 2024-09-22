# GitBashCommands

### <a href="https://git-scm.com/downloads" target="_blank"> GIT-i Endirmək üçün klikləyin</a>
--------

### Git-in hansı versiyada olduğunu öyrənmək üçün: 
```git -v & git --version```
>:bulb:**Not:** CMD və GitBash-ın hər ikisində də bu command işləyir.
--------

### Git Repository-lər(.git file-ın yer aldığı folder-lər) daxilində edilən dəyişikliklərin(commit-lərin) hansı istifadəçi tərəfindən edildiyi məlumatlarının saxlanması üçün: 
```git config --global user.name “username”```

```git config --global user.email “email”```

>:bulb:**Not:** Qeyd etdiyimiz kimi --global keyword ilə biz informasiyaları sistemdə olan bütün Repository-lər üçün təyin edirik, Spesifik bir Repository üçün isə --global yazmadan bu command-ı işə salmalıyıq.
--------

### Unstaged mərhələsində olan fayllar(və ya folder) stage mərhələsinə göndərmək üçün:
```git add <fileName> ```
>:bulb:**Not:** Bu command vasitilə biz spesifik bir faylı(və ya folder) unstaged mərhələsindən stage mərhələsinə göndərmiş oluruq. Bütün edilmiş dəyişiklikləri göndərmək üçün (git add .) , spesifik extensiona sahib olan faylları göndərmək üçün isə (git add *.extension).

>:bulb:**Not:** Unstaged yəni track olunan lakin stage mərhələsinə göndərilməmiş faylların yer aldığı mərhələdir.
--------

### Stage mərhələsinə add olunmuş faylları(və ya folder) yenidən unstage mərhələsinə göndərmək üçün:
```git restore --staged <fileName>```

--------

### Stage mərhələsinə əlavə olunan local-daki dəyişiklikləri remote-a göndərmək üçün hazırlamaq və bu dəyişikliyi qısa izzah edərək rəy yazmaq üçün:
```git commit -m "message"```
>:bulb:**Not:** Bir neçə sətr rəy yazmaq üçün isə git commit -m "message1" -m "message2" 
--------

### Indiyədək local-da olan commit-ləri göstərmək üçün:
```git log```

--------

### Commit olunmuş dəyişiklikləri remote-a göndərmək üçün:
```git push```

--------


### Remote-da olan dəyişiklikləri Local-a gətirmək üçün:
```git pull```

--------












