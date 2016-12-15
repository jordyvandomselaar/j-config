[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://beta.webcomponents.org/element/jordyvandomselaar/jvd-config)
#jvd-config
Store all your global config in one place

##Example

```
// Set config
<jvd-config api-url="localhost:8000"/>
// All other instances will now have that config, no need to set it again
<jvd-config id="config" />

<script>
document.getElementById('config').get('api-url');
// localhost:8000
</script>

```
##Wish to help?
There's 2 things you can do:
1. File an issue report
2. Fork this project and submit a pr with your changes