# RailsGoogleLogin

This is a Rails project with google omniauth authentication.

## Config
You need set environment variables. After dowload the project, follow the steps:
* Remove `config/credentials.yml.enc` and `config/master.key` (if there are).
* run `EDITOR="code --wait" rails credentials:edit` and add your "google api omniauth Client ID and Secret keys". Like this:
```ruby
google_oauth_client_id: myAwesomeClientIdKeyHere
google_oauth_client_secret: myAwesomeSecretKeyHere
```
Save and close the file.

Now you can run:
```bash
rails db:create db:migrate
rails s
```
and visit `http://localhost:3000`
=)
