# arch-update-full
Um automatizador de atualizações para o arch linux 


# 🚀 Arch Update Full - Protocolo Cyberpunk
### Desenvolvido por Gustavo Gianeli (Sétimo) 

Este é um script de automação e manutenção completa para usuários de **Arch Linux**. Ele unifica a atualização de pacotes oficiais, AUR, Flatpaks e realiza uma limpeza profunda no sistema para manter a performance em nível máximo.

---

## 🛠️ O que o protocolo faz?
- [x] **Sincronização Total:** Atualiza a base de dados e pacotes do sistema (`pacman`).
- [x] **Injeção AUR:** Atualiza programas do Arch User Repository usando o `yay`.
- [x] **Sandboxing:** Verifica e atualiza todos os aplicativos `Flatpak`.
- [x] **Purga de Fragmentos:** Remove pacotes órfãos (desnecessários) automaticamente.
- [x] **Otimização de Cache:** Limpa versões antigas de pacotes baixados para economizar SSD.
- [x] **Interface Visual:** Estética Neon Blue/Cyberpunk no terminal com assinatura personalizada.

---
## 📸 Demonstração Visual

### ⚡ Protocolo Sétimo em Ação

<img width="2560" height="1440" alt="print2" src="https://github.com/user-attachments/assets/e1bacc88-e26b-4572-92a7-2de61826b2a9" />
<img width="2560" height="1440" alt="print3" src="https://github.com/user-attachments/assets/d0b36d25-4700-4334-aecb-ff4b1c0e60e0" />

### 🚀 Atalho no Menu do Sistema

<img width="788" height="410" alt="print1" src="https://github.com/user-attachments/assets/bba5d8ab-dd11-44a5-b764-73c2f4e6bc11" />


## 🚀 Como Instalar Manualmente

Para usar o script como um comando nativo e ter o atalho no seu menu de aplicativos, rode os seguintes comandos no terminal:

### 1. Configure o Executável e o Atalho
```bash
sudo cp arch-update-full /usr/bin/arch-update-full
sudo chmod 755 /usr/bin/arch-update-full
sudo cp arch-update-full.desktop /usr/share/applications/




