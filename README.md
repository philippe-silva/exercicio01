# exercicio01
Exercicio da aula de CI-CD

Letra A:
    echo 1 > arquivo.txt
    cat arquivo.txt
    2
Letra B:
    git add arquivo.txt
    git status
        philippe.silva@ARK-282940 MINGW64 /j/INFRAESTRUTURA/25 - Users/Philippe/MBA IMPACTA/CI-CD/exercicio01 (main)
        $ git status
            On branch main
            Your branch is up to date with 'origin/main'.      

            Changes to be committed:
            (use "git restore --staged <file>..." to unstage)
                new file:   arquivo.txt

Letra C:
    git commit -m "git add example - arquivo.txt"
        [main bc96c1c] git add example - arquivo.txt
        1 file changed, 1 insertion(+)
        create mode 100644 arquivo.txt

Letra D:
    cat arquivo.txt
    2

LETRA E:
    $ git diff
    warning: in the working copy of 'arquivo.txt', LF will be replaced by CRLF the next time Git touches it
    diff --git a/arquivo.txt b/arquivo.txt
    index 8a0f05e..0cfbf08 100644
    --- a/arquivo.txt
    +++ b/arquivo.txt
    @@ -1 +1 @@
    -01
    +2


Letra F:
    git add arquivo.txt
    git status
    On branch main
    Your branch is up to date with 'origin/main'.      

    Changes to be committed:
        (use "git restore --staged <file>..." to unstage)
            modified:   arquivo.txt

Letra G:
    git diff

Letra H:
    echo 03 > arquivo.txt

Letra I:
    git diff
    $ git diff
    warning: in the working copy of 'arquivo.txt', LF will be replaced by CRLF the next time Git touches it
    diff --git a/arquivo.txt b/arquivo.txt
    index 0cfbf08..75016ea 100644
    --- a/arquivo.txt
    +++ b/arquivo.txt
    @@ -1 +1 @@
    -2
    +3

LETRA J:
    git restore --stage arquivo.txt
    $ git status
        On branch main
        Your branch is up to date with 'origin/main'.

        Changes not staged for commit:
        (use "git add <file>..." to update what will be committed)
        (use "git restore <file>..." to discard changes in working directory)
            modified:   arquivo.txt

            no changes added to commit (use "git add" and/or "git commit -a")  


Letra K:
    $ git add arquivo.txt
    $ git commit -m "echo arquivo.txt"
    [main 1d49885] echo arquivo.txt
    1 file changed, 1 insertion(+), 1 deletion(-)

    $ git log
    commit 1d4988512e4398b6e63cf1d21276af8166bc39e4 (HEAD -> main)
    Author: Philippe Silva <philippe.silva@aluno.faculdadeimpacta.com.br>
    Date:   Mon Aug 5 20:19:17 2024 -0300

    echo arquivo.txt

    commit bc96c1c7f8aebb7fea65ef4536d20cc1e4e56ad2 (origin/main, origin/HEAD)
    Author: Philippe Silva <philippe.silva@aluno.faculdadeimpacta.com.br>
    Date:   Mon Aug 5 19:58:33 2024 -0300

    git add example - arquivo.txt

    commit 0fa1981e8203ad73aed691366e5a63cb5fc611b1
    Author: philippe-silva <philippe.silva@aluno.faculdadeimpacta.com.br>
    Date:   Mon Aug 5 19:28:36 2024 -0300

    Initial commit


Letra L:
    vi .gitignore
    *.txt
    

Letra M:
    $ git status
    On branch main
    Your branch is ahead of 'origin/main' by 1 commit.
    (use "git push" to publish your local commits)

    Untracked files:
    (use "git add <file>..." to include in what will be committed)
        .gitignore

    nothing added to commit but untracked files present (use "git add" to track)

