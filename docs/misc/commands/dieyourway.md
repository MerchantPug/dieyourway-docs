---
title: /dieyourway (Command)
date: 2021-07-13
---

# `/dieyourway`

The `/dieyourway` command can be used to test dieyourway files' messages. You can get a random message or you can get a message at a specific index.

### Syntax:

```mcfunction
dieyourway <file>
```
Fetch a random message .
<br>

* `<file>` being the namespace and ID of a Die Your Way file
    * (e.g: `biomedeaths:savannah` (`data/biomedeaths/dieyourway/savannah.json`))
<br>
<br>

```mcfunction
dieyourway <file> <index>
```
Fetches a specific message from a specific file.
<br>

* `<file>` being the namespace and ID of a Die Your Way file
    * (e.g: `biomedeaths:savannah` (`data/biomedeaths/dieyourway/savannah.json`))
* `<index>` being the integer that corresponds to the message in the `messages` tag. (This starts at 1 and ends at however many messages are in your file)
<br>
<br>