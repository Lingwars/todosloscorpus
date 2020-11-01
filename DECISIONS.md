# Decisiones
Aquí recogemos las decisiones que hemos tenido que ir tomando en Discord.

## ¿Qué hacer con el género y el número?
Para que puedan usarse de forma combinada con adjetivos, determinantes, etc. en español necesitamos saber qué genero y número tiene cada palabra (en el caso de nombres, adjetivos y verbos). Así que vamos a etiquetar cada una de las palabras de este tipo.

Estamos usando estas etiquetas para el género:
- "c" si la palabra se puede usar tanto en femenino como en masculino
- "f" si la palabra solo se puede usar en femenino
- "m" si la palabra solo se puede usar en masculino

Y estas etiquetas para el número:
- "c" si la palabra se puede usar tanto en singular como en plural
- "p" si la palabra solo se puede usar en plural
- "s" si la palabra solo se puede usar en singular

De todas formas, esto no significa que haya que desdoblar todas las palabras en todos sus posibles géneros y números, solamente etiquetarlas.

Dos ejemplos:

1)
- Original en inglés
```
        {
            "member": "grandparent",
            "inverse": "grandchild"
        }
```
En español
```
        {
            "member": {
                "name": "abuelo",
                "gender": "m"
            }
            "inverse": {
                "name": "nieto",
                "gender": "m"
            }
        }
```
Es posible que quieras añadir también relación abuela/nieta, pero no es obligado, aunque en casos como yerno/nuera probablemente sí, ya que es una forma muy diferente.

2)
- Original en inglés
```
[
    "ant",
    "shark",
    "rhino",
    "lion"
]
```
- En español
```
[
    {
        "name": "hormiga",
        "gender": "f",
        "number": "s"
    },
    {
        "name": "tiburón",
        "gender": "m",
        "number": "s"
    },
    {
        "name": "rinoceronte",
        "gender": "c",
        "number": "s"
    },
    {
        "name": "león",
        "gender": "m",
        "number": "s"
    },
    {
        "name": "leona",
        "gender": "f",
        "number": "s"
    }
]
```

## ¿Puede estar una misma palabra en dos listados diferentes?
Si tiene sentido, ¡sí! Por ejemplo, "ansiedad" es una palabra de uso común, pero también es un término médico, así que podría estar tanto en un fichero de nombres comunes (words/nouns.json) como en uno de, ponte tú, medicina (medicine.json).

## ¿Qué hacer con los duplicados en un mismo fichero?
Elimínalos sin problema, no tiene sentido que haya duplicados

## ¿Hacemos pull request por fichero?
¡Vale! Así vamos incorporando los cambios de forma más controlada.
