# Git cheat sheet

## Работа без веток

1. *git init* - команда инициализации локального репозитория

1. **git status** - команда отображения состояния файлов в рабочей директории(папки) и индексе

1. ***git add*** - команда добавления содержимого рабочей директории(папки) в индекс для последующего **commit**'а

    * git commit - команда для сохранения состояния рабочей директории(папки) из индекса

    * git log - командна для просмотра истории **commit**'ов

    * **git diff - команда, сравнивающая разные состояния системы, commit'ы**  
## Работа с ветками

1. **git branch <new_branch>** - команда, создающая новую ветку в текущем репозитории ,где **<new_branch>** - название новой ветки

    при создании новой ветки, с помощью вышеуказанной команды, указатель HEAD не перемещается на новую ветку. в свою очередь укзаатель HEAD указывает на наше местоположение в древе.

    **git checkout <branch_or_commit_name>** - команда, позволяющая пемещать указатель HEAD в древе между ветками, коммитами и файлами(с файлами ещё не разобрался)

    **git merge <shown_branch>** использует для слияния указанной(**<shown_branch**>) ветки в текущую 

    какая-то инфа о ветке

1. git push 

    **git push** используется для установления связи с удалённым репозиторием, вычисления локальных изменений отсутствующих в нём, и собственно их передачи в вышеупомянутый репозиторий. Этой команде нужно право на запись в репозиторий, поэтому она использует аутентификацию.

1. git pull 

**main** branch

святой рандом и проесвятой git, дай мне силы и команды создать кофликт при слиянии ветки main и ветки pull

**pull** branch

    **git pull** работает как комбинация команд git fetch и git merge, т. е. Git вначале забирает изменения из указанного удалённого репозитория, а затем пытается слить их с текущей веткой.

1. git fetch

    как я понял, чтобы создать конфликт (а далее, сделать так чтобы его не было, нужно НЕ ДЕЛАТЬ как указано ниже), необходимо выполнить последовательно следующие действия:

    1. закоммитить изменения в текущей ветке

    1. создать и перейти на новую ветку

    1. внести в новой ветке изменения и закоммитить их

    1. перейти в новую ветку, внести в неё изменения и закоммитить их

    1. слить ветки

    1. ???

    1. PROFIT

1. git remote 

  **git remote** служит для управления списком удалённых репозиториев. Она позволяет сохранять длинные URL репозиториев в виде понятных коротких строк, например «origin», так что нам не придётся забивать голову всякой ерундой и набирать её каждый раз для связи с сервером. Мы можем использовать несколько удалённых репозиториев для работы и **git remote** поможет добавлять, изменять и удалять их.

Практичеки всегда команда имеет вид 

    git remote add <имя> <url>

   **git fetch** связывается с удалённым репозиторием и забирает из него все изменения, которых у вас пока нет и сохраняет их локально.

<details>
    <summary>Бонус</summary>Рецепт коктейля ***Рекурсивный***

* 40 мл рома 
* 100 мл колы 
* 50 мл коктейля ***Рекурсивный***
</details>
