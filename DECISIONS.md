# Decisiones
Aquí recogemos las decisiones que hemos tenido que ir tomando en Discord.

## ¿Qué hacer con el género?
Para que puedan usarse de forma combinada con adjetivos, determinantes, etc. en español necesitamos saber qué genero tiene cada palabra (en el caso de nombres y adjetivos). Así que vamos a desdoblarlo, etiquetando cada una de las palabras:
- "c" si la palabra se puede usar tanto en femenino como en masculino
- "f" si la palabra solo se puede usar en femenino
- "m" si la palabra solo se puede usar en masculino

Dos ejemplos:
```
        {
            "member": {
                "m": "abuelo",
                "f": "abuela"
            }
            "inverse": {
                "m": "nieto",
                "f": "nieta"
            }
        }
```

```
[
    {
        "name": "hormiga",
        "gender": "f"
    },
    {
        "name": "tiburón",
        "gender": "m"
    },
    {
        "name": "rinoceronte",
        "gender": "c"
    },
    {
        "name": "león",
        "gender": "m"
    },
    {
        "name": "leona",
        "gender": "f"
    }
]
```

## ¿Puede estar una misma palabra en dos listados diferentes?
Si tiene sentido, ¡sí! por ejemplo, "ansiedad" es una palabra de uso común, pero también es un término médico, así que podría estar tanto en un fichero de nombres comunes (words/nouns.json) como en uno de, ponte tú, medicina (medicine.json).

## ¿Qué hacer con los duplicados en un mismo fichero?
Elimínalos sin problema, no tiene sentido que haya duplicados

## ¿Hacemos pull request por fichero?
¡Vale! Así vamos incorporando los cambios de forma más controlada.
