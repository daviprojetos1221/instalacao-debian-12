# Configurações Pós-Instalação

1. **Atualize o sistema:**
   ```bash
   sudo apt update
   sudo apt upgrade -y
   ```

2. **Configure o idioma do sistema:**
   ```bash
   sudo dpkg-reconfigure locales
   ```

3. **Configure o horário e fuso horário:**
   ```bash
   sudo dpkg-reconfigure tzdata
   ```

4. **Adicione seu usuário ao grupo sudo (caso ainda não esteja):**
   ```bash
   sudo usermod -aG sudo seu-usuario
   ```

5. **Reinicie o computador para garantir que todas as configurações sejam aplicadas:**
   ```bash
   sudo reboot
   ```