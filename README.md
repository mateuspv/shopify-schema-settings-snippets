# Shopify schema snippets

This extension allows you to quickly create [shopify schema settings](https://help.shopify.com/en/themes/development/theme-editor/settings-schema)

Simple open your `.liquid` file and type `_`(underscore), you shall get the follow schema settings options:

* _schema
* _text
* _textarea
* _image_picker
* _radio
* _select
* _checkbox
* _range
* _color
* _font
* _collections
* _product
* _blog
* _page
* _link_list
* _url
* _video
* _richtext
* _html
* _article
* _header
* _paragraph


## Example

Open your `.liquid` file and type `_schema`, then press tab and expand the follow snippet

```liquid
{% schema %}
  {
    "name": "$1",
    "class": "$2",
    "settings": [
      $3
    ]
  }
{% endschema %}
```

You can press tab again to navigate between $1, $2 and $3 Tabstops,

Inside the settings, you can expand `_text` or any other snippet:

```liquid
{% schema %}
  {
    "name": "",
    "class": "",
    "settings": [
      {
        "type": "text",
        "id": "$1",
        "label": "$2",
        "default": "$3",
        "info": "$4",
        "placeholder": "$5"
      },      
    ]
  }
{% endschema %}
```