# GIT
Um pouco sobre git para me guiar

1- Git e Versionamento

---------- Versionamento ----------

-> Registro de mudanças em arquivos, que possibilita recuperação ou acesso a versões anteriores;

-> Desenvolvimento de código em colaboração com outros integrantes.

---------- Git ----------

Git é um sistema de versionamento de código, que guarda os registros de versão como snapshots (fotos) do estado do projeto, além da referência/caminho para essa foto.

A maioria das operações feitas pelo Git são locais e por isso boa parte das operações são praticamente instantâneas devido á facilidade de acessar arquivos em seu próprio computador.


Possiveis estados  que o git classifica:

- Untracked => 

- Unmodified => Já está mapeado, significa que ele já passou pelo processo de Staged e que já foi commitado, é um cara que se encontra salvo do jeito que ele está.

- Modified => Quando o arquivo é modificado

- Staged => é o estado que o arquivo fica antes de ser commitado


Pode instalar:
- github desktop
- gitlens

Comandos:

git --verison => verificar vesão

git config --global user.name "seunome" => para configurar seu nome
git config --global user.email  seuemail   => para configurar o seu e-mail

git clone  seulink ENTER	=> serve para clona algo pronto da web
git init  => inicia um repositorio git
git status =>  mostra o estado da branch

git add arquivo_quer_adcionar => para adicionar um arquivo com suas modificações para a aréa de staged

git diff => ele mostra as linhas que foram modificadas
git diff --staged => serve para ver a diferença dos arquivos que já estão na aréa de staged

git commit -m "sua mensagem"

git log => ele trás um histórico dos commits

git restore nome_do_arquivo => volta a versão anterior ou desfazer as modificações que foram feitas.

git restore --staged nome_do_arquivo => para restaurar e voltar para a aréa de modificações

git push => Para enviar para o repósitorio remoto

git remote => consegui vê tudo sobre o remoto

git push origin master => enviar para a areá remota (origem) no ramo principal (basicamente atualiza o repositorio remoto)


git pull  => vai puxar tudo que está no repositorio remoto

git fetch => vai fazer dowload de tudo que não tem no repositorio local 

git diff origin/master => vai mostrar o que está faltando do fetch


Branch ----------------------------------------------

São ramificações que podemos fazer no desenvolvimento do nosso código.

git branch testing => 
git log  --oneline --decorate => ele informa onde o HEAD está apontando

git checkout testing => vai para a branch testing


.gitignore => serve para o git ignorar 


Merging branches ------------------------------------------------
serve para unir as branches

git branch => mostra as branchs que existem e também mostra a branch que está atualmente

 git merge testing => está juntando a master mais a testing
