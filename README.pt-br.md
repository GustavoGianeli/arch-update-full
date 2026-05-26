 <img src="https://flagcdn.com/16x12/us.png" alt="US">  [English (US)](README.md) | <img src="https://flagcdn.com/16x12/br.png" alt="BR">  [Português (BR)](README.pt-br.md)
---
***🛡️ Arch Update Full (Protocolo Sentinela)🔄*** **Versão 3.8**
---

**Organizador avançado, leve e totalmente automatizado desenvolvido para o Arch Linux. Centraliza atualizações, otimizações de desempenho e auditorias de integridade do sistema..**

**Arch-Update-Full: O Protocolo de Elite para Gestão de Atualizações do Arch Linux. Sincronização inteligente de Pacman, AUR e Flatpaks e Snaps,  com auditoria de integridade em tempo real. Automação absoluta, incluído tudo que é preciso para atualização e manutenções de rotina ( pacote órfãos e cache).**

---
**🚀 Novidades: Arch Update Full v3.8 (Sentinel Update)**
Destaques da nova versão do protocolo de automação:

**⚡ Smart Connectivity Gatekeeper:** Sistema de pré-verificação de uplink que valida a conexão antes de iniciar processos críticos, evitando timeouts e corrupção de base de dados.

**📊 Real-time Latency Telemetry:** Extração precisa de latência via AWK, exibindo o status da rede em milissegundos (ms) diretamente na interface.

**🎨 Redesign de Interface (Block Edition):** Next-Gen UI Architecture: Implementação da interface Block Edition, utilizando molduras de caracteres duplos e alinhamento dinâmico para uma experiência de terminal imersiva e profissional.

**🧹 Correção do bug dos Pacotes Órfãos**

**🛡️Conflict Mediation:** Remoção estratégica da flag --noconfirm no ambiente Pacman para permitir a validação humana em mudanças críticas de pacotes, mantendo a integridade total do Arch Linux.

✅ **Certificação ShellCheck: Código 100% validado**. Zero erros de sintaxe e lógica, garantindo estabilidade máxima no Bash.

---
**📦 Instalação (AUR): O Arch Update Full está disponível no AUR. Esta é a forma recomendada de instalação para manter o software sempre atualizado.**
---

**👉  Link do pacote no AUR:https://aur.archlinux.org/packages/arch-update-full**

**⚠️ Nota sobre a versão no AUR:** No repositório do AUR, o pacote encontra-se na versão 3.8-7. O sufixo -7 representa apenas revisões de empacotamento (pkgrel) feitas durante o deploy (como correções de checksums e caminhos de ícones). O código-fonte principal e as funcionalidades permanecem exatamente os mesmos da versão 3.8 estável deste repositório.


### 🚀 **Instalação Rápida (AUR Helpers)**
**Escolha o seu gerenciador do AUR de preferência para sincronizar e instalar o pacote automaticamente:**

 **➡ Instalação via Yay:** 
```bash
yay -S arch-update-full
```
 **➡ Instalação via Paru:**
```bash
paru -S arch-update-full
```

---
# **Arquitetura do Protocolo (Core Functions):**
**🛡️ Arch Update Full: Sentinel Protocol (v3.8)**

O arch-update-full evoluiu de um simples script para um ecossistema de manutenção autônomo. Agora, ele executa uma sequência rigorosa de 14 camadas de integridade e inteligência, garantindo que o seu Arch Linux esteja sempre na vanguarda da performance e segurança:

### 🚀 Camadas de Integridade e Inteligência (Sentinel Protocol)

1. **Modo Sentinela (Silent Interception)**: Implementação de monitoramento em segundo plano via Systemd User Timers. O sistema verifica atualizações silenciosamente **a cada 3 horas** e emite notificações nativas via libnotify apenas se houver novos pacotes disponíveis.

2. **Auto-Instalação Dinâmica:** O script possui lógica de autoconfiguração. Ao ser executado, ele valida sua própria persistência no sistema, garantindo que o serviço Sentinela esteja sempre ativo, independente do diretório de instalação.

