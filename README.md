***🛡️ Arch Update Full (Protocolo Sentinela)*** **Versão 3.7-4**

**"Automação é a fundação da soberania digital."** > Script desenvolvido para centralizar a manutenção crítica de sistemas baseados em Arch Linux.

O arch-update-full evoluiu de um utilitário de manutenção para um Orquestrador de Integridade e Automação de Próxima Geração. Projetado para o ecossistema Arch Linux, ele transcende a simples atualização ao unificar a gestão de pacotes oficiais, AUR (Yay/Paru), Flatpaks e Snaps sob o Sentinel Protocol v3.7-4 Através de monitoramento em background via Systemd User Timers, auditoria em tempo real de Kernel/Drivers e um sistema de notificações inteligentes, ele garante que a estabilidade e a segurança do sistema operem de forma autônoma, silenciosa e com performance absoluta

🚀 Novidades: Arch Update Full v3.7-4 (Sentinel Update)
Destaques da nova versão do protocolo de automação:

🛡️ Sentinel Mode (100% Fantasma): Implementação de um interceptador silencioso para o Systemd. Agora o sistema verifica atualizações em background sem abrir terminais ou vazar processos de interface.

📊 Telemetria Segregada: Criação de logs específicos e automáticos para as rondas do Sentinela, isolando o histórico de background das sessões manuais.

✅ Certificação ShellCheck: Código 100% validado e refatorado. Zero erros de sintaxe e lógica, garantindo estabilidade máxima no Bash.

🧹 Aritmética Blindada: Correção no processamento de contagem de pacotes, eliminando bugs de espaços vazios no retorno dos comandos.

**📦 Instalação (AUR)**
**O Arch Update Full está disponível no AUR. Esta é a forma recomendada de instalação para manter o software sempre atualizado.**

## Via yay:
**yay -S arch-update-full**

## Via paru:
**paru -S arch-update-full**

# 🛠️ Arquitetura do Protocolo (Core Functions)

🛡️ Arch Update Full: Sentinel Protocol (v3.7-4)
O arch-update-full evoluiu de um simples script para um ecossistema de manutenção autônomo. Agora, ele executa uma sequência rigorosa de 13 camadas de integridade e inteligência, garantindo que o seu Arch Linux esteja sempre na vanguarda da performance e segurança:

### 🚀 Camadas de Integridade e Inteligência (Sentinel Protocol v3.7-4)

1. **Modo Sentinela (Silent Interception)**: Implementação de monitoramento em segundo plano via Systemd User Timers. O sistema verifica atualizações silenciosamente **a cada 3 horas** e emite notificações nativas via libnotify apenas se houver novos pacotes disponíveis.

2. **Auto-Instalação Dinâmica:** O script possui lógica de autoconfiguração. Ao ser executado, ele valida sua própria persistência no sistema, garantindo que o serviço Sentinela esteja sempre ativo, independente do diretório de instalação.

3. **Mirror Optimization (Reflector):** Otimiza dinamicamente a *mirrorlist* para os 5 servidores HTTPS mais rápidos e sincronizados, maximizando a largura de banda de download.

4. **Integrity & Core Sync (Pacman):** Sincronização profunda dos repositórios oficiais e atualização dos pacotes vitais do sistema.

5. **AUR Intelligence Hub:** Detecção automática de *AUR Helpers*. Possui suporte nativo e inteligente para **Yay** ou **Paru**, permitindo a escolha do motor de atualização em tempo real.

6. **Universal Sandbox Update:** Sincronização completa de aplicações isoladas via **Flatpak** e pacotes universais via **Snapd**, garantindo que nenhum setor do sistema fique desatualizado.

7. **Disk Integrity Reserve:** Auditoria de espaço em disco pré-atualização. Se o SSD estiver com menos de 5GB livres, o script executa uma limpeza de emergência ou aborta o processo para evitar a corrupção de dados.

8. **Auditoria de Núcleo (Kernel & Driver Check):** Varredura em tempo real nos logs do Pacman para detectar alterações críticas em drivers **Nvidia**, **Kernel Linux**, **Mesa** ou **Systemd**.

9. **Purga de Órfãos & Cache:** Localização e remoção de dependências residuais (órfãos) e estabilização de cache via `paccache`, preservando a vida útil do SSD.

10. **Sentinel Logs (FIFO Rotation):** Sistema de telemetria com logs rotativos. O script mantém apenas as últimas 7 sessões de atualização, garantindo histórico para depuração sem poluir o armazenamento.

11. **Protocolo de Notificação Universal:** Ao concluir a sequência de manutenção, o script dispara um alerta para a interface desktop via `libnotify`. Isso garante que, mesmo em outra área de trabalho ou focado em outros estudos, você receba a confirmação imediata de que o **Sentinel** finalizou a tarefa e o log foi gerado.
    
12. **📊 Sistema de Telemetria (Logs)**
O protocolo mantém dois fluxos de logs independentes:
**~/.logs_arch_update_full/:** Histórico completo das sessões manuais.
**~/.logs_sentinel_check/:** Logs técnicos da ronda do sentinela (retenção de 3 versões).

13. **Validação ShellCheck (Certificação de Qualidade)** O Padrão: O código foi passado pelo crivo do ShellCheck e saiu com zero erros. Resultado: Isso garante que a sintaxe do Bash está impecável, as variáveis estão protegidas com aspas e não há riscos de falhas silenciosas por má formação de comandos. É um código blindado.

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
<img width="1165" height="863" alt="print 1" src="https://github.com/user-attachments/assets/3cfa2620-f109-4e65-87a9-9da0094d9ae5" />
<img width="1165" height="863" alt="print 2" src="https://github.com/user-attachments/assets/42fb18be-d516-4918-a6bd-03d6c4de7850" />
<img width="1165" height="863" alt="print 3" src="https://github.com/user-attachments/assets/648287ab-8879-44f6-a521-ede113763281" />



### 🚀 Menu do Sistema 

<img width="114" height="120" alt="logoarchupdatefull" src="https://github.com/user-attachments/assets/f3229a30-43b3-42e5-94b4-dd3110b7203d" />


### Pasta de logs:
<img width="609" height="180" alt="pasta logs" src="https://github.com/user-attachments/assets/dd63a2f2-708c-490f-baef-e97028eb2ad2" />
<img width="1337" height="773" alt="log check" src="https://github.com/user-attachments/assets/80f5efc6-c01e-4b93-bbcf-52ba1c9fab4d" />






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
