# Widget Installation

## Install

To install the code snippet please refer to the *Prudio* [administration](https://app.prudio.com).

There you can create and find your applications.

Copy the following code and paste it inside your `<body>` tag.

Simple example:

```html
<script src="https://widget.prudio.com/client.js?appid=YOURAPPID" async></script>
```

Don't forget to change the `YOURAPPID` for your own code.

## Personalize your widget

Prudio comes with a good default configuration that meets the needs of many of its deployments. However we know that each use case has its own special demands, this way we give you the chance to configure and adapt the widget to your website look and feel. Bellow are some of the settings available:

```html
<script src="https://widget.prudio.com/client.js?appid=YOURAPPID" async></script>
<script>

    window._PrudioSettings = {
        title: '', // Title of the window (on the top)
        icon: '', // Check the available icon bellow (default: prd-icon-btn-help)
        buttonColor: '', // Color of the default button (default: rgba(0, 114, 176, 0.9))
        borderColor: '', // Color of the button border (default: rgba(0, 114, 176, 1))
        iconColor: '', // Color of the icon (default: white)
        buttonSelector: '' // the jQuery like selector .class or #id
    };

</script>
```

As you can see in the example above, you can change the displayed text (`title`), the icon of the default button (see bellow the available icons) and the colors (`buttonColor`, `borderColor`, `iconColor`). If it is not enough, you can also specify an element in your own page to trigger the Prudio Widget (`buttonSelector`) instead of using the default button.

**Available icons:**

* prd-icon-btn-help (*default*)
* prd-icon-btn-bubble
* prd-icon-btn-chat
* prd-icon-btn-prudio
* prd-icon-btn-chats

## Identify your users

Use the configurations to give a brief insight of your users.

For example, if your user is already authenticated in you web app you don't need
to ask for the name and e-mail again.

Check this example:

```html
<script src="https://widget.prudio.com/client.js?appid=YOURAPPID" async></script>
<script>

    window._PrudioSettings = {
        name: 'John Doe',
        email: 'john.doe@example.com'
    };

</script>
```

Simple example using **PHP**:

```
<script src="https://widget.prudio.com/client.js?appid=YOURAPPID" async></script>
<script>

    window._PrudioSettings = {
        name: '<?php echo $user->name; ?>',
        email: '<?php echo $user->email; ?>'
    };

</script>
```

## Language

Please check the [documentation on localization](/localization/).
