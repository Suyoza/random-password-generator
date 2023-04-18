# random-password-generator
This code generates a random password.

import secrets
import string

def generate_password(length):
    """Génère un mot de passe aléatoire avec une longueur donnée"""
    chars = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(secrets.choice(chars) for i in range(length))
    return password

# Exemple d'utilisation : générer un mot de passe de 12 caractères
password = generate_password(12)
print(password)
