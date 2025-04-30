# Mini curso de git github

## Comandos

Verifica se o Git está instalado e a versão.
``` bash
 git --version
```

Inicializar o git na projeto local
``` bash
 git init
```

Adicionar todos arquivos
``` bash
 git add .
```

Faz um commit com uma mensagem descritiva sobre as alterações realizadas
``` bash
 git commit -m "descriçã do commit"
```
Enviar para repositorio remoto
``` bash
 git push
```

Enviar para repositorio remoto
``` bash
 git push -U oringin <nome da branch>
```

Ver o histórico
```bash
git reflog
```
Voltar para o commit
```bash
git reset --hard "HEAD@{<numero do commit>}"
```

ou

```bash
git reset --hard <hash>
```

Clonar projeto
```bash
git clone <endereco do projeto>
```
lista as branches
```bash
git branch
```

cria uma nova branch
```bash
git branch <nome da branch>
```
muda para branch
```bash
git checkout <nome da branch>
```
cria e muda para branch
```bash
git checkout -b <nome da branch>
```
realiza o commit

push na branch
```bash
git push -u origin <nome da branch>
```

fazer merge

remoto precisa criar uma cópia

lista as branches locais e remotas
```bash
git branch -a
```

Caso não tenha as branches locais:
```bash
git branch <nome da branch> origin/<nome da branch>
```

cria e muda para a branch, neste caso para fazer o merge precisa voltar para branch principal
```bash
git checkout -b feature/pag3 origin/<nome da branch>
```
faz o merge para cada branch
```bash
git merge <nome da branch>
```

Faz o push da branch principal atualizada
```bash
git push origin main
```
Para deletar a branch
```bash
git branch -d <nome da branch>
```

Para deletar a branch se ainda não tiver realizado merge
```bash
git branch -D <nome da branch>
```
Para deletar a branch remota
```bash
git push origin --delete <nome da branch>
```