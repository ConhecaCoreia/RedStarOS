# RedStarOS

## Introdução
O RedStarOS é um sistema operacional baseado em linux criado e mantido pela KCC, Korea Computer Center, está atualmente na sua versão 4 (Server e Desktop) e é baseado no Fedora. Ele também é distribuído na versão mobile, baseado no Android.

## Utilização
O RedStarOS 4.0 Server atualmente é utilizado nos servidores em geral na Coreia Popular, como pode ser visto, por exemplo, neste link: http://pyongyangtimes.com.kp/404

Já RedStarOS 4.0 Desktop é utilizado geralmente nos computadores do governo, pois este oferece mais segurança para os dados do mesmo, como controle de portas através do Firewall, por exemplo. Nos outros computadores do país (sejam desktops, notebooks, etc) é mais comum o uso do sistema speracional Windows.

E o RedStarOS Mobile é utilizado nos dispositivos móveis como celulares e tablets fabricados por empresas coreanas, como por exemplo Woolim, Ariang, Samjiyon e Manbang.

## Download e Instalação
Ainda não foi disponibilizado para download na internet a versão mais recente do RedStarOS, entretanto, abaixo é disponibilizado o manual de download e instalação da versão 3.0-Desktop.

Por se tratar de uma versão antiga, não é recomendado instalar no seu computador como sistema operacional principal. Baixe um emulador de maquinas virtuais, como o VirtualBox e aproveite.

### RedStarOS_3.0-Desktop (2013)

1. Faça o download pelo link:
https://archive.org/download/RedStarOS/Red%20Star%20OS%203.0%20Desktop/DESKTOP_redstar_desktop3.0_sign.iso

2. Altere o idioma do instalador de Coreano para Inglês se preferir (recomendado):
Edite o arquivo dentro da iso /isolinux/isolinux.cfg de lang=ko para lang=en.
Dica: use um programa chamado Iso Master para fazer isso.

3. Dê boot na ISO modificada e siga os passos de instalação normalmente.

4. Ao chegar na tela da rede, selecione DHCP.

5. Na última tela antes de clicar em 'inciar a instalação', você pode selecionar quais programas quer instalar, e portanto adicionar programas a instalação que não vem selecionados por padrão.

6. Reinicie o computador (ou a maquina virtual, se for o caso) e logue com seu usuario.

OBS: o sistema vem em coreano por padrão (mesmo alterando o idioma do instalador).

7. Habilite a conta root (administrador) e defina uma senha.
Digite no terminal:	rootsetting
Clique no cadeado e insira a senha do SEU usuário.
Depois habilite a caixa de seleção e então crie uma senha para o usuário ROOT.

OBS: para acessar o usuario root pelo terminal digite o comando su e depois entre com a senha escolhida no passo anterior.

8. Altere o idioma do sistema se preferir (recomendado).
Digite no terminal (como usuário root):
sed -i 's/ko_KP/en_US/g' /etc/sysconfig/i18n
e depois:
sed -i 's /ko_KP/en_US/g' /usr/share/config/kdeglobals

9. Desabilite as restrições do Firewall.
Digite no terminal (como usuário root):
rm /etc/sysconfig/iptables

OBS: É preciso reiniciar para as alterações do passo 8 e 9 surtirem efeito, mas pode deixar para reiniciar depois.

10. Altere o idioma do navegador de internet:
Abra o navegador Naenara.
Abra a segunda lista suspensa à direita e escolha a terceira opção.
Vá para a segunda guia da direita na janela que apareceu, clique no único botão que não está acinzentado / é clicável.
Isso traz uma barra amarela com um botão, clique nele.

11. Agora reinicie o computador e aproveite!
