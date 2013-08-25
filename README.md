Grails Spring Social plugin for Tumblr
==============================

Grails plugin to use Tumblr via Spring Social API

## Required properties in Config.groovy:

tumblr.consumerKey = "consumer_key"

tumblr.consumerSecret = "consumer_secret"

After this properties are configured you can use 'tumblr' providerId in your app with spring social core to connect user Tumblr account. After this all operations you got permissions for are available through TumblrTemplate.

## Examples
### Signin through Tumblr button:
```html
  <g:form method="POST" mapping="springSocialSignIn" params="[providerId: 'tumblr']">
    <g:submitButton name="connectTumblr" value="Sign in with Tumblr"/>
  </g:form>
```