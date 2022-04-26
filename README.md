# Repositorio do desafio de projeto sobre Git/GitHub da Dio
Desafio de projeto sobre Git/GitHub

# Introd:  

Esse projeto é criado para mostra um pouco do conhecime de estudo do Git/GitHub feito no projeto de estudos da Dio. 

# O que é GitHub?

GitHub é uma plataforma de hospedagem de código-fonte e arquivos com controle de versão usando o Git. Ele permite que programadores, utilitários ou qualquer usuário cadastrado na plataforma contribuam em projetos privados e/ou Open Source de qualquer lugar do mundo.

# instalador do Git 
[git](https://git-scm.com/) 

# Como configurar seu Git 

1.6 Começando - Configuração Inicial do Git
Configuração Inicial do Git
Agora que você tem o Git em seu sistema, você deve fazer algumas coisas para personalizar o ambiente Git. Você fará apenas uma vez por computador e o efeito se manterá após as atualizações. Você também pode mudá-las em qualquer momento rodando esses comandos novamente.

O Git vem com uma ferramenta de chamada git configque permite ver e variáveis ​​de configuração que controlam todos os aspectos como o Git aparece e opera. Estas variáveis ​​podem ser em todas as coisas diferentes:

/etc/gitconfig: válido para todos os usuários no sistema e todos os seus usuários. Se você passar a opção --systempara git config, ele lê e escreve neste arquivo.

~/.gitconfigou ~/.config/git/config: Somente para o seu usuário. Você pode fazer o Git ler e escrever neste arquivo passando a opção --global.

configno Git ( seja .git/config) de qualquer opçãoou você está usando: específico para este uso.

Cada nível sobrescreve os valores no nível anterior, ou seja, valores em .git/configprevalecem sobre /etc/gitconfig.

No Windows, Git procura pelo arquivo .gitconfigno pasta $HOME( C:\Users\$USERpara a maioria). Ele também procura por /etc/gitconfig, mesmo sendo relativo à raiz do sistema, que é onde quer que você tenha instalado Git no seu sistema.

Sua Identidade
A primeira coisa que você deve fazer ao instalar Git é configurar seu nome de usuário e endereço de e-mail. Isto é importante porque cada commit usa esta informação, e ela é carimbada de forma imutável nos commits que você começa a criar:

$ git config --global user.name "Fulano de Tal"
$ git config --global user.email fulanodetal@exemplo.br
Reiterando, você deve fazer isso somente uma vez se você quiser a opção --global, porque o Gitt está informando para qualquer coisa que você deve fazer esse sistema. Se você quiser substituir essa informação com nome para um projeto específico, você pode ou o comando sem a opção --globaldentro daquele projeto.

Muitas ferramentas GUI ou com isso quando foram usadas pela primeira vez.

Seu Editor
Agora que sua identidade está definida, você pode escolher o editor de texto padrão que será chamado quando o Git precisar que você entre uma mensagem. Se não for configurado, o Git usará o editor padrão, que normalmente é o Vim. Se você quiser usar um editor de texto diferente, como o Emacs, você pode fazer o seguinte:

$ git config --global core.editor emacs
Aviso
Em e Emac são editores comumente usados ​​por designers em sistemas populares e comumente usados ​​em Linux como Linux. Se você não for configurado com estes editores ou estiver em um sistema Windows, você pode procurar por instruções de como configurar o seu editor preferido com Git. Se você não pode configurar você o seu editor preferido e não sabe usar o Vim ou Emacs, é que não pode configurar você o seu bastante confuso ao entrar.

Testando Suas Configurações
Se você quiser testar como suas configurações, você pode usar o comando git config --listpara listar todas as configurações que o Git conseguir encontrar naquele momento:

$ git config --list
user.name=Fulano de Tal
user.email=fulanodetal@exemplo.br
color.status=auto
color.branch=auto
color.interactive=auto
color.diff=auto
...
Pode ser que algumas palavras sejam diferenciadas, mais de uma vez, porque lêem as mesmas chaves de arquivos ( /etc/gitconfige ~/.gitconfig, por exemplo). Neste caso, Git usa o último valor para cada chave única que ele vê.

Você também pode testar o que Git tem em uma chave específica digitando git config <key>:

$ git config user.name
Fulano de Tal

[link](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Configura%C3%A7%C3%A3o-Inicial-do-Git)

ass: Tiago Lopes 