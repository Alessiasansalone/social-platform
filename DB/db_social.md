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
  - VARCHAR(45)
  - NOTNULL

- nickname
  - VARCHAR(45)
  - NOTNULL

- email
  - VARCHAR(45)
  - NOTNULL

- date_of_birth
  - DATE
  - NOTNULL

- registration_date
  - DATE
  - NULL


# table: posts

- id
  - BIGINT
  - PK
  - AUTO_INCREMENT
  - UNIQUE
  - NOTNULL
  
- user_id
  - UNSIGNED
  - BIGINT
  - FOREIGN KEY

- description
  - VARCHAR(255)
  - NULL

- date
  - DATE
  - NOTNULL

- hour
  - TIME
  - NOTNULL


# table: medias

- id
  - BIGINT
  - PK
  - AUTO_INCREMENT
  - UNIQUE
  - NOTNULL
  
- post_id
  - UNSIGNED
  - BIGINT
  - FOREIGN KEY

- type
  - VARCHAR(20)
  - NOTNULL

- name
  - VARCHAR(255)
  - NOTNULL

- size
  - VARCHAR(20)
  - NOTNULL

- date
  - DATE
  - NULL

- hour
  - TIME
  - NULL


# table: hashtags

- id
  - BIGINT
  - PK
  - AUTO_INCREMENT
  - UNIQUE
  - NOTNULL

- name
  - VARCHAR(80)
  - NOTNULL

- date
  - DATE
  - NULL

- hour
  - TIME
  - NULL


# table: likes

- id
  - BIGINT
  - PK
  - AUTO_INCREMENT
  - UNIQUE
  - NOTNULL

- post_id
  - UNSIGNED
  - BIGINT
  - FOREIGN KEY

- user_id
  - UNSIGNED
  - BIGINT
  - FOREIGN KEY

- date
  - DATE
  - NOTNULL

- hour
  - TIME
  - NOTNULL


# table: comments

- id
  - BIGINT
  - PK
  - AUTO_INCREMENT
  - UNIQUE
  - NOTNULL

- contents
  - VARCHAR(255)
  - NOTNULL

- post_id
  - UNSIGNED
  - BIGINT
  - FOREIGN KEY

- user_id
  - UNSIGNED
  - BIGINT
  - FOREIGN KEY

- date
  - DATE
  - NOTNULL

- hour
  - TIME
  - NOTNULL