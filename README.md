# 🟦 Protocolo Cyberpunk: arch-update-full (v3.5)

**"Automação é a fundação da soberania digital."** > Script desenvolvido para centralizar a manutenção crítica de sistemas baseados em Arch Linux.

O arch-update-full evoluiu de um utilitário de manutenção para um Orquestrador de Integridade e Automação de Próxima Geração. Projetado para o ecossistema Arch Linux, ele transcende a simples atualização ao unificar a gestão de pacotes oficiais, AUR (Yay/Paru), Flatpaks e Snaps sob o Sentinel Protocol v3.5. Através de monitoramento em background via Systemd User Timers, auditoria em tempo real de Kernel/Drivers e um sistema de notificações inteligentes, ele garante que a estabilidade e a segurança do sistema operem de forma autônoma, silenciosa e com performance absoluta


# 🛠️ Arquitetura do Protocolo (Core Functions)

🛡️ Arch Update Full: Sentinel Protocol (v3.5)
O arch-update-full evoluiu de um simples script para um ecossistema de manutenção autônomo. Agora, ele executa uma sequência rigorosa de 11 camadas de integridade e inteligência, garantindo que o seu Arch Linux esteja sempre na vanguarda da performance e segurança:

1 ## Modo Sentinela (Silent Interception) [NOVO v3.5]: Implementação de monitoramento em background via Systemd User Timers. O sistema verifica atualizações silenciosamente a cada 12h e emite notificações nativas via libnotify apenas se houver reforços disponíveis.
2 ## Auto-Instalação Dinâmica [NOVO v3.5]: O script possui lógica de autoconfiguração. Ao ser executado, ele valida sua própria persistência no sistema, garantindo que a Sentinela esteja sempre ativa, independente do diretório de instalação.
3 ## Mirror Optimization (Reflector): Otimiza dinamicamente a mirrorlist para os 5 servidores HTTPS mais rápidos e sincronizados, maximizando a largura de banda.
4 ## Integrity & Core Sync (Pacman): Sincronização profunda dos repositórios oficiais e atualização dos pacotes core do sistema.
5 ## AUR Intelligence Hub [ATUALIZADO v3.5]: Detecção automática de helpers. Suporte nativo e inteligente para Yay ou Paru, permitindo a escolha do motor de injeção em tempo real.
6 ## Universal Sandbox Update: Sincronização completa de aplicações isoladas via Flatpak e pacotes universais via Snapd, garantindo que nenhum setor do sistema fique desatualizado.
7 ## Disk Integrity Reserve [NOVO v3.5]: Auditoria de espaço em disco pré-atualização. Se o SSD estiver abaixo de 5GB livres, o script executa uma limpeza de emergência ou aborta o processo para evitar corrupção de dados.
8 ## Auditoria de Núcleo (Kernel & Driver Check) [NOVO v3.5]: Varredura em tempo real nos logs do Pacman para detectar alterações críticas em drivers Nvidia, Kernel Linux, Mesa ou Systemd.
9 ## Purga de Órfãos & Cache: Localização e remoção de dependências residuais (órfãos) e estabilização de cache via paccache, preservando a vida útil do SSD.
10 ## Sentinel Logs (FIFO Rotation) [NOVO v3.5]: Sistema de telemetria com logs rotativos. O script mantém apenas as últimas 7 sessões de atualização, garantindo histórico para debug sem poluir o armazenamento.
11 ## Protocolo de Notificação Universal [NOVO v3.5]: Ao concluir a sequência de reforço, o script dispara um alerta crítico para a interface do GNOME via libnotify. Isso garante que, mesmo que você esteja em outra área de trabalho ou focado em outro estudo, você receba a confirmação imediata de que o Sentinel v3.5 terminou a ronda e o log foi gerado.
---

## 🚀 Instalação Oficial (AUR)
# Disponível no AUR: yay -S arch-update-full
<img width="1577" height="512" alt="Captura de tela de 2026-04-06 18-06-31" src="https://github.com/user-attachments/assets/b6552189-32b1-4e26-959e-908e77a4e55a" />



---
## 📸 Interface e Visual
CLI: Estética Neon Blue com logs detalhados e assinatura personalizada.

Menu: Integração nativa com ambientes GNOME/KDE através do atalho customizado.

Demonstração Visual

### ⚡ Protocolo Sétimo em Ação
<img width="1165" height="863" alt="print 1" src="https://github.com/user-attachments/assets/83e723d5-82b9-43d5-899e-d32b0fefaa9d" />
<img width="1165" height="863" alt="print 2" src="https://github.com/user-attachments/assets/edaa0685-2c07-4f8e-84af-1e5871ad462f" />
<img width="1165" height="863" alt="print 3 " src="https://github.com/user-attachments/assets/85753f93-36db-4e6e-b53d-38f77664a5ad" />

## 📸 Notificações inteligentes: alertas desktop em tempo real sobre a disponibilidade de novas atualizações e a confirmação imediata ao concluir o protocolo de manutenção.
<img width="1425" height="588" alt="print notificaçao" src="https://github.com/user-attachments/assets/4990617b-c5f3-4726-a682-b6f20b4937ce" />


### 🚀 Menu do Sistema (v3.5) — novo Ícone Personalizado
<img width="321" height="285" alt="print logo" src="https://github.com/user-attachments/assets/6b883264-8908-4337-984f-588210056ea9" />




### 🚀 Como Instalar Manualmente

Para usar o script como um comando nativo e ter o atalho no seu menu de aplicativos, execute os seguintes comandos:
```bash
git clone https://aur.archlinux.org/arch-update-full.git
cd arch-update-full
makepkg -si
```
```bash
# 1. Injeta o script no path do sistema
sudo cp arch-update-full /usr/bin/arch-update-full
sudo chmod +x /usr/bin/arch-update-full

# 2. Move o ícone para o diretório de pixmaps do sistema
sudo cp logoarchupdatefull.jpeg /usr/share/pixmaps/

# 3. Instala o atalho no menu de aplicações (XDG)
sudo cp arch-update-full.desktop /usr/share/applications/
```
---

# 🚀 Arch Update Full - Protocolo Cyberpunk
### Desenvolvido por Gustavo Gianeli (Sétimo) 
### "Desenvolvido por The Sétimo — Onde a integridade encontra a performance."


🛡️ Developer Profile (Red Team Focus)
"Projeto focado em Automação Shell e Segurança da Informação."

Autor: Gustavo Gianeli (Sétimo)

Hardware: Acer Nitro V15 | i7 13th Gen | RTX 4050 | 32GB RAM

Location: Ourinhos, SP - Brazil
