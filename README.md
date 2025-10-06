# Pulpo
Configuracion de HomeServer local para experimentos de ciberseguridad

#Configura un usuario no-root (si no lo hiciste):
Por seguridad, usa un usuario normal con privilegios sudo en lugar de root. Si no tienes uno, créalo:

sudo adduser casa
sudo usermod -aG sudo casa

#2. Configurar acceso remoto desde la laptop (Windows 11)
Configuraremos SSH en Kali para que puedas gestionarlo desde tu laptop con Windows 11.

Instala y configura OpenSSH en Kali:
sudo apt install openssh-server -y

Edita el archivo de configuración SSH:
sudo nano /etc/ssh/sshd_config
sudo systemctl enable ssh  # Habilita en arranque

Obtén la IP del servidor:
En Kali, ejecuta:
ip addr show

Conecta desde Windows 11:
En la laptop, usa la terminal (PowerShell o CMD):
ssh nombre_usuario@IP_del_servidor





