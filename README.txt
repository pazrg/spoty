Adjunto remito el ejercicio de spotify de la tercera semana de FaceToFace.

Genial trabajar en grupo para sacarla adelante: Sara Mesa, Alvaro Madrena y Oscar Arjona. 

----> Aplicaci�n:
Desde 'spotyLogin.html' el usuario accede introduciendo usuario y contrase�a; que en 'spoty.js' son cotejados en el jsonP que contiene los registros de usuarios (funcion LogIn de la consulta ajax a JsonP) y s�lo si es verificado como usuario registrado, se le redirecciona al segundo html ('mainPage.html').

En 'mainPage.html' el usuario puede introducir el nombre de un artista y le ser� devuelto los top-tracks (funci�n top-tracks) del artista (funcion search) introducido junto con un bot�n de save (las consultas ajax que detonan estas funciones se han unificado bajo la misma funci�n "request").Los top-tracks aparecen al lado derecho del cuerpo de la pagina, mientras que le lado izquierdo queda reservado para la playlist (canciones que 'salve' con el bot�n 'save' y que adjunta la funci�n 'appendPlaylist').

Si el usuario sale de su sesi�n (haciendo click en el 'retroceder' del propio navegador) y vuelve a 'sportyLogin.html', reintroduciendo su nombre y contrase�a, al abrirse 'mainPage.html' se recuperar� su playlist de la sesi�n anterior (responsabilidad de la funci�n "prior_login").

Muy interesante el tema LocalStorage para guardar la informaci�n relativa a las sesiones previas (cuarta iteraci�n).  A la hora de 'desloguearte' no existe un bot�n  para ello en 'mainPaige.html' (lo ideal: esquina superior derecha), que queda como deuda t�cnica (el usuario debe usar el 'retroceder' propio del navegador). Igualmente, paciencia con la carga de los top-tracks del artista consultado, pues hasta que no est�n todos, el play de los iframes de spoty no estar�n habilitados ni los botones de 'save'.

Un saludo,

Paz rg