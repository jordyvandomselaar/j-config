[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://beta.webcomponents.org/element/jordyvandomselaar/jvd-config)
# jvd-config#
Store all your global config in one place

## Example

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

## Available functions
Just one really:
`get(key, default)`
If key doesn't exist, `default` will be returned.
If `default` doesn't exist either `false` will be returned. The reason I chose to return false is so you can use boolean attributes the regular way.

I personally have a `jvd-config` element with my api urls in there. If I comment the element my `default` values will trigger which are my live api so that's an easy dev to prod mode =)
## Wish to help?
There's 2 things you can do:
1. File an issue report
2. Fork this project and submit a pr with your changes