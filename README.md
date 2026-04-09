***🛡️ Arch Update Full (Protocolo Sentinela)*** **Versão 3.6**

**"Automação é a fundação da soberania digital."** > Script desenvolvido para centralizar a manutenção crítica de sistemas baseados em Arch Linux.

O arch-update-full evoluiu de um utilitário de manutenção para um Orquestrador de Integridade e Automação de Próxima Geração. Projetado para o ecossistema Arch Linux, ele transcende a simples atualização ao unificar a gestão de pacotes oficiais, AUR (Yay/Paru), Flatpaks e Snaps sob o Sentinel Protocol v3.6. Através de monitoramento em background via Systemd User Timers, auditoria em tempo real de Kernel/Drivers e um sistema de notificações inteligentes, ele garante que a estabilidade e a segurança do sistema operem de forma autônoma, silenciosa e com performance absoluta

🚀 Novidades da Versão 3.6 (Protocolo Sentinela)
Esta atualização foca em automação proativa e refinamento visual:

Monitoramento Sentinela: O script agora conta com uma **verificação automática a cada 3 horas**, notificando o usuário sobre atualizações pendentes sem a necessidade de verificação manual.

Interface de Terminal Corrigida: Ajuste completo nas caixas de texto e diálogos internos do terminal, eliminando erros de exibição e melhorando a legibilidade dos logs.

Identidade Visual: Implementação oficial do novo ícone de alta resolução para integração total com menus de sistemas modernos.

**📦 Instalação (AUR)**
**O Arch Update Full está disponível no AUR. Esta é a forma recomendada de instalação para manter o software sempre atualizado.**

## Via yay:
**yay -S arch-update-full**

## Via paru:
**paru -S arch-update-full**

# 🛠️ Arquitetura do Protocolo (Core Functions)

🛡️ Arch Update Full: Sentinel Protocol (v3.6)
O arch-update-full evoluiu de um simples script para um ecossistema de manutenção autônomo. Agora, ele executa uma sequência rigorosa de 11 camadas de integridade e inteligência, garantindo que o seu Arch Linux esteja sempre na vanguarda da performance e segurança:

### 🚀 Camadas de Integridade e Inteligência (Sentinel Protocol v3.6)

O **arch-update-full** executa uma sequência rigorosa de onze camadas de integridade: ele unifica a atualização de pacotes oficiais, AUR (com suporte a Yay e Paru), Flatpaks e Snaps, realizando uma limpeza profunda no sistema, auditoria de Kernel e drivers de vídeo, verificação de espaço em disco e agora conta com o **Modo Sentinela**, logs rotativos e notificações desktop de disponibilidade e conclusão.

1. **Modo Sentinela (Silent Interception) [ATUALIZADO v3.6]: Implementação de monitoramento em segundo plano via Systemd User Timers. O sistema verifica atualizações silenciosamente **a cada 3 horas** e emite notificações nativas via libnotify apenas se houver novos pacotes disponíveis.

2. **Auto-Instalação Dinâmica:** O script possui lógica de autoconfiguração. Ao ser executado, ele valida sua própria persistência no sistema, garantindo que o serviço Sentinela esteja sempre ativo, independente do diretório de instalação.

3. **Mirror Optimization (Reflector):** Otimiza dinamicamente a *mirrorlist* para os 5 servidores HTTPS mais rápidos e sincronizados, maximizando a largura de banda de download.

4. **Integrity & Core Sync (Pacman):** Sincronização profunda dos repositórios oficiais e atualização dos pacotes vitais do sistema.

5. **AUR Intelligence Hub:** Detecção automática de *AUR Helpers*. Possui suporte nativo e inteligente para **Yay** ou **Paru**, permitindo a escolha do motor de atualização em tempo real.

6. **Universal Sandbox Update:** Sincronização completa de aplicações isoladas via **Flatpak** e pacotes universais via **Snapd**, garantindo que nenhum setor do sistema fique desatualizado.