3. **Mirror Optimization (Reflector):** Otimiza dinamicamente a *mirrorlist* para os 5 servidores HTTPS mais rápidos e sincronizados, maximizando a largura de banda de download.

4. **Integrity & Core Sync (Pacman):** Sincronização profunda dos repositórios oficiais e atualização dos pacotes vitais do sistema.

5. **AUR Intelligence Hub:** Detecção automática de *AUR Helpers*. Possui suporte nativo e inteligente para **Yay** ou **Paru**, permitindo a escolha do motor de atualização em tempo real.

6. **Universal Sandbox Update:** Sincronização completa de aplicações isoladas via **Flatpak** e pacotes universais via **Snapd**, garantindo que nenhum setor do sistema fique desatualizado.

7. **Disk Integrity Reserve:** Auditoria de espaço em disco pré-atualização. Se o SSD estiver com menos de 5GB livres, o script executa uma limpeza de emergência ou aborta o processo para evitar a corrupção de dados.

8. **Auditoria de Núcleo (Kernel & Driver Check):** Varredura em tempo real nos logs do Pacman para detectar alterações críticas em drivers **Nvidia**, **Kernel Linux**, **Mesa** ou **Systemd**.

9. **Purga de Órfãos & Cache:** Localização e remoção de dependências residuais (órfãos) e estabilização de cache via `paccache` `paccache -r` `pacman -Sc`  usando comando Sc, preservando a vida útil do SSD.

10. **Sentinel Logs (FIFO Rotation):** Sistema de telemetria com logs rotativos. O script mantém apenas as últimas 13 sessões de atualização, garantindo histórico para depuração sem poluir o armazenamento.

11. **Protocolo de Notificação Universal:** Ao concluir a sequência de manutenção ou achar uma atualização (modo sentinela ghost), o script dispara um alerta para a interface desktop via `libnotify`. Isso garante que, em **qualquer interface, desktop environment (DE)** mesmo em outra área de trabalho ou focado em outros estudos, você receba a confirmação imediata de que o **Sentinel** finalizou a tarefa ou se alguma atualição foi detectada e que os logs foram gerados.
    
12. **Sistema de Telemetria (Logs)**
O protocolo mantém dois fluxos de logs independentes:
**~/.logs_arch_update_full/:** Histórico completo das sessões manuais. (retenção de 13 versões)
**~/.logs_sentinel_check/:** Logs técnicos da ronda do sentinela (retenção de 3 versões).

13. **Validação ShellCheck (Certificação de Qualidade)** O Padrão: O código foi passado pelo crivo do ShellCheck e saiu com zero erros. Resultado: Isso garante que a sintaxe do Bash está impecável, as variáveis estão protegidas com aspas e não há riscos de falhas silenciosas por má formação de comandos. É um código blindado.

14.**Smart Connectivity Gatekeeper:** Sistema de pré-verificação de uplink que valida a conexão antes de iniciar processos críticos, evitando timeouts e corrupção de base de dados.

---
**Notificações Inteligentes**
---

**Alertas desktop em tempo real sobre a disponibilidade de novas atualizações e a confirmação imediata ao concluir o protocolo de manutenção.**

<img width="1752" height="681" alt="sentinela avisando updates" src="https://github.com/user-attachments/assets/677ed619-7c58-4fd2-ada5-414ac2dc342d" />
<img width="1774" height="643" alt="captura protocolo concluido" src="https://github.com/user-attachments/assets/ebb01beb-f0a1-4224-a2a3-037636158249" />


---
## **Interface e Visual :**
**CLI: Estética Neon Blue com logs detalhados e assinatura personalizada.**

**Menu: Integração nativa com os ambientes através do atalho customizado.**

 **⚡ Protocolo Sentinela em Ação:** 
