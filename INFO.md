создаем файл file-feature-1.txt с помощью консоли: 
touch file-feature-1.txt создание файла
git add file-feature-1.txt добавление файла из working area в staging area
git commit -m "создан новый файл" сохраняем изменения из staging area в repositiry
git status проверяем статус изменений
git push публикуем выгружаемые локальные изменения в центральный репозиторий

vim file-feature-1.txt добавляем содержимое в файл с пом-ю этой команды
:qw enter выходим из режима ркдактирования файла
git add file-feature-1.txt добавляем файл
git status проверяем статус, видим, что нужно сделать commit
git commit -m "добавлена лекция по API"  сохранили изменения
git push 

       //Выдалась Ошибка(To https://github.com/Nadine915/SF.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Nadine915/SF.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
nadezda@MacBook-Pro-Nadezda SF % git fetch
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
From https://github.com/Nadine915/SF
   3dc7ce3..a0d39d3  main       -> origin/main
nadezda@MacBook-Pro-Nadezda SF % git push
To https://github.com/Nadine915/SF.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/Nadine915/SF.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
nadezda@MacBook-Pro-Nadezda SF % git pull
Merge made by the 'recursive' strategy.
 INFO.md | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)
nadezda@MacBook-Pro-Nadezda SF % git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean)//

git push 
git log

touch file-feature-2.txt добавляем новый файл
git add file-feature-2.txt
добавляем содержимое в файл file-feature-2.txt на локальной машине
вносим информацию в файл file-feature-1.txt 
git add file-feature-1.txt
git commit -m "добавили инфо по http запросам"
git add file-feature-2.txt
git commit -m "контрольное задание по гит"
touch file-feature-3.txt
git add file-feature-3.txt
git commit -m "новый файл"
git status
удаляем файл file-feature-1.txt
git rm file-feature-1.txt фиксируем удаление файла






 
