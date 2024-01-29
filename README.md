# Galeria de Gats amb Laravel

Aquest és un projecte que demostra com utilitzar Laravel per crear una galeria d'imatges de gats utilitzant una API externa. L'activitat consta de dues parts principals: llegir d'una API externa i crear una API pròpia per gestionar les imatges.

## Descripció de l'Activitat

### Part 1: Llegir de l'API Externa

En aquesta part de l'activitat, hem utilitzat Laravel per llegir d'una API externa que proporciona imatges de gats. Hem utilitzat la llibreria Guzzle per fer sol·licituds HTTP a l'API i hem emmagatzemat les dades a la nostra base de dades local. També hem descarregat les imatges i les hem emmagatzemat localment al servidor.

### Part 2: Crear una API Pròpia

A la segona part de l'activitat, hem creat una API pròpia utilitzant Laravel per gestionar les imatges de gats que hem emmagatzemat a la nostra base de dades local. Hem afegit funcionalitats com la llista de les imatges, l'afegir noves imatges, i la cerca d'imatges per etiquetes.

## Desplegament del Projecte

Per desplegar aquest projecte al teu propi entorn, segueix aquestes instruccions:

Clona el repositori a la teva màquina local utilitzant Git:

   ```bash
   git clone https://github.com/oriolmiro/cataas.git
   ```

Instal·la les dependències de Laravel mitjançant Composer:

   ```bash
    composer install
    cp .env.example .env
   ```

Edita l'arxiu .env i configura la connexió a la base de dades.

   ```bash
    php artisan key:generate
    php artisan migrate:refresh --seed
    php artisan serve
   ```

El teu projecte s'iniciarà a http://localhost:8000.
