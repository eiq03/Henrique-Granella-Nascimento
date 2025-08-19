Git flow

Normalmente existem 3 "linhas do tempo" acontecendo em um codigo, a MAIN, Homologação e Develop

todas andam juntas, até o momento que outra funcionalidade entra na sequencia

Features, features são novas branchs apartir da develop, que server para o desenvolvedor pegar o codigo da develop (que esta atualizado) e realizar as alterações/implementações necessarias

para criar uma feature:
git checkout -b "nome da feature" - aqui dentro da feature vc pode commitar e adicionar o quanto de codigo vc quiser
para adicionar suas implementações vc envia uma requisição de pull - pull request

caso tenham sido criadas 2 features em tempo proximo e uma dessas ja esta mergeada na main, (foi realizado um pull request anteriormente) caso vc se encontre nesse caso, vc n deve dar um pull request, vc deve puxar as modificações causadas pela outra feature para tua, usando o GIT FETCH ou GIT MERGE DEVELOP, se der conflito, vc deixa a develop passar por cima da tua alteração.

CASO USE O MERGE ele puxa as info da develop para a feature, e ele faz um commit automatico pra deixar as alterações "marcadas"
polui o historico da branch, mas depende da empresa

usando o GIT REBASE origin/develop faz a msm coisa que o merge mas n cria o commit