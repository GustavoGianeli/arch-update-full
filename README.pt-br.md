 <img src="https://flagcdn.com/16x12/us.png" alt="US">  [English (US)](README.md) | <img src="https://flagcdn.com/16x12/br.png" alt="BR">  [Português (BR)](README.pt-br.md)
---
***🛡️ Arch Update Full (Protocolo Sentinela)🔄*** **Versão 4.1-1**
---

**Organizador avançado, leve e totalmente automatizado desenvolvido para o Arch Linux. Centraliza atualizações, otimizações de desempenho e auditorias de integridade do sistema..**

**Arch-Update-Full: O Protocolo de Elite para Gestão de Atualizações do Arch Linux. Sincronização inteligente de Pacman, AUR e Flatpaks e Snaps,  com auditoria de integridade em tempo real. Automação absoluta, incluído tudo que é preciso para atualização e manutenções de rotina( pacote órfãos e cache) mas ainda mantendo o controle nas suas mãos.**

---
**🚀 Arch Update Full — Release v4.1-1**

bugs fixes!

Destaques da nova versão do protocolo de automação:

**💡 Observação para Atualizações**
**Após atualizar o pacote pelo AUR/pacman, execute o programa principal uma vez no terminal para que a migração automática do serviço Sentinela seja concluída ou abra o App desktop**

**​⚜️Módulo Sentinela (Notificações Inteligentes):**

Introdução do sistema visual de alertas dinâmicos com ícones exclusivos de faróis em três níveis:
( botão de notificação espera por 37 minutos antes de encerrar como ignorado pelo operado!)

**🔷 Farol Azul: Atualizações de rotina (baixo volume).**

**🔶 Farol Amarelo: Volume moderado de pacotes pendentes.**

**🔴 Farol Vermelho Refatorado:** O ícone do Farol Vermelho passa a ser acionado estritamente por acúmulo de pacotes (=+ 34  pacotes pendentes), garantindo uma hierarquia de alertas mais precisa e clara para o usuário.
( botão de notificação espera por 37 minutos antes de encerrar como ignorado pelo operado!)

**🐧 Novo Ícone Especial & Ajustes na Lógica do Farol** Novo Ícone Tux com Ferramentas: Adicionada uma notificação especial e exclusiva com o ícone do Tux segurando chave e engrenagem para sinalizar atualizações de Kernel e Drivers de Vídeo (GPU).

**⚡ Suporte Oficial ao Pikaur:**

Além do yay e paru, agora o script conta com integração completa e nativa para o helper pikaur, expandindo a compatibilidade para os usuários do AUR.

**🧱 Arquitetura Modular & Sentinela Isolado:**

* Desacoplamento de Módulos: O modo Sentinela foi separado do script principal e agora possui seu próprio binário dedicado (arch-update-full-sentinela), reduzindo drasticamente o tamanho do script interativo.

* Eliminação de Race Condition (Modo Corrida): Fim dos conflitos de execução entre a interface do usuário e as verificações automáticas em segundo plano.

* Operação Fantasma Otimizada: O Sentinela executa a cada 3 horas via systemd --user de forma 100% invisível e sem necessidade de sudo, emitindo notificações apenas quando houver atualizações pendentes.

* Mecanismo de Auto-Reparo (Self-Healing): O script principal agora identifica configurações antigas do systemd e atualiza automaticamente os arquivos de serviço e timer para o novo caminho na primeira execução pós-atualização.

**📰 Arch Linux News Integrado:**
Agora você pode ler a última notícias oficiais do Arch Linux diretamente pelo terminal dentro do arch-update-full, garantindo que você saiba de intervenções manuais antes de atualizar.

**🌐 Refletor de Espelhos Interativo:**
A otimização de mirrors via reflector foi aprimorada: agora o sistema pergunta explicitamente se você deseja otimizar os espelhos na sessão, dando total controle da rede ao usuário.

**🎨 UI/UX Terminal Renovada & Preparação para detecção automática do idioma:**
Interface CLI limpa, moderna e minimalista, utilizando paleta em tons Neon para máxima legibilidade.
**O código base foi estruturado para suportar detecção automática do idioma do sistema em atualizações futuras, exibindo o terminal diretamente em PT-BR ou EN-US.**

**🌐 Suporte Multi-Idioma em Andamento: Início da reestruturação do código para identificar automaticamente a linguagem padrão do sistema operacional. Linguagens Suportadas no Roadmap: Estruturação inicial para suporte a PT-BR (Português), EN-US (Inglês) e ES-ES (Espanhol)..**

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

**🛡️ Arch Update Full: Sentinel Protocol (v4.1)**

O arch-update-full evoluiu de um simples script para um ecossistema de manutenção autônomo. Agora, ele executa uma sequência rigorosa de 16 camadas de integridade e inteligência, garantindo que o seu Arch Linux esteja sempre na vanguarda da performance e segurança:

### 🚀 Camadas de Integridade e Inteligência 

