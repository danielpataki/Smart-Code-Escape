# Smart Code Escampe

A tiny plugin for WordPress which converts greater than signs, smaller than signs and ampersands to html entities within pre tags. It supports semantic syntax you would use when using the Prism highlighter for example. If a code tag sits immediately within a pre tag it will not be escaped.

Code is escaped before it is displayed which gives you easy editing access in the backend as you will always see the unescaped version.

## Usage

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

## Installation

Since this a WordPress plugin just search for "Smart Code Escape" in the plugins section in the admin and install it from there. If you would rather use this repository the easiest way is to use the trunk directory:

1. Download this whole repository
2. Rename the trunk directory within the smart-code-escape directory to smart-code-escape
3. Copy the smart-code-escape/smart-code-escape directory into your WordPress plugins directory
4. Go to your WordPress admin and activate the plugin.

For advanced use you can use a symbolic link that points to the trunk directory within the repository. Download the whole repository anywhere and create symbolic link between the `trunk` directory and the plugin. For example: `ln -s smart-code-escape/trunk /path/to/wordpress/wp-content/plugins/smart-code-escape`
