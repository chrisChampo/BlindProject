# Documentation du serveur

## Endpoints:

**n est l'indices de la base sélectionnée**

-   ### GET /api/ping/n:

    _Renvoie le status de la base n_
    Retour:

    ```json
    {
      "up": bool,
      "playing": bool
    }
    ```

-   ### GET /api/battery/n:

    _Retourne le % de batterie de la base n_  
     Retour:

    ```json
    {
        "battery": number
    }
    ```

-   ### GET /api/volume/n:

    _Retourne le % du volume de la base n_  
     Retour:

    ```json
    {
        "volume": number
    }
    ```

-   ### POST /api/play/n:

    _Lance le son sur la base n_

-   ### POST /api/stop/n:

    _Arrete de jouer le son sur la base n_

-   ### POST /api/volume/n:
    _Règle le volume de la base n_  
     Body:
    ```json
    {
        "volume": number
    }
    ```

    ### POST /api/upload/n:
    _La base n va jouer le son uploader_
    Le body est un fichier son.