1. **Modo Sentinela (Silent Interception)**: Implementação de monitoramento em segundo plano via Systemd User Timers. O sistema verifica atualizações silenciosamente **a cada 3 horas** e emite notificações nativas via libnotify apenas se houver novos pacotes disponíveis.

2. **Auto-Instalação Dinâmica:** O script possui lógica de autoconfiguração. Ao ser executado, ele valida sua própria persistência no sistema, garantindo que o serviço Sentinela esteja sempre ativo, independente do diretório de instalação.

3. **Mirror Optimization (Reflector):** Otimiza dinamicamente a *mirrorlist* para os 5 servidores HTTPS mais rápidos e sincronizados, maximizando a largura de banda de download.

4. **Integrity & Core Sync (Pacman):** Sincronização profunda dos repositórios oficiais e atualização dos pacotes vitais do sistema.

5. **AUR Intelligence Hub:** Detecção automática de *AUR Helpers*. Possui suporte nativo e inteligente para **Yay**,**PikAur** ou **Paru**, permitindo a escolha do motor de atualização em tempo real.

6. **Universal Sandbox Update:** Sincronização completa de aplicações isoladas via **Flatpak** e pacotes universais via **Snapd**, garantindo que nenhum setor do sistema fique desatualizado.

7. **Disk Integrity Reserve:** Auditoria de espaço em disco pré-atualização. Se o SSD estiver com menos de 5GB livres, o script executa uma limpeza de emergência ou aborta o processo para evitar a corrupção de dados.

8. **Auditoria de Núcleo (Kernel & Driver Check):** Varredura em tempo real nos logs do Pacman para detectar alterações críticas em drivers **Nvidia**, **AMD** **Kernel Linux**, **Mesa** ou **Systemd**.

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
<img width="533" height="178" alt="imagem aviso de kernel" src="https://github.com/user-attachments/assets/2b922164-af33-4afc-92bd-3b8a02656f6d" />

<img width="543" height="167" alt="notificação final" src="https://github.com/user-attachments/assets/472f8e81-ecaf-4f12-b440-569f5af8035d" />

---
**Alertas desktop em tempo real sobre a disponibilidade de novas atualizações e a confirmação imediata ao concluir o protocolo de manutenção.**

**Logica de uso dos ícones:**

<img width="1200" height="896" alt="novo funcionamento arch " src="https://github.com/user-attachments/assets/b5507f91-90db-4e78-a0d6-573961bdae8f" />

---
## **Interface e Visual :**
**CLI: Estética Neon Blue com logs detalhados e assinatura personalizada.**

**Menu: Integração nativa com os ambientes através do atalho customizado.**

 **⚡ Protocolo Sentinela em Ação:** 
---

<img width="1043" height="747" alt="1 Imagem colada" src="https://github.com/user-attachments/assets/df6ae414-718d-47ee-b334-dc2d21dd03b6" />
<img width="1043" height="747" alt="2" src="https://github.com/user-attachments/assets/e9038c8c-297e-4ad9-b90f-f00ed143e451" />
<img width="1043" height="747" alt="3" src="https://github.com/user-attachments/assets/7a6f3728-d329-476c-b783-dbaf0a26f211" />
<img width="1043" height="747" alt="4" src="https://github.com/user-attachments/assets/0fb28535-8f00-415e-992c-a2d472fe58f8" />
<img width="1043" height="747" alt="5" src="https://github.com/user-attachments/assets/46f9d7e9-16dc-42b6-991b-f99b12da7ecb" />
<img width="1069" height="763" alt="6" src="https://github.com/user-attachments/assets/5ca7eb8c-223e-494f-9f6a-df78250c7685" />
<img width="1069" height="763" alt="7" src="https://github.com/user-attachments/assets/22149649-305c-42f9-a0e4-752ff971da4e" />
<img width="1090" height="829" alt="8" src="https://github.com/user-attachments/assets/5a0c2736-dd08-45a0-b4ea-649df156846e" />

https://github.com/user-attachments/assets/031f683f-5628-4a40-aef4-98ed4a6cef47

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

**➡ Para usar o script como um comando nativo e ter o atalho no seu menu de aplicativos, execute os seguinte comando:**
```bash
git clone https://aur.archlinux.org/arch-update-full.git
cd arch-update-full
makepkg -si
```
---

**"Created By: 𝕿𝖍𝖊 S𝖊𝖛𝖊𝖓𝖙𝖍  —  𝓸𝓷𝓭𝓮  𝓪  𝓲𝓷𝓽𝓮𝓰𝓻𝓲𝓭𝓪𝓭𝓮  𝓮𝓷𝓬𝓸𝓷𝓽𝓻𝓪  𝓪  𝓹𝓮𝓻𝓯𝓸𝓻𝓶𝓪𝓷𝓬𝓮."**

---

**🛡️ Developer Profile (Red Team Focus)**

**Foco do Projeto:** Automação Shell para Manutenção e Auditoria da Base Arch Linux.

**Autor:** Gustavo Gianeli (O Sétimo)

**Educação:** Estudante de Ciência da Computação (entusiasta de Linux e fuçador)







