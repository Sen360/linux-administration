# linux-administration
Scripts Bash pour gérer Linux (utilisateurs, services, sauvegardes).

#!/bin/bash
for i in {1..5}; do
    sudo useradd -m -s /bin/bash user$i
    echo "user$i:P@ssw0rd" | sudo chpasswd
    echo "Utilisateur user$i créé avec succès !"

