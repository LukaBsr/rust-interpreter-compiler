**# Simple Practice Language (SPL)**

## Fonctionnalités

- **Variables:** Support pour les types entier (`int`) et booléen (`bool`).
- **Fonctions:** Définir et appeler des fonctions avec des paramètres et des valeurs de retour.
- **Contrôle de flux:** Instructions conditionnelles (`if-else`) et boucles (`while`).
- **Entrée/Sortie:** Opérations basiques d'entrée et de sortie.
- **Commentaires:** Commentaires sur une seule ligne (`//`) et sur plusieurs lignes (`/* */`) pris en charge.
- **Constantes:** Déclarer des constantes en utilisant `const`.

## Exemple

Voici un programme simple en **SPL** :

```rust
// Exemple de langage de pratique simple

fn main() {
    let x = 10;
    let y = 20;
    let result = add(x, y);
    print(result);
}

fn add(a: int, b: int) -> int {
    return a + b;
}

fn print(value: int) {
    // Fonction d'impression pour afficher la valeur
    // Pour simplifier, nous allons simplement imprimer sur la console
    println("Le résultat est : ", value);
}