---
<img width="1433" height="1033" alt="cap1" src="https://github.com/user-attachments/assets/ad003aba-a45e-41a9-a316-e1aea8b07aaa" />
<img width="1433" height="1033" alt="cap2" src="https://github.com/user-attachments/assets/ac6b51c9-67dd-4d05-9027-32059575dde9" />
<img width="1433" height="1033" alt="cap3" src="https://github.com/user-attachments/assets/6714d4f7-c713-430e-8139-a8f0517d674b" />
<img width="1433" height="1033" alt="cap4" src="https://github.com/user-attachments/assets/09e9baef-7eed-4a18-8481-5ea40da6008b" />
<img width="1433" height="1033" alt="cap5" src="https://github.com/user-attachments/assets/0fcea070-2bc4-4c2f-8ce0-6dcdbb3df2a0" />


### **🚀 Menu do Sistema (Novidade 3.8!)** 
---
<img width="256" height="256" alt="sentinela-v38" src="https://github.com/user-attachments/assets/1475fb9f-b6cd-42e0-a6ae-64e17270cbdc" />

---
### **📁 Localização dos arquivos de Logs: /home/$USER/. (arquivo oculto) (~/.logs_arch_update_full/ & ~/.logs_sentinel_check/)**
---
<img width="325" height="180" alt="pasta de logs" src="https://github.com/user-attachments/assets/f62cefa6-c59f-4f41-9571-3389a2c1075c" />
<img width="2012" height="1288" alt="logs script completo" src="https://github.com/user-attachments/assets/23425720-bc8d-49be-ac76-51031f53ff46" />
<img width="2012" height="1288" alt="logs do sentinela" src="https://github.com/user-attachments/assets/6e383cce-85ad-4572-940f-4035da5808bd" />

---
**⚠️RECOMENDAMOS INSTALAR VIA PACOTE AUR⚠️** 

**...mas se prefirir fazer manualmente...**

**Como Instalar Manualmente:**
---

**➡ Para usar o script como um comando nativo e ter o atalho no seu menu de aplicativos, execute os seguintes comandos:**
```bash
git clone https://aur.archlinux.org/arch-update-full.git
cd arch-update-full
makepkg -si
```
**➡ Ou se preferir fazer o desdobramento dos arquivos de forma direta e manual:**

**1. Injeta o script no path do sistema:**
```bash
sudo cp arch-update-full /usr/bin/arch-update-full
sudo chmod 755 /usr/bin/arch-update-full
```
**2. Move o ícone para o diretório de pixmaps do sistema:**
```bash
sudo cp sentinela-v38.png /usr/share/pixmaps/
```
**3. Instala o atalho no menu de aplicações (XDG):**
```bash
sudo cp arch-update-full.desktop /usr/share/applications/
```

---
**𝓓𝓮𝓼𝓮𝓷𝓿𝓸𝓵𝓿𝓲𝓭𝓸  𝓹𝓸𝓻  𝓖𝓾𝓼𝓽𝓪𝓿𝓸  𝓖𝓲𝓪𝓷𝓮𝓵𝓲  (O 𝓢é𝓽𝓲𝓶𝓸)**

**"𝓓𝓮𝓼𝓮𝓷𝓿𝓸𝓵𝓿𝓲𝓭𝓸  𝓹𝓸𝓻  𝓣𝓱𝓮 𝓢𝓮𝓿𝓮𝓷𝓽𝓱  —  𝓸𝓷𝓭𝓮  𝓪  𝓲𝓷𝓽𝓮𝓰𝓻𝓲𝓭𝓪𝓭𝓮  𝓮𝓷𝓬𝓸𝓷𝓽𝓻𝓪  𝓪  𝓹𝓮𝓻𝓯𝓸𝓻𝓶𝓪𝓷𝓬𝓮."**

---

**🛡️ Developer Profile (Red Team Focus)**

**Foco do Projeto:** Automação Shell para Manutenção e Auditoria da Base Arch Linux.

**Autor:** Gustavo Gianeli (Sétimo)

**Educação:** Estudante de Ciência da Computação (entusiasta de Linux e fuçador)

**Hardware:** Acer Nitro V15 | i7 13th Gen | RTX 4050 | 32GB RAM

**Localização:** Ourinhos, SP - Brazil






