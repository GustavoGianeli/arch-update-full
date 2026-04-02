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


## 🚀 Como Instalar Manualmente

Para usar o script como um comando nativo e ter o atalho no seu menu de aplicativos, rode os seguintes comandos no terminal:

### 1. Configurar o Executável Para Aparecer como um App
```bash
sudo cp arch-update-full /usr/bin/arch-update-full
sudo chmod 755 /usr/bin/arch-update-full
sudo cp arch-update-full.desktop /usr/share/applications/

