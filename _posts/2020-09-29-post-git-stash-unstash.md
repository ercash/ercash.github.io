---
title: "Проектеги өзгөрүүлөрдү, кандай кылып убактылуу жерге сактоо (git stash)"
date: 2020-09-29T15:15:00-00:00
categories:
  - git-commands
tags:
  - git stash
---

**Кырдаал**: 
Жергиликтүү (local) проект өзгөртүлдү, бирок алыскы (remote) өзгөртүүнү проекте кошуш керек болуп калды. `git sync` командасын чакырканда төмөнкү маалымат чыгып, проект жаныланбай жатат.
> Commit your changes or stash them before you can merge

**Чечүү жолу**:
Бул деген проект жергиликтүү өзгөргөн, анан өзгөргөн маалыматтар алыска киргизилген (git commit) эмес. Бул маселени чечүүнүн **үч жолу** бар:
*1. Өзгөрүүнү алыска киргизүү.*
Бул үчүн бул команданы колдонобуз:
`git commit -m "Bul jerge emne bolgon ozgoruu jonundo maalymat jaz"`

*2. Өзгөрүүнү убактылуу бир жерге сактоо.*
Же өзгөртүлгөн маалыматты алыска киргизгенге эртерээк болсо, дагы өзгөрүүлөр болушу мүмкүн болгондуктан, буларды убактылуу жайга сактап, анан кайра проект жанылангандан кийин, кайра айта кайтарып келебиз.

Өзгөрүүнү убактылуу жерге сактоо:
`git stash`

Алыскы өзгөртүүнү проектке жанылоо:
`git sync`

Эми кайра убактылуу сакталган өзгөртүүнү кайра кайтарып проекте алып келүү:
`git stash pop`

*3. Жергиликтүү өзгөрүүнү өчүрүп салуу:*

Өчүрүп салуунун эки жолу бар:
`git reset --hard`
`git checkout -t -f remote/branch`

**Bonus**: Бир эле файлдагы өзгөрүүнү өчүрүп салуу: 
`git checkout <filename>`

Маалымат булагы:
* How do I resolve git saying “Commit your changes or stash them before you can merge”? (https://stackoverflow.com/questions/15745045/how-do-i-resolve-git-saying-commit-your-changes-or-stash-them-before-you-can-me "How do I resolve git saying “Commit your changes or stash them before you can merge”?")
