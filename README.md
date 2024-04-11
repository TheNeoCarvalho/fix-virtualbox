## Corrigir erro no VirtualBox

### Execute os comandos abaixo:

Execute seguinte o comando com o usuário `root`.

```
sudo modprobe vboxdrv
```
Depois, atualize o sistema com o seguinte comando:

```
sudo apt update
```

Resinstale os header e depedências necessárias:
```
sudo apt install --reinstall linux-headers-$(uname -r) virtualbox-dkms dkms
```

Execute seguinte o comando com o usuário `root`.
```
sudo modprobe vboxdrv
```
### Desabilitar o "Security Boot" nas configurações da BIOS.

Entre na `BIOS` e na opção `BOOT`, desative o `security boot`.

Salve as alterações realizadas e reiniciei o computador.