7. **Disk Integrity Reserve:** Auditoria de espaço em disco pré-atualização. Se o SSD estiver com menos de 5GB livres, o script executa uma limpeza de emergência ou aborta o processo para evitar a corrupção de dados.

8. **Auditoria de Núcleo (Kernel & Driver Check):** Varredura em tempo real nos logs do Pacman para detectar alterações críticas em drivers **Nvidia**, **Kernel Linux**, **Mesa** ou **Systemd**.

9. **Purga de Órfãos & Cache:** Localização e remoção de dependências residuais (órfãos) e estabilização de cache via `paccache`, preservando a vida útil do SSD.

10. **Sentinel Logs (FIFO Rotation):** Sistema de telemetria com logs rotativos. O script mantém apenas as últimas 7 sessões de atualização, garantindo histórico para depuração sem poluir o armazenamento.

11. **Protocolo de Notificação Universal:** Ao concluir a sequência de manutenção, o script dispara um alerta para a interface desktop via `libnotify`. Isso garante que, mesmo em outra área de trabalho ou focado em outros estudos, você receba a confirmação imediata de que o **Sentinel v3.6** finalizou a tarefa e o log foi gerado.

---

### 🔔 Notificações Inteligentes
**Alertas desktop em tempo real sobre a disponibilidade de novas atualizações e a confirmação imediata ao concluir o protocolo de manutenção.**
<img width="1425" height="588" alt="print notificaçao" src="https://github.com/user-attachments/assets/c84c3874-0940-4a60-bbc0-2943818cc826" />

---
## 📸 Interface e Visual
CLI: Estética Neon Blue com logs detalhados e assinatura personalizada.

Menu: Integração nativa com ambientes GNOME/KDE através do atalho customizado.

Demonstração Visual

### ⚡ Protocolo Sétimo em Ação
<img width="1617" height="1053" alt="print1" src="https://github.com/user-attachments/assets/a6d40088-0e30-4f8e-92b7-161d77f51d30" />
<img width="1617" height="1053" alt="print2" src="https://github.com/user-attachments/assets/7f698a04-61af-4b92-b656-8698368a8cdb" />
<img width="1617" height="1053" alt="print3" src="https://github.com/user-attachments/assets/fabf4be0-e7d4-4e74-b1f6-facac26cb8b9" />




### 🚀 Menu do Sistema (v3.6) — novo Ícone Personalizado

<img width="114" height="120" alt="logoarchupdatefull" src="https://github.com/user-attachments/assets/f3229a30-43b3-42e5-94b4-dd3110b7203d" />




### 🚀 **RECOMENDAMOS INSTALAR VIA PACOTE AUR** mas se prefirir fazer manualmente 

# Como Instalar Manualmente

Para usar o script como um comando nativo e ter o atalho no seu menu de aplicativos, execute os seguintes comandos:
```bash
git clone https://aur.archlinux.org/arch-update-full.git
cd arch-update-full
makepkg -si
```
Ou se preferir...

```bash
# 1. Injeta o script no path do sistema
sudo cp arch-update-full /usr/bin/arch-update-full
sudo chmod +x /usr/bin/arch-update-full

# 2. Move o ícone para o diretório de pixmaps do sistema
sudo cp logoarchupdatefull.png /usr/share/pixmaps/

# 3. Instala o atalho no menu de aplicações (XDG)
sudo cp arch-update-full.desktop /usr/share/applications/
```
---

# 🚀 Arch Update Full - Protocolo Cyberpunk - - Protocolo Sentinela
### Desenvolvido por Gustavo Gianeli (Sétimo) 
### "Desenvolvido por The Sétimo — Onde a integridade encontra a performance."


🛡️ Developer Profile (Red Team Focus)
"Projeto focado em Automação Shell e Segurança da Informação."

Autor: Gustavo Gianeli (Sétimo)

Hardware: Acer Nitro V15 | i7 13th Gen | RTX 4050 | 32GB RAM

Location: Ourinhos, SP - Brazil
