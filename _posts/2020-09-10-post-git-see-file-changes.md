---
title: "Кантип git колдонуп бир эле файлдагы өзгөрүүлөрдү караса болот?"
date: 2020-09-10T13:45:00-00:00
categories:
  - git-commands
tags:
  - git
---

Кантип git колдонуп бир эле файлдагы өзгөрүүлөрдү караса болот?

Эгер git колдонуп бир эле файлдагы (мисалы катары файлды bishkek.txt деп атап коелу) өзгөрүүлөрдү караш керек болсо, git ар тараптуу командарды сунуштайт. 
Бул жерде ошолордун арасынан коп колдонулган командалар каралат.

## `git diff` командасы 

Бул команданын жардамы менен файлдагы акыркы өзгөрүүнү караса болот. Мисалы:

`git diff bishkek.txt`

Эгер файл бул жердеги папканын (мисал катары папканы kgz деп атап коелу) ичинде болсо, анда бул папка дагы көргөзүш керек болот:

`git diff kgz/bishkek.txt`

## `gitk` графикалык терезе 

gitk бул git озунун графикалык терезеси. Бул куралды колдонуп файлдагы өзгөрүүнү көрсөк болот:

`gitk bishkek.txt`

## `git difftool` графикалык терезе

difftool бул дагы озунчо графикалык терезе, бирок бул бирични git конфигурациясында көргөзүлүш керек, кайсы курал колдонулат.

`git difftool bishkek.txt`

Маалымат булагы:
* See changes to a specific file using git (https://stackoverflow.com/questions/8048584/see-changes-to-a-specific-file-using-git "See changes to a specific file using git")
* git-diff(1) Manual Page(http://schacon.github.io/git/git-diff.html "git-diff(1) Manual Page")
