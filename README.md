# Shopify Imgix

Shopify Imgix is a Liquid snippet for Shopify that makes it easier to use imgix real-time image processing and image cdn.

## Installation

To get started, upload the shopify-imgix.liquid file into you themes snippets folder.

Basic Usage
===========

```liquid
{% capture shopify_logo_asset_url %}{{ 'logo.png' | asset_url }}{% endcapture %}
{% capture imgix_logo_url %}{% include 'shopify-imgix' path: shopify_logo_asset_url, w: 160, h: 42, q: 100, fit: 'fill', bg: 'ffffff' %}{% endcapture %}

<img src="{{ imgix_logo_url | strip }}">
```

Read the full [Image URL API Reference](https://docs.imgix.com/apis/url)

## License

[The MIT License](LICENSE).