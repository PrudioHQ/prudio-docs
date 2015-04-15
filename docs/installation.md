# Widget Installation

## Install

To install the code snippet please refer to the *Prudio* [administration](https://app.prud.io).

There you can create and find your applications.

Copy the following code and paste it inside your `<body>` tag.

Simple example:

```html
<script src="https://static.prud.io/client.js?appid=YOURAPPID" async></script>
```

Don't forget to change the `YOURAPPID` for your own code.

## Options

### Identify your users

Use the configurations to give a brief insight of your users.

For example, if your user is already authenticated in you web app you don't need
to ask for the name and e-mail again.

Check this example:

```html
<script src="https://static.prud.io/client.js?appid=YOURAPPID" async></script>
<script>

    window._PrudioSettings = {
        name: 'John Doe',
        email: 'john.doe@example.com'
    };

</script>
```

Simple example using **PHP**:

```
<script src="https://static.prud.io/client.js?appid=YOURAPPID" async></script>
<script>

    window._PrudioSettings = {
        name: '<?php echo $user->name; ?>',
        email: '<?php echo $user->email; ?>'
    };

</script>
```

## Personalize your widget

```html
<script src="https://static.prud.io/client.js?appid=YOURAPPID" async></script>
<script>

    window._PrudioSettings = {
        title: '', // Title of the window (on the top)
        icon: '', // Check the available icon bellow
        buttonColor: '', // Color of the default button
        borderColor: '', // Color of the button border
        buttonSelector: '' // the jQuery like selector .class or #id
    };

</script>
```

**Available icons:**

* prd-icon-btn-bubble
* prd-icon-btn-chat
* prd-icon-btn-prudio
* prd-icon-btn-chats
* prd-icon-btn-help
