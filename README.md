<h3 align="center"><strong>Obtén imágenes, textos y gifs del tipo anime para comandos de acción, reacción y diversión o para los que quieras, además 100% en español y muy facil de usar.</strong></h3>

## Instalación ⚙

Descargar el proyecto y ponerlo en la carpeta de **node_modules**

Intalación automatica proximamente
```bash
$ npm install 
```

## Usos ✨
### Gifs 😺
#### Verificar que funcione 🔒
```javascript
const animaction = require('animaction')
const wag = animaction.wag()
const dance = animaction.dance()

console.log(dance) /* Obtiene un gif de Wag */
console.log(wag)  /* Obtiene un gif de Dance  */
```

#### En un bot de Discord 🤖
```javascript
const animaction = require("animaction");
const Discord = require("discord.js");
const client = new Discord.Client();

client.on("message", async message => {
  /* Solo el gif, en este caso un gif de Wag */
  if (message.content === "comun") {
    const wag = animaction.wag();
    message.channel.send(wag);
  }
  /* En un embed (Discord.JS Version 12) en este caso un gif de Dance */
  if (message.content === "embed") {
    const dance = animaction.dance();
    const animaction_embed = new Discord.MessageEmbed()
        .setTitle('Vamos a bailar!!')
        .setImage(dance)
        .setFooter('Potenciado por animaction');
    message.channel.send(animaction_embed);
  }
});

client.login("BOT_TOKEN");
```
### Texto 😺
#### Verificar que funcione 🔒
```javascript
const animaction = require('animaction')
const answer = animaction.facts()

console.log(facts) /* Devuelve una dato curioso */
```

#### En un bot de Discord 🤖
```javascript
const animaction = require("animaction");
const Discord = require("discord.js");
const client = new Discord.Client();

client.on("message", async message => {
  /* Devuelve una dato curioso */
  if (message.content === "comun") {
    const facts = animaction.facts();
    message.channel.send(facts);
  }
  /* Devuelve la respuesta en un embed (Discord.JS Version 12)  */
  if (message.content === "embed") {
    const answer = animaction.facts();
    const animaction_embed = new Discord.MessageEmbed()
        .setTitle('Lo sabias')
        .setDescription(facts)
        .setFooter('Potenciado por animaction');
    message.channel.send(animaction_embed);
  }
});

client.login("BOT_TOKEN");
```
### Imagenes 😺
#### Verificar que funcione 🔒
```javascript
const animaction = require('animaction')
const anime = animaction.anime()

console.log(anime) /* Devuelve una imagen al azar de un anime */
```

#### En un bot de Discord 🤖
```javascript
const animaction = require("animaction");
const Discord = require("discord.js");
const client = new Discord.Client();

client.on("message", async message => {
  /* Solo la imagen al azar de un anime */
  if (message.content === "comun") {
    const anime = animaction.anime();
    message.channel.send(anime);
  }
  /* En un embed (Discord.JS Version 12) devuelve la imagen al azar de un anime */
  if (message.content === "embed") {
    const anime = animaction.anime();
    const animaction_embed = new Discord.MessageEmbed()
        .setTitle('Imagen de un anime')
        .setImage(anime)
        .setFooter('Potenciado por animaction');
    message.channel.send(animaction_embed);
  }
});

client.login("BOT_TOKEN");
```

## Opciones 🧰
### Gifs 😺
**Opción** | **Tipo** | **Descripción** | **Uso**
:---: | --- | --- | ---
wag | Gif | Bate la cola owo | `animaction.wag()`
dance | Gif | Bailemos!! | `animaction.dance()`
sip | Gif | Bebe algo | `animaction.sip()`
### Texto 😺
**Opción** | **Tipo** | **Descripción** | **Uso**
:---: | --- | --- | ---
facts | Texto | Devuelve un dato | `animaction.facts()`
catfacts | Texto | Devuelve un dato sobre los gatos | `animaction.catfacts()`
topics | Texto | Devuelve un tema de conversasión | `animaction.topics()`
### Imagenes 😺
**Opción** | **Tipo** | **Descripción** | **Uso**
:---: | --- | --- | ---
anime | Imagen | Devuelve una imagen al azar de un anime .w. | `animaction.anime()`

## Actualizaciónes ⭐

```lua
Animaction
├── v0.0.1
│   └── 📦 Lanzada oficialmente.
├── v0.0.2
|   ├── ⭐ Cambios.
|   │    ├── Se agrego una nueva acción Sip.
|   │    └── Se añadieron mas gifs a las acciones existentes, para un total de 20 x acción.
|   └── ⭐ Correcciones.
|        └── Se reparo la accióm Dance.
└── v0.0.3     
    ├── ⭐ Cambios.
    │    ├── Se agregaron nuevas funciones de texto > topics, catfacts y facts.
    │    └── Se añadieron mas gifs a las acciones existentes, para un total de 25 x acción.
    ├── ⭐ Remociones.
    │    └── Se elimino la función answers.
    └── ⭐ Correcciones.
         └── Se reparo la funcion anime.
```


## Ayuda extra 🎫
- Puedes encontrar ayuda detallada en el mismo servidor de soporte de mi bot clickeando [aqui](https://discord.gg/QR6xQbTNab)
- Puedes ahorrar trabajo utilizando los archivos en la carpeta [templates](https://github.com/KitsuneCode/animaction/tree/main/templates)
- Puedes apoyarme tambien invitando a mi bot [aqui](https://discord.com/oauth2/authorize?client_id=831865259357896755&permissions=8&scope=bot)

## Licensia 🗃
[MIT](https://github.com/KitsuneCode/animaction/blob/main/LICENSE) © [KitsuneCode](https://kitsunecode.glitch.me) con 🧡
