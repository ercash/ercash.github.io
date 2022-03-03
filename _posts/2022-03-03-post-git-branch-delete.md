---
title: "Проектеги кереги жок алыскы (remote) жана жергиликтүү (local) branch-ты өчүрүп салуу."
date: 2020-03-03T10:52:00-00:00
categories:
  - git-commands
tags:
  - git delete
---

**Кырдаал**: 
Кээ бир учурда branch-ты негизки (master) branch-ка бириктийбей эле өчүрүп салыш керек болуп калат. Бирок биздин branch алысты git-те дагы киргизилген (commit).
Ушуна кандай жол менен өчүрүп салуу керек бул жерде карап чыгабыз.

**Чечүү жолу**:
Биз branch-ты 2 жолу өчүрүшүбүз керек болот. Бул деген жергиликтүү жана алыскы branch-ты. 

*Кыскача жолу:*

1. Жергиликтүү өчүрүү:
`git branch -d <branchname>`

Мисалы: `git branch -d testingBranch`

2. Алыскы branch-ты өчүрүү:
`git push -d <remote-name> <branchname>`

Мисалы: `git push -d origin testingBranch`

кээ бир учурда `<remote-name>` бул  `origin` болушу мүмкүн.

*Кенерирээк жолу:*

TODO: