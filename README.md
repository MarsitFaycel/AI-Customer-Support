# AI-Customer-Support

Construire une application permettant à un conseiller de répondre aux demandes clients grâce à l'IA.

Architecture cible :

                    ┌─────────────────┐
                    │   Angular       │
                    │   Interface     │
                    └────────┬────────┘
                             │ REST
                             ▼
                    ┌─────────────────┐
                    │    FastAPI      │
                    │    Python       │
                    └────────┬────────┘
                             │
              ┌──────────────┼──────────────┐
              ▼              ▼              ▼
         PostgreSQL        LLM API       CRM API
          clients          GPT/...       (mock)

L'application devra progressivement savoir :

1 recevoir une demande client ;

2 comprendre l'intention ;

3 récupérer les informations du client ;

4 utiliser un LLM ;

5 appeler des outils/API ;

6 générer une réponse ;

7 afficher la réponse dans l'interface ;

8 enregistrer la conversation ;

9 être entièrement dockerisée.
