# Cómo colaborar

## 1. Elegir un fichero

Puedes navegar por [el repositorio de darius](http://github.com/dariusk/corpora) a ver qué fichero te llama la atención, o quizá se te ocurra alguna idea que no exista allí (listado de CCAA de España, por ejemplo).

## 2. Descargar el fichero

Si sabes git, clona el repo de darius, clona este repo, copia el fichero en la misma ruta. Si es nuevo, colócalo donde tenga sentido.

Si no sabes git, una vez estés viendo el fichero en [el repo de darius](http://github.com/dariusk/corpora), pulsa en el botón `Raw` encima y a la derecha del código. Una vez veas el código en pantalla sin más adorno, ve a `Archivo > Guardar` en tu navegador para descargar el fichero. A continuación consulta [Editar el fichero en local](#3a-editar-el-fichero-en-local).

También puedes pedirle a alguien en [el Discord](https://discord.gg/gWxrvdh) que te lo copie en este repo. Si es así, baja a [Editar en el navegador](#3b-editar-en-el-navegador).

## 3a. Editar el fichero en local

Para editar el fichero en tu ordenador, asegúrate de usar un editor de textos y no un procesador de textos.

Editores de texto válidos son el Bloc de notas, Textedit, Notepad++, Sublime Text... Procesadores de texto no válidos son Word, Libreoffice, Google Docs...

## 3b. Editar en el navegador

Si solicitaste ayuda para que te subiesen el fichero al repo de Todos Los Corpus, te pasarán la dirección del fichero ya en nuestro repositorio. Pulsa en el lápiz encima y a la derecha del código (cerca de la zona donde pulsaste antes `Raw`) para comenzar a editarlo. 

## 4. El formato JSON

Los ficheros están en formato JSON. Es muy importante que respetes caracteres como comillas, llaves, comas y dos puntos.

Además, lo que va antes de los dos puntos se llama _clave_ y has de mantenerlo en inglés. Lo que va después se llama _valor_ y eso es lo que has de traducir, _siempre que vaya entre comillas_, de lo contrario déjalo como está.

Por ejemplo, este pedazo del listado de santos:

```
[
    {
        "saint": "Abadiu of Antinoe",
        "birth": "",
        "death": "4th century",
        "canonization": "",
        "anglican": false,
        "oriental_orthodox": true,
        "eastern_orthodox": true,
        "roman_catholic": true
    },
    {
        "saint": "Abakuh",
        "birth": "",
        "death": "Unknown",
        "canonization": "",
        "anglican": false,
        "oriental_orthodox": false,
        "eastern_orthodox": true,
        "roman_catholic": true
    }
]
```

Podríamos traducirlo así:

```
[
	{
		"saint": "Abadiu de Antinoe",
		"birth": "",
		"death": "Siglo IV",
		"canonization": "",
		"anglican": false,
		"oriental_orthodox": true,
		"eastern_orthodox": true,
		"roman_catholic": true
	},
	{
		"saint": "Abakuh",
		"birth": "",
		"death": "Desconocida",
		"canonization": "",
		"anglican": false,
		"oriental_orthodox": false,
		"eastern_orthodox": true,
		"roman_catholic": true
	}
]
```

Fíjate que dejamos intactos los símbolos (llaves etc), las claves, y los valores no entrecomillados.

## 5. Subir los cambios

Si sabes git, comitea y empuja tus cambios a tu repo y haz una pull request.

Si no sabes git y descargaste el fichero para editarlo en local, pide ayuda [en Discord](https://discord.gg/gWxrvdh) para que alguien lo suba al repositorio por ti.

Si no sabes git y estabas editando el fichero en el navegador, una vez termines y repases bien, verás que al final de la página hay un pequeño formulario. Escribe un mensaje corto en inglés en el primer campo de texto (por ejemplo, "Translate list of rooms") y dale a `Propose changes`. No es necesario que cambies el nombre de la rama.

## 6. Confirmar cambios

¡Listo! Avisa por [el Discord](https://discord.gg/gWxrvdh) de que terminaste para que todos te felicitemos y agradezcamos tu trabajo. ¡Eres une hacha!
