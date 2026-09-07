 <img src="https://flagcdn.com/16x12/us.png" alt="US">  [English (US)](README.md) | <img src="https://flagcdn.com/16x12/br.png" alt="BR">  [Português (BR)](README.pt-br.md)
---
***🛡️ Arch Update Full (Protocolo Sentinela)🔄*** **Versão 4.0**
---

**Organizador avançado, leve e totalmente automatizado desenvolvido para o Arch Linux. Centraliza atualizações, otimizações de desempenho e auditorias de integridade do sistema..**

**Arch-Update-Full: O Protocolo de Elite para Gestão de Atualizações do Arch Linux. Sincronização inteligente de Pacman, AUR e Flatpaks e Snaps,  com auditoria de integridade em tempo real. Automação absoluta, incluído tudo que é preciso para atualização e manutenções de rotina( pacote órfãos e cache) mas ainda mantendo o controle nas suas mãos.**

---
**🚀 Novidades: Arch Update Full v: 4.0**
Destaques da nova versão do protocolo de automação:

**Módulo Sentinela (Notificações Inteligentes):**
Introdução do sistema visual de alertas dinâmicos com ícones exclusivos de faróis em três níveis:

**🔷 Farol Azul: Atualizações de rotina (baixo volume).**

**🔶 Farol Amarelo: Volume moderado de pacotes pendentes.**

**🔴 Farol Vermelho / Kernel Tux: Alerta crítico (Kernel, drivers NVIDIA/Mesa, Systemd) exigindo atenção e sugerindo reboot do sistema.**

**⚡ Suporte Oficial ao Pikaur:**
Além do yay e paru, agora o script conta com integração completa e nativa para o helper pikaur, expandindo a compatibilidade para os usuários do AUR.

**🧱 Arquitetura Modular (Código Refatorado):**
O código deixou de ser um script monobloco extenso e foi totalmente reconstruído em funções independentes e legíveis, orquestradas por uma função main() limpa e performática.

**📰 Arch Linux News Integrado:**
Agora você pode ler a última notícias oficiais do Arch Linux diretamente pelo terminal dentro do arch-update-full, garantindo que você saiba de intervenções manuais antes de atualizar.

**🌐 Refletor de Espelhos Interativo:**
A otimização de mirrors via reflector foi aprimorada: agora o sistema pergunta explicitamente se você deseja otimizar os espelhos na sessão, dando total controle da rede ao usuário.

**🎨 UI/UX Terminal Renovada & Preparação para detecção automática do idioma:**
Interface CLI limpa, moderna e minimalista, utilizando paleta em tons Neon para máxima legibilidade.
**O código base foi estruturado para suportar detecção automática do idioma do sistema em atualizações futuras, exibindo o terminal diretamente em PT-BR ou EN-US.**

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
**➡ Instalação via Pikaur:**
```bash
pikaur -S arch-update-full
```

---
# **Arquitetura do Protocolo (Core Functions):**
**🛡️ Arch Update Full: Sentinel Protocol (v4.0)**

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

12.**Notificação Interativa (Modo Sentinela AGORA com ícones personalizados para notificar): O daemon em background agora dispara um alerta visual inteligente com um botão "Click to Launch App". Ao clicar, ele aciona o lançador .desktop nativo e abre o terminal automaticamente na sua frente.** 
    
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
<img width="620" height="241" alt="notificação sentila azul" src="https://github.com/user-attachments/assets/6c33de62-1567-4165-a4b4-6c99276b0175" />

<img width="678" height="261" alt="notificação vermelha" src="https://github.com/user-attachments/assets/661f8cb3-0631-441d-9dea-649ed53f284e" />

<img width="543" height="167" alt="notificação final" src="https://github.com/user-attachments/assets/472f8e81-ecaf-4f12-b440-569f5af8035d" />

**Alertas desktop em tempo real sobre a disponibilidade de novas atualizações e a confirmação imediata ao concluir o protocolo de manutenção.**

**Logica de uso dos ícones:**

<img width="1254" height="1254" alt="logica farol atualizado" src="https://github.com/user-attachments/assets/407f6146-b462-4300-bb2a-dfe3a87c8db7" />



---
## **Interface e Visual :**
**CLI: Estética Neon Blue com logs detalhados e assinatura personalizada.**

**Menu: Integração nativa com os ambientes através do atalho customizado.**

 **⚡ Protocolo Sentinela em Ação:** 
---

<img width="1165" height="863" alt="1" src="https://github.com/user-attachments/assets/925ed2c6-e6fd-4c22-b515-c82c774ce377" />
<img width="1165" height="863" alt="2" src="https://github.com/user-attachments/assets/b1553c7b-e0de-4350-b877-b0b026f190e0" />
<img width="1165" height="863" alt="3" src="https://github.com/user-attachments/assets/d65a37d8-fab0-4553-8d37-748a17bfa610" />
<img width="1165" height="863" alt="4" src="https://github.com/user-attachments/assets/d80391e3-ca48-4b37-a767-b26e3f2069df" />
<img width="1165" height="863" alt="5" src="https://github.com/user-attachments/assets/59631110-0e65-42bc-898c-083ebb9576e2" />
<img width="1165" height="863" alt="6" src="https://github.com/user-attachments/assets/6004057e-4d4e-4a83-a594-ed0c38e6a6d6" />
<img width="1165" height="863" alt="7" src="https://github.com/user-attachments/assets/4fcca75b-0045-4c7f-9458-82f199e56d94" />
<img width="1165" height="863" alt="8" src="https://github.com/user-attachments/assets/47cdd17e-7a53-47a6-8044-85e770431e74" />
<img width="1165" height="863" alt="9" src="https://github.com/user-attachments/assets/5e88660b-74ac-4554-9b80-14bd40a90bed" />

https://github.com/user-attachments/assets/a4ff6b85-45d6-49a7-9239-4b07692c0f02


### **🚀 Menu do Sistema** 
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
**4. Instala os ícones do Módulo Sentinela (Faróis de Notificação):**
```bash
sudo mkdir -p /usr/share/arch-update-full/icons
sudo cp farol_azul_simbolo.png /usr/share/arch-update-full/icons/
sudo cp farol_amarelo_simbolo.png /usr/share/arch-update-full/icons/
sudo cp farol_vermelho_simbolo.png /usr/share/arch-update-full/icons/
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






