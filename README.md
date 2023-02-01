# **Ambiente Desenvolvimento**

## Zsh
Primeiramente certifique que o ``git`` esteja instalado, pois vamos precisar dele mais na frente, caso nao esteja instalado é só digitar o seguinte comando:

````
sudo apt install git
````

Feito isso, agora vamos instalar o ZSH:

````
sudo apt install zsh
````
Ótimo, agora vamos precisar clonar um repositório do Oh My Zsh:

```
git clone https://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh
```
Clonado o repositório, agora será preciso criar o arquivo ``.zshrc`` que é um arquivo onde estará todas as configurações do zsh, nesse arquivo você pode mudar o tema, adicionar alias e outros. No meu caso eu só uso para adicionar os meus Alias, que são atalhos para que eu nao precise digitar comandos enormes que utilizo sempre. Logo mais vou ensinar como fazer os alias. 

Bom, agora crie o arquivo com esse comando:

````
cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc
````

Agora mude o padrão do seu terminal para o Zsh, já que ele ja vem como bash:

```
chsh -s $(which zsh)
```
Feito isso, será preciso reiniciar seu Linux, se tiver usando WSL é só fechar o terminal e abrir novamente.
### Theme OhMyZsh
Para ativar um tema, defina ZSH_THEMEo nome do tema em seu ~/.zshrc, antes de obter Oh My Zsh.

```
ZSH_THEME=passion
```
##  Docker
### Desinstalar versões antigas
 
Versões mais antigas do Docker eram chamadas de `docker`, `docker.io` ou `docker-engine`. Desinstale essas versões mais antigas antes de tentar instalar uma nova versão:

```bash
sudo apt-get remove docker docker-engine docker.io containerd runc
```
    https://docs.docker.com/engine/install/ubuntu/#uninstall-docker-engine

### Instalar Docker Engine

    https://docs.docker.com/engine/install/ubuntu/

### Pós Instalação

    https://docs.docker.com/engine/install/linux-postinstall/
