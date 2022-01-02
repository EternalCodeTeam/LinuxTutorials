# Instalacja node.js

Aktualizujemy linuxa.

```java
sudo apt update && sudo apt upgrade -y
```

Instalujemy node.js

```java
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
````

Instalujemy skrypt nvm

```java
source ~/.bashrc
```


Wybór wersji node.js

```java
nvm list-remote
```


Instalacja node z wybraną wersja

```java
nvm install v17.3.0
```


Sprawdzamy wersje node.js

```java
node -v
```
