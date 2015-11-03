# WEB-CASCAVEL

Site do Grupo de Usuários Web de Cascavel no Paraná!

- Github para autenticação
- MySQL

## Instalação

```bash
cp .env.example .env # altere as chaves caso queira trocar a aplicação
cp config/database.yml.example config/database.yml # configure seus dados de acesso ao DB
bundle install
rake db:create db:migrate
rails server
```
