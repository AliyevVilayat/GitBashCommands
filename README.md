# Linux Commands

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
### Hazırda olduğumuz folder daxilindəki folder və fayl-lar haqqında məlumat almaq üçün:
```dir və ya ls```
>:bulb:**Not:** ls -l (long listing format) vasitəsi ilə biz folder və fayllar barəsində daha ətraflı məlumat əldə edə bilərik.

>:bulb:**Not:** ls -h (human readable) vasitəsi ilə biz folder və faylların ölçüləri haqqında məlumatı KB,MB,GB və s. şəklində əldə edə bilərik.

>:bulb:**Not:** ls -a (all) vasitəsi ilə biz gizli fayllar da daxil olmaqla bütün folder və fayllar haqqında məlumat əldə edə bilərik.

>:bulb:**Not:** ls -R (recursive) vasitəsi ilə biz folder-lərin hər birinin özlərinin də daxilində yer alan folder və fayllar daxil olmaqla bütün folder və fayllar haqqında məlumat əldə edə bilərik.

>:bulb:**Not:** ls -r (reverse) vasitəsi ilə biz folder və fayllar haqqında məlumatlar sılamasını əks istiqamətdə əldə edə bilərik.

---------
### Yeni folder yaratmaq üçün:
```mkdir <folderName>```
>:bulb:**Not:** mkdir-in açılımı Make Directory-dir.

---------
### Yeni folder yaratdıqdan sonra bir başa o folder-ə keçid etmək üçün:
```mkdir <folderName> && cd "$_"```
>:bulb:**Not:** Burada $_ sonuncu istifadə edilən arqumenti təmsil edir.

---------
### Ekrana yazı çıxarmaq üçün:
```printf <text> və ya echo <text>```

---------
### Yeni file yaratmaq üçün:
```> <fileName>.extension```
>:bulb:**Not:** Əgər həmin adda bir fayl mövcuddursa içindəkiləri siləcək.

---------
### Yeni file yaratmaq üçün:
```touch <fileName>.extension```
>:bulb:**Not:** Uzantısını özümüz təyin edərək fayl yaradırıq. Əgər həmin adda bir fayl mövcuddursa sadəcə modified date dəyişiləcək, fayl daxili olduğu kimi qalacaq.

---------
### Yeni file yaratmaq üçün:
```echo > <fileName>.extension```
>:bulb:**Not:** Belə bir fayl mövcud deyilsə, fayl yaradır. Əks təqdirdə həmin fayl daxilini təmizləyərək daxilini boşaldır.

---------
### Yeni file yaratmaq və daxilinə yazı yazmaq üçün:
```echo <text> > <fileName>.extension```
>:bulb:**Not:** Belə bir fayl mövcud deyilsə, fayl yaradır və daxilində bizim vermiş olduğumuz text-i yazır. Əks təqdirdə həmin fayl daxilini təmizləyərək bizim text-i ora əlavə edir.

>:bulb:**Not:** Əgər biz mövcud fayla yazı yazdırmaq istəsək bu zaman > operatoru əvəzinə >> operatoru istifadə edəcəyik.

---------
### Yeni file yaratmaq üçün:
```cat > <fileName>.extension```
>:bulb:**Not:** Fayl daxilində yazı yazmaq üçün terminal açılacaq və işimizi bitirdikdən sonra CTRL + D edərək prosesi dayandıra bilərik.

---------
### File daxilindəki bütün yazıları əldə etmək üçün:
```cat <fileName>.extension```

---------
### File daxilindəki yazıları səhifə-səhifə əldə etmək üçün:
```less <fileName>.extension```
>:bulb:**Not:** Less əmri istifadəsi zamanı aşağı və yuxarı ox düymələri ilə səhifələr arası keçid mümkündür. q ilə açılan terminaldan çıxış edirik.

---------
### File daxilindəki yazılardan ilk 10 sətri əldə etmək üçün:
```head <fileName>.extension```
>:bulb:**Not:** Əgər daha çox sətr göstərmək istəsək, -n <count> yazaraq bu əmri yenidən istifadə edəcəyik.

---------
### File daxilindəki yazılardan son 10 sətri əldə etmək üçün:
```tail <fileName>.extension```
>:bulb:**Not:** Əgər daha çox sətr göstərmək istəsək, -n <count> yazaraq bu əmri yenidən istifadə edəcəyik.

---------
### File daxilindəki hansısa string ifadəni axtarmaq üçün:
```grep <searchedString> <fileName>.extension```
>:bulb:**Not:** Nəticədə geriyə həmin sətrləri qaytaracaq.

---------
### Verilən folder-i silmək üçün:
```rmdir <folderName>``` və ya ```rm -d folderName>``` və ya ```rm --dir folderName>```

>:bulb:**Not:** Nəzərə alınmalıdır ki, bu əmr sadəcə daxili boş olan folder-ləri silmək üçün nəzərdə tutulmuşdur.

---------
### Verilmiş file-ı readonly etmək üçün:
```chmod -w <folderName>```
>:bulb:**Not:** Readonly olaraq təyin olunmuş fayl üzərində dəyişiklik etmək olmur.

---------
### Hazırdaki folder daxilində fayl silmək üçün:
```rm <fileName>```
>:bulb:**Not:** Birdən çox fayl silmək üçün isə rm fileName1 fileName2 fileNameN şəklində command yazılmalıdır.

---------
### Hazırdaki folder daxilində sorğusuz şəkildə(force) fayl silmək üçün:
```rm -f <fileName>```

