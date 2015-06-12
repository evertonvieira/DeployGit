# Deploy Git

A primeira coisa que você deve fazer no servidor de produção é definir o seu nome de usuário e endereço de e-mail:

git config --global user.name "Seu Nome" <br />
git config --global user.email "seuemail@example.com"
<br />	

Alterado o enderço da raiz de produção no arquivo <strong>post-receive</strong>:<br />	
DIRETORIO_PRODUCAO = "home/usuario/www"
<br />

Depois colocar o arquivo <strong>post-receive</strong> dentro da pasta hooks de seu repositório BARE e via terminal dar seguite permissão:
<strong>chmod +x</strong> .

pronto pasta dar push :D 
