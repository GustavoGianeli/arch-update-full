 <img src="https://flagcdn.com/16x12/us.png" alt="US">  [English (US)](README.md) | <img src="https://flagcdn.com/16x12/br.png" alt="BR">  [Português (BR)](README.pt-br.md)
---
***🛡️ Arch Update Full (Protocolo Sentinela)🔄*** **Versão 3.9-5**
---

**Organizador avançado, leve e totalmente automatizado desenvolvido para o Arch Linux. Centraliza atualizações, otimizações de desempenho e auditorias de integridade do sistema..**

**Arch-Update-Full: O Protocolo de Elite para Gestão de Atualizações do Arch Linux. Sincronização inteligente de Pacman, AUR e Flatpaks e Snaps,  com auditoria de integridade em tempo real. Automação absoluta, incluído tudo que é preciso para atualização e manutenções de rotina( pacote órfãos e cache) mas ainda mantendo o controle nas suas mãos.**

---
**🚀 Novidades: Arch Update Full v3.9-5**
Destaques da nova versão do protocolo de automação:

**⚡Auditoria de Conexão Inteligente: O teste de rede foi aprimorado. O protocolo agora faz um ping primário nos seus mirrors locais. Se não houver resposta, uma segunda tentativa direta no archlinux.org é feita antes de abortar a operação.**

**📊Real-time Latency Telemetry:** **Extração precisa de latência via AWK, exibindo o status da rede em milissegundos (ms) diretamente na interface.**

**🎨 Novo Ícone Oficial: Um visual totalmente renovado e personalizado para combinar com a interface cyberpunk da ferramenta, agora está mais minimalista e qualidade superior.**

**⚙️ Atualização do AUR Híbrida: O controle absoluto está nas suas mãos. Agora você pode escolher o modo de operação na hora de atualizar o AUR:**

**Automático: Executa a atualização rápida (--noconfirm).**

**Manual: Modo interativo onde você pode auditar os PKGBUILDs e confirmar as alterações passo a passo ([!] caso erro de digitação modo manual é executado por padrão).**

**🛡️Conflict Mediation:** Remoção estratégica da flag --noconfirm no ambiente Pacman para permitir a validação humana em mudanças críticas de pacotes, mantendo a integridade total do Arch Linux.

**🔔 Notificação Interativa (Modo Sentinela): O daemon em background agora dispara um alerta visual inteligente com um botão "⚡ Click to Launch App". Ao clicar, ele aciona o lançador .desktop nativo e abre o terminal automaticamente na sua frente.**

**🌐 Suporte Bilíngue Temporário: Para abraçar nossa comunidade global, as saídas do terminal agora apresentam textos duplicados lado a lado (PT-BR e EN-US).**

✅ **Certificação ShellCheck: Código 100% validado**. Zero erros de sintaxe e lógica, garantindo estabilidade máxima no Bash.

---
**📦 Instalação (AUR): O Arch Update Full está disponível no AUR. Esta é a forma recomendada de instalação para manter o software sempre atualizado.**
---

**👉  Link do pacote no AUR:https://aur.archlinux.org/packages/arch-update-full**

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
**🛡️ Arch Update Full: Sentinel Protocol (v3.9-5)**

O arch-update-full evoluiu de um simples script para um ecossistema de manutenção autônomo. Agora, ele executa uma sequência rigorosa de 16 camadas de integridade e inteligência, garantindo que o seu Arch Linux esteja sempre na vanguarda da performance e segurança:

### 🚀 Camadas de Integridade e Inteligência 

1. **Modo Sentinela (Silent Interception)**: Implementação de monitoramento em segundo plano via Systemd User Timers. O sistema verifica atualizações silenciosamente **a cada 3 horas** e emite notificações nativas via libnotify apenas se houver novos pacotes disponíveis.

2. **Auto-Instalação Dinâmica:** O script possui lógica de autoconfiguração. Ao ser executado, ele valida sua própria persistência no sistema, garantindo que o serviço Sentinela esteja sempre ativo, independente do diretório de instalação.

3. **Mirror Optimization (Reflector):** Otimiza dinamicamente a *mirrorlist* para os 5 servidores HTTPS mais rápidos e sincronizados, maximizando a largura de banda de download.

4. **Integrity & Core Sync (Pacman):** Sincronização profunda dos repositórios oficiais e atualização dos pacotes vitais do sistema.

5. **AUR Intelligence Hub:** Detecção automática de *AUR Helpers*. Possui suporte nativo e inteligente para **Yay** ou **Paru**, permitindo a escolha do motor de atualização em tempo real.

6. **Universal Sandbox Update:** Sincronização completa de aplicações isoladas via **Flatpak** e pacotes universais via **Snapd**, garantindo que nenhum setor do sistema fique desatualizado.

7. **Disk Integrity Reserve:** Auditoria de espaço em disco pré-atualização. Se o SSD estiver com menos de 5GB livres, o script executa uma limpeza de emergência ou aborta o processo para evitar a corrupção de dados.

8. **Auditoria de Núcleo (Kernel & Driver Check):** Varredura em tempo real nos logs do Pacman para detectar alterações críticas em drivers **Nvidia**, **Kernel Linux**, **Mesa** ou **Systemd**.

9. **Purga de Órfãos & Cache:** Localização e remoção de dependências residuais (órfãos) e estabilização de cache mantendo os últimos 3 via `paccache` `paccache -r` `pacman -Sc`, preservando a vida útil do SSD.

10. **Sentinel Logs (FIFO Rotation):** Sistema de telemetria com logs rotativos. O script mantém apenas as últimas 13 sessões de atualização, garantindo histórico para depuração sem poluir o armazenamento.

