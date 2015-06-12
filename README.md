# Deploy Git

A primeira coisa que você deve fazer no servidor de produção é definir o seu nome de usuário e endereço de e-mail:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```

<br />	

Altere o enderço da raiz de produção no arquivo <strong>post-receive</strong>:<br />	
```bash
DIRETORIO_PRODUCAO = "home/usuario/www"
```

Depois coloque o arquivo <strong>post-receive</strong> dentro da pasta hooks de seu repositório <strong>bare</strong> e via terminal dê a seguite permissão:
```bash
chmod +x
```
pronto basta dar <strong>push</strong> :D. 
