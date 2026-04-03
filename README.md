# 🟦 Protocolo Cyberpunk: arch-update-full (v2.0)

**"Automação é a fundação da soberania digital."** > Script desenvolvido para centralizar a manutenção crítica de sistemas baseados em Arch Linux.


# 🚀 Arch Update Full - Protocolo Cyberpunk
### Desenvolvido por Gustavo Gianeli (Sétimo) 

Este é um script de automação e manutenção completa para usuários de **Arch Linux**. Ele unifica a atualização de pacotes oficiais, AUR, Flatpaks e também Snaps e realiza uma limpeza profunda no sistema para manter a performance em nível máximo.

# 🛠️ Arquitetura do Protocolo (Core Functions)

O **arch-update-full** executa uma sequência rigorosa de sete camadas de integridade:

1.  **Mirror Optimization (Reflector):** [NOVO v2.0] Verifica e atualiza a lista de espelhos para os servidores mais rápidos e sincronizados, garantindo downloads em alta velocidade.
2.  **Sincronização de Base (Pacman):** Atualiza os repositórios oficiais e pacotes core do sistema.
3.  **Injeção de Pacotes AUR (Yay):** Gerencia e compila atualizações da comunidade de forma automatizada.
4.  **Sandboxing Update (Flatpak):** Verifica e aplica patches em aplicações isoladas via Flatpak.
5.  **Snap Deployment (Snapd):** [NOVO v2.0] Sincroniza e atualiza pacotes universais via Snap.
6.  **Purga de Órfãos:** Localiza e remove dependências não utilizadas, otimizando a árvore de pacotes.
7.  **Otimização de Cache:** Limpa o cache de pacotes para preservar o SSD e liberar espaço em disco.

---

## 🚀 Instalação Oficial (AUR)
# Disponível no AUR: yay -S arch-update-full
<img width="2101" height="501" alt="print aur" src="https://github.com/user-attachments/assets/28061db4-76b2-4168-a194-f1aa6d2e73c1" />


---
## 📸 Interface e Visual
CLI: Estética Neon Blue com logs detalhados e assinatura personalizada.

Menu: Integração nativa com ambientes GNOME/KDE através do atalho customizado.

Demonstração Visual

### ⚡ Protocolo Sétimo em Ação
<img width="1282" height="863" alt="print 1" src="https://github.com/user-attachments/assets/c0942c06-c07a-4fe7-8a44-be14cbf003db" />
<img width="1282" height="863" alt="print 2" src="https://github.com/user-attachments/assets/031fedfc-0568-4f98-9b00-803e14bd8ca8" />

### 🚀 Menu do Sistema (v2.0) — Ícone Personalizado
<img width="233" height="232" alt="print logo" src="https://github.com/user-attachments/assets/9176294e-bfbf-42bd-a4af-9fb9cfe4fee5" />



### 🚀 Como Instalar Manualmente

Para usar o script como um comando nativo e ter o atalho no seu menu de aplicativos, execute os seguintes comandos:

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


🛡️ Developer Profile (Red Team Focus)
"Projeto focado em Automação Shell e Segurança da Informação."

Autor: Gustavo Gianeli (Sétimo)

Hardware: Acer Nitro V15 | i7 13th Gen | RTX 4050 | 32GB RAM

Location: Ourinhos, SP - Brazil
