# Criando um Pendrive Bootável

## No Windows

1. Baixe e instale o [Rufus](https://rufus.ie/).
2. Insira o pendrive.
3. Abra o Rufus.
4. Selecione o pendrive na opção "Dispositivo".
5. Clique em "Selecionar" e escolha a ISO do Debian baixada.
6. Mantenha as opções padrão (Sistema de arquivos: FAT32, Esquema de partição: MBR ou GPT conforme seu sistema).
7. Clique em "Iniciar" e aguarde o processo terminar.

## No Linux

1. Insira o pendrive.
2. Descubra o caminho do pendrive:  
   `lsblk`
3. Use o comando (substitua `/dev/sdX` pelo seu pendrive):

   ```bash
   sudo dd if=/caminho/para/debian.iso of=/dev/sdX bs=4M status=progress
   sync
   ```

4. Aguarde o processo terminar antes de remover o pendrive.

**Atenção:** O comando `dd` apaga todo o conteúdo do pendrive.