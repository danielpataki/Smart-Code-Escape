# Smart Code Escape WordPress Plugin

A plugin that enables you to write code more easily in the WordPress editor by escaping it in the front-end but leaving it in-tact in the back-end.

## Description

A tiny plugin for WordPress which converts greater than signs, smaller than signs and ampersands to html entities within pre tags. It supports semantic syntax you would use when using the Prism highlighter for example. If a code tag sits immediately within a pre tag it will not be escaped.

Code is escaped before it is displayed which gives you easy editing access in the backend as you will always see the unescaped version.

Just write your code and forget anything else :) You can write code in two ways:

```
<pre><strong>some code</strong></pre>
<pre><code class="language-php"><strong>some code here</strong></code></pre>
```

In the second example the code tag will not be escaped, leading to semantically nice syntax. When output to the user in the front end the following will be used:

```
<pre>&lt;strong&gt;somecode&lt;/strong&gt;&lt;/pre&gt;</pre>
<pre><code class="language-php">&lt;strong&gt;somecode&lt;/strong&gt;&lt;/pre&gt;</code></pre>
```

#### Useful Links

This Github repository is for the development of this plugin. If you would like to read installation and in-depth usage instructions you might want to look at the WordPress plugin page instead.

* [Plugin Page](https://wordpress.org/plugins/smart-code-escape/)
* [SVN Repository](http://plugins.svn.wordpress.org/smart-code-escape/)


# Want To Help?

If you like the plugin and you like helping others out there are a few things you can do:

* **[Review the plugin](https://wordpress.org/support/view/plugin-reviews/smart-code-escape)**
* **[Tip me on Gratipay](https://gratipay.com/danielpataki/)**