11. **Protocolo de Notificação Universal:** Ao concluir a sequência de manutenção ou achar uma atualização (modo sentinela ghost), o script dispara um alerta para a interface desktop via `libnotify`. Isso garante que, em **qualquer interface, desktop environment (DE)** mesmo em outra área de trabalho ou focado em outros estudos, você receba a confirmação imediata de que o **Sentinel** finalizou a tarefa ou se alguma atualição foi detectada e que os logs foram gerados.

12.**Notificação Interativa (Modo Sentinela): O daemon em background agora dispara um alerta visual inteligente com um botão "⚡ Click to Launch App". Ao clicar, ele aciona o lançador .desktop nativo e abre o terminal automaticamente na sua frente.** 
    
13. **Sistema de Telemetria (Logs)**
O protocolo mantém dois fluxos de logs independentes:
**~/.logs_arch_update_full/:** Histórico completo das sessões manuais. (retenção de 13 versões)
**~/.logs_sentinel_check/:** Logs técnicos da ronda do sentinela (retenção de 3 versões).

14. **Validação ShellCheck (Certificação de Qualidade)** O Padrão: O código foi passado pelo crivo do ShellCheck e saiu com zero erros. Resultado: Isso garante que a sintaxe do Bash está impecável, as variáveis estão protegidas com aspas e não há riscos de falhas silenciosas por má formação de comandos. É um código blindado.

15.**Smart Connectivity Gatekeeper:** O teste de rede foi aprimorado. O protocolo agora faz um ping primário nos seus mirrors locais. Se não houver resposta, uma segunda tentativa direta no archlinux.org é feita antes de abortar a operação.

16.**Atualização do AUR Híbrida: O controle absoluto está nas suas mãos. Agora você pode escolher o modo de operação na hora de atualizar o AUR:**
**Automático: Executa a atualização rápida (--noconfirm).**
**Manual: Modo interativo onde você pode auditar os PKGBUILDs e confirmar as alterações passo a passo ([!] caso erro de digitação modo manual é executado por padrão).**

---
**Notificações Inteligentes**

---
<img width="535" height="184" alt="botaoclick" src="https://github.com/user-attachments/assets/61031249-977f-4e72-94ca-5dd3139201a2" />
<img width="543" height="167" alt="notificação final" src="https://github.com/user-attachments/assets/472f8e81-ecaf-4f12-b440-569f5af8035d" />



**Alertas desktop em tempo real sobre a disponibilidade de novas atualizações e a confirmação imediata ao concluir o protocolo de manutenção.**




---
## **Interface e Visual :**
**CLI: Estética Neon Blue com logs detalhados e assinatura personalizada.**

**Menu: Integração nativa com os ambientes através do atalho customizado.**

 **⚡ Protocolo Sentinela em Ação:** 
---
<img width="1075" height="700" alt="1" src="https://github.com/user-attachments/assets/e518bd96-1a0b-4d71-891b-5c6f391151ee" />
<img width="1075" height="700" alt="2" src="https://github.com/user-attachments/assets/12531f69-3a59-4252-a737-35117753a633" />
<img width="1075" height="700" alt="3" src="https://github.com/user-attachments/assets/3b4e6489-35b2-4d39-9a32-ca31578f1f0e" />
<img width="1075" height="700" alt="4" src="https://github.com/user-attachments/assets/16b5da16-1121-4c77-8caf-cf3d92b07eca" />
<img width="1075" height="700" alt="5" src="https://github.com/user-attachments/assets/462cb9b6-2f37-41ab-b0e5-1af9bfeaa834" />



### **🚀 Menu do Sistema (Novidade 3.9!)** 
---
<img width="512" height="512" alt="novalogoarchupdatefullv39" src="https://github.com/user-attachments/assets/95b947d3-da51-4098-b1db-477ec0165bb0" />


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
sudo cp novalogoarchupdatefullv39.png /usr/share/pixmaps/
```
**3. Instala o atalho no menu de aplicações (XDG):**
```bash
sudo cp arch-update-full.desktop /usr/share/applications/arch-update-full.desktop
```

---
**𝓓𝓮𝓼𝓮𝓷𝓿𝓸𝓵𝓿𝓲𝓭𝓸  𝓹𝓸𝓻  𝓖𝓾𝓼𝓽𝓪𝓿𝓸  𝓖𝓲𝓪𝓷𝓮𝓵𝓲  (O 𝓢é𝓽𝓲𝓶𝓸)**

**"𝓓𝓮𝓼𝓮𝓷𝓿𝓸𝓵𝓿𝓲𝓭𝓸  𝓹𝓸𝓻  𝓣𝓱𝓮_ 𝓢𝓮𝓿𝓮𝓷𝓽𝓱  —  𝓸𝓷𝓭𝓮  𝓪  𝓲𝓷𝓽𝓮𝓰𝓻𝓲𝓭𝓪𝓭𝓮  𝓮𝓷𝓬𝓸𝓷𝓽𝓻𝓪  𝓪  𝓹𝓮𝓻𝓯𝓸𝓻𝓶𝓪𝓷𝓬𝓮."**

---

**🛡️ Developer Profile (Red Team Focus)**

**Foco do Projeto:** Automação Shell para Manutenção e Auditoria da Base Arch Linux.

**Autor:** Gustavo Gianeli (O Sétimo)

**Educação:** Estudante de Ciência da Computação (entusiasta de Linux e fuçador)

**Hardware:** Acer Nitro V15 | i7 13th Gen | RTX 4050 | 32GB RAM

**Localização:** Ourinhos, SP - Brazil






