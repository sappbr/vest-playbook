# Embed the assistant

Use this after the site is published. GitBook does not serve the widget from the repo.

1. Publish the site.
2. Settings, AI and MCP, enable Assistant.
3. Copy the embed script URL.

```html
<script src="https://YOUR-SITE/~gitbook/embed/script.js"></script>
<script>
  window.GitBook('init', { siteURL: 'https://YOUR-SITE' });
  window.GitBook('configure', {
    button: { label: 'Ask', icon: 'assistant' },
    tabs: ['assistant', 'docs'],
    greeting: { title: 'Vest playbook', subtitle: 'Rules, fees, and the path.' },
    suggestions: ['What do I buy first?', 'When do I claim?']
  });
  window.GitBook('show');
</script>
```

Replace YOUR-SITE with the published URL. The script will not load before the site is public.