---------
### Verilən folder-i və onun daxilindəki file-ları silmək üçün:
```rm -r <folderName>```

---------
### Verilən folder-i və onun daxilindəki file-ları hər dəfə sorğu(y/n) ilə silmək üçün:
```rm -ri <folderName>```

---------
### Hazırdaki folder daxilində sorğusuz şəkildə(force) folder silmək üçün:
```rm -rf <folderName>```


# GIT
---------
### Git-in hansı versiyada olduğunu öyrənmək üçün: 
```git -v & git --version```

---------
### Git Repository-lər(.git file-ın yer aldığı folder-lər) daxilində edilən dəyişikliklərin(commit-lərin) hansı istifadəçi tərəfindən edildiyi məlumatlarının saxlanması üçün: 
```git config --global user.name “username”```

```git config --global user.email “email”```

>:bulb:**Not:** Qeyd etdiyimiz kimi --global keyword ilə biz informasiyaları sistemdə olan bütün Repository-lər üçün təyin edirik, Spesifik bir Repository üçün isə --global yazmadan bu command-ı işə salmalıyıq.

---------
### Faylların vəziyyəti barəsində məlumat almaq üçün:
```git status ```
>:bulb:**Not:** Bu command vasitilə biz yeni əlavə olunmuş(izlənilməyən), dəyişiklik edilmiş lakin stage edilməmiş(unstaged), əlavə olunmuş və üzərində heçbir dəyişiklik edilməmiş fayllar, branch məlumatlarını gətirmiş oluruq.

>:bulb:**Not:** Git Workflow-da mərhələlər bu şəkildədir. İzlənilməyən(Untracked), Dəyişdirilmiş, amma stage edilməmiş fayl(unstaged), Commit edilməyə hazır(Staged) və local repository-ə yazılmış(commited) mərhələləri.

---------
###  üçün:
```git diff ```
>:bulb:**Not:** Bu command vasitilə biz . Git diff --staged

---------
### Unstaged mərhələsində olan file-lar(və ya folder) stage mərhələsinə göndərmək üçün:
```git add <fileName> ```
>:bulb:**Not:** Bu command vasitilə biz spesifik bir faylı(və ya folder) unstaged mərhələsindən stage mərhələsinə göndərmiş oluruq. Bütün edilmiş dəyişiklikləri göndərmək üçün (git add .) , spesifik extensiona sahib olan faylları göndərmək üçün isə (git add *.extension).

>:bulb:**Not:** Unstaged yəni track olunan lakin stage mərhələsinə göndərilməmiş faylların yer aldığı mərhələdir.

---------
### Stage mərhələsinə add olunmuş file-lar(və ya folder) yenidən unstage mərhələsinə göndərmək üçün:
```git restore --staged <fileName>```
>:bulb:**Not:** Əgər bu command-ı işə saldıqdan sonra işləmirsə bu deməkdir ki köhnə versiya git istifadə edilir. Yuxarıdaki prosesi həyata keçirmək üçün alternativ yol olaraq (git reset HEAD fileName) və ya (git reset HEAD .) istifadə edilir.

---------
### Stage mərhələsinə əlavə olunan local-daki dəyişiklikləri remote-a göndərmək üçün hazırlamaq, local repository-ə(commited mərhələ) göndərmək və bu dəyişikliyi qısa izzah edərək rəy yazmaq üçün:
```git commit -m "message"```
>:bulb:**Not:** Bir neçə sətr rəy yazmaq üçün isə git commit -m "message1" -m "message2" 

---------
### Indiyədək local-da olan commit-ləri göstərmək üçün:
```git log```
>:bulb:**Not:** Daha detaylı şəkildə məlumat almaq üçün (git log --patch)
>
---------
### Local repository-də Commit olunmuş dəyişiklikləri remote repository-ə göndərmək üçün:
```git push```

---------
### Remote-da olan repository-i Local-a gətirmək üçün:
```git clone <repositoryLink>```

---------
### Remote-da olan dəyişiklikləri Local-a gətirmək üçün:
```git pull```

--------
### Local-da olan branch-ləri gətirmək üçün:
```git branch```

--------
### Remote-da olan branch-ləri gətirmək üçün:
```git branch -r```

--------
### Həm local-da, həm də remote-da olan branch-ləri gətirmək üçün:
```git branch -a```

--------
### Hazırda local-da olduğumuz branch daxilində branch yaratmaq üçün:
```git branch <branchName>```

--------
### Branch-lar arası keçid etmək üçün:
```git checkout <branchName>```

--------
### Branch yaradan zaman bir başa həmin branch-a keçid etmək üçün:
```git checkout -b <branchName>```

--------
### Branch-i silmək üçün:
```git branch -d <branchName>```

---------
### Local repository-də yaranmış branch-i və üzərindəki dəyişikliyi remote repository-ə göndərmək üçün:
```git push origin <branchName>```
>:bulb:**Not:** Bu command nəticəsində branch-in hazırda remote-da çalışdığımız branch olduğunu bildirmir, sadəcə bu dəfəlik həmin branch-ə edilmiş dəyişikliklər göndərilir. Üzərində çalışdığımız branch-i git push -u origin <branchName> yazaraq bildiririk. Beləliklə bir sonraki push əməliyyatları həmin branch-ə olacaq.


[Vilayat Aliyev](https://www.linkedin.com/in/vilayataliyev/)



vim nano vi printf

git fetch --prune



