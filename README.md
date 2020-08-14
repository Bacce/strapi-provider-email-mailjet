# strapi-provider-email-mailjet

[Mailjet](https://mailjet.com/) provider for Strapi with attachments support for latest Strapi versions.

Made by [Automat-IT](https://www.automat-it.com/)

Added email "from" name field to parameters.
Example for usage with Strapi v3.0+ below.

## Resources

- [MIT License](LICENSE.md)

## Links

- [Strapi website](http://strapi.io/)
- [Strapi community on Slack](http://slack.strapi.io)
- [Strapi news on Twitter](https://twitter.com/strapijs)

## Installation

```bash
npm i strapi-provider-email-mailjet
```


### Example

**Path -** `config/plugins.js`

```js
module.exports = ({ env }) => ({
    email: {
    provider: 'mailjet',
    providerOptions: {
        mailjet_default_from_name:"Friendly Joe",
        mailjet_default_from:"no-reply@example.com",
        mailjet_default_replyto:"no-reply@exampl.com",
        username: env('MAILJET_API_USERNAME'), //example of env variable
        password:"xx"
    }
  }
});

```
