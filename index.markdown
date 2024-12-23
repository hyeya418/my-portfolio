---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>{{ site.data.info.title }}</title>
</head>
<body>
  <h1>{{ site.data.info.title }}</h1>
  <p>{{ site.data.info.description }}</p>
  <ul>
    {% for feature in site.data.info.features %}
      <li>
        <strong>{{ feature.name }}</strong>: {{ feature.description }}
      </li>
    {% endfor %}
  </ul>
</body>
</html>
