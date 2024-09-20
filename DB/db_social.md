# Vogliamo creare uno spazio virtuale in stile social network dove gli utenti possano condividere le proprie esperienze. Ogni 
# - utente 
# può creare dei 
# - post, 
# al quale può aggiungere uno o più 
# - media 
# come foto e video. Ogni post può avere uno o più 
# - tags 
# che servono per categorizzare i contenuti. Gli altri utenti possono interagire con il post esprimendo il loro gradimento attraverso un semplice 
# - like.
# BONUS: i post possono avere anche i 
# - Commenti.

## DB Social

# table: users 

- id
  - BIGINT
  - PK
  - AUTO_INCREMENT
  - UNIQUE
  - NOTNULL

- name
  - VARCHAR(45)
  - NOTNULL

- surname
- nickname
- email
- date_of_birth 