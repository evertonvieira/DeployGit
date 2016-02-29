# Deploy Git
###Automatizando o deploy com o Git.

Para que não haja a necessidade de se logar no servidor de produção (**POR SSH**) toda vez que houver uma nova alteração, esse script foi criado com o intuíto de realizar esta tarefa automática. Toda vez que houver um **push** no repositório **bare**, o script se encarrega de jogar para a raiz do servidor (**projeto online**) o **commit** enviado. 

A primeira coisa que deve ser feita no servidor de produção é definir o seu **nome de usuário** e **endereço de e-mail** (caso não tenha definido antes):

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```

<br />	

Altere o endereço da raiz de produção no arquivo <strong>post-receive</strong>:<br />	
```bash
DIRETORIO_PRODUCAO = "home/usuario/www"
```

Depois coloque o arquivo <strong>post-receive</strong> dentro da pasta <strong>hooks</strong> de seu repositório <strong>bare</strong> e via terminal dê a seguite permissão:
```bash
chmod +x
```
pronto basta dar <strong>push</strong> e ver a mágica :D. 
