Adjunto remito el ejercicio de spotify de la tercera semana de FaceToFace.

Genial trabajar en grupo para sacarla adelante: Sara Mesa, Alvaro Madrena y Oscar Arjona. 

----> Aplicación:
Desde 'spotyLogin.html' el usuario accede introduciendo usuario y contraseña; que en 'spoty.js' son cotejados en el jsonP que contiene los registros de usuarios (funcion LogIn de la consulta ajax a JsonP) y sólo si es verificado como usuario registrado, se le redirecciona al segundo html ('mainPage.html').

En 'mainPage.html' el usuario puede introducir el nombre de un artista y le será devuelto los top-tracks (función top-tracks) del artista (funcion search) introducido junto con un botón de save (las consultas ajax que detonan estas funciones se han unificado bajo la misma función "request").Los top-tracks aparecen al lado derecho del cuerpo de la pagina, mientras que le lado izquierdo queda reservado para la playlist (canciones que 'salve' con el botón 'save' y que adjunta la función 'appendPlaylist').

Si el usuario sale de su sesión (haciendo click en el 'retroceder' del propio navegador) y vuelve a 'sportyLogin.html', reintroduciendo su nombre y contraseña, al abrirse 'mainPage.html' se recuperará su playlist de la sesión anterior (responsabilidad de la función "prior_login").

Muy interesante el tema LocalStorage para guardar la información relativa a las sesiones previas (cuarta iteración).  A la hora de 'desloguearte' no existe un botón  para ello en 'mainPaige.html' (lo ideal: esquina superior derecha), que queda como deuda técnica (el usuario debe usar el 'retroceder' propio del navegador). Igualmente, paciencia con la carga de los top-tracks del artista consultado, pues hasta que no estén todos, el play de los iframes de spoty no estarán habilitados ni los botones de 'save'.

Un saludo,

Paz rg