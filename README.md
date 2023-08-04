
# Istruzioni
-docker rm phormer (se presente)
-docker build -t phormer .
-docker run -d -p 80:80 --name phormer phormer
-docker stop phormer
