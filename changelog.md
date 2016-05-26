Dj4x
===

# Change log

* 2014-07-26 (1.0.0)
> * first code

* 2014-07-27 / 2014-09-30 (1.0.1 - 1.19.22)

* 2014-10-02 (2.0.0 Bonne Jenet)
> * Réécriture du code
> * Création des fichiers .json
> * Debugging

* 2014-10-02 - 2014-10-03 (2.1.0 Bonne Jenet)
> * Multiple reminders support

* 2014-10-03 (2.2.1)
> * Petite correction de format %
> * Dynamisation de auto_tip et check_bal pour supporter plusieurs bots

* 2014-10-04 (2.2.2)
> * Corrections mineures

* 2014-10-05 (2.3.2)
> * Ajout de +donate

* 2014-10-08 (2.3.3)
> * Portage Python 2.7 / Linux

* 2014-10-09 (2.3.4)
> * Compatibilité 2.7 / Linux

* 2014-10-10 (2.3.5)
> * Fixed a problem with tip timeout

* 2014-10-15 (2.5.5)
> * Added BITtrex api
> * Unified the ticker APIs

* 2014-10-16 (2.5.6)
> * Minor fix on *ticker

* 2014-10-22 (2.5.7)
> * Minor fix on handling tips channels

* 2014-10-23 (2.5.8)
> * Arranged an oversight that prevented the bot from tipping a received tip even after a timeout or a keep <hash>

* 2014-10-30 (2.8.9)
> * Added more NOTICE messages to make the bot less spammy (addie.cc, ltcrabbit, help)
> * Added Cryptonator API
> * Added *convert command
> * Added DOGED to AutoTip

* 2014-11-09 (2.8.10)
> * Fixed float division

* 2014-11-28 (2.9.10)
> * Ajouté : système de sécurité pour vérifier l'identité des administrateurs

* 2014-12-19 (2.9.11)
> * Added XPY to AutoTip

* 2014-12-28 (2.9.12)
> * Fixed: UTF-8 support for *translate and its XML parsing

* 2014-12-29 (2.10.12)
> * Added API with Chuck Norris facts (French)

* 2015-01-02 (2.10.13)
> * Ajouté +aide

* 2015-01-06 (2.11.13)
> * Ajout de la fonction de calcul à *convert

* 2015-01-13 (2.11.14)
> * Adaptation de autotip à pndtip, Tip sur le canal, non en privé.

* 2015-01-16 (2.12.14)
> * LOCAL (True|False) support

* 2015-01-17 (2.13.14)
> * Bitly API support (*bitly | *short)

* 2015-02-01 (2.13.15)
> * Minor change to LOCAL const and _timeout_reminder()

* 2015-02-13 (2.13.17)
> * Importing urllib.parse for Py3
> * Adding "owner" params for *bitly

* 2015-02-14 (2.14.18)
> * Ajout de is_auth() pour une utilisation extérieure à cmd_admins()
> * Remaniement de is_auth() et création de auth_users pour la gestion des groupes d'utilisateurs

* 2015-02-16 (2.15.18)
> * Ajout de api_ticker_custom()

* 2015-02-19 (2.15.19)
> * Ajout de LazyCoinsRainBot (doge) à auto-tip

* 2015-03-14 (2.15.20)
> * Version-dependent UTF-8 usage in api_chucknorrisfact()

* 2015-08-08 (3.15.20)
> * Ajout de l'interface Telegram

* 2015-08-09 (3.16.20)
> * Réglages de l'interface Telegram

* 2015-08-10 (3.17.20)
> * Ajout de la commande Telegram /enligne pour avoir la liste des utilisateurs présents sur le canal IRC.

* 2015-08-11 (3.20.20)
> * Ajout d'un filtre anti-flood pour les messages Telegram > IRC
> * Changements de compatibilité urllib3/ssl_
> * Ajout du transfert des messages join / part / quit

* 2016-01-08 (3.20.21)
> * requests.packages.urllib3 .disable_warnings()

* 2016-01-10 (3.20.22)
> * Support of UNICODE chars in Telegram chat names.

* 2016-01-11 (3.20.23)
> * Corrigé un oubli dans le code qui doit déclarer le bot comme telegram_classes_User avant d'envoyer un message dans AutoTip

* 2016-02-09 (3.20.24)
> * Markdown formatting for Telegram-side messages.

* 2016-02-10 (3.20.25)
> * Markdown formatting for ticker results.

* 2016-02-11 (3.20.26)
> * Comblé une faille qui permet d'écrire en Markdown à partir de IRC vers Telegram.

