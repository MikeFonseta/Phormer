# Phormer

[Vedi pagina sourceforge](https://sourceforge.net/projects/rephormer/)

## Avvio applicativo

Prima dell'avvio dell'applicativo sarà necessario scegliere una delle versioni disponibili nella cartella Versions.\
Per modificare la versione sarà necessario modificare la riga seguente nel DockerFile cambiando ./Versions/3.0.1 in ./Versions/{Nome versione disponibile nella cartella Versions}

```
COPY ./Versions/3.0.1 /var/www/html/
```
Per avviare l'applicativo:
```
docker build -t phormer .
docker run -d -p 80:80 --name phormer phormer
```
## Terminare applicativo
```
docker stop phormer
```
