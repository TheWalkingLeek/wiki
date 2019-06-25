* ermöglicht single-sign on
* kann Benutzer und deren Zugriff verwalten (und dies somit der Applikation abnehmen)
* kann mit LDAP verbunden gekoppelt werden
* ermöglicht two factor authentication
* erlaubt social login (einloggen per Google/Facebook/... Konto)
* die Applikation handled nie selber mit user credentials
* die Applikation erhält ein Identity Token von dem Keycloak server zur Authentifizierung
* das Identity Token enthält Daten wie die E-Mail, den Namen etc. (je nach Applikation)