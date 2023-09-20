+++
title = "Doublecode"
description = ""
weight = 6
+++

The _doublecode_ shortcode works the same as the [code](/shortcodes/code/) shortcode, but extends the functionality by also rendering the code in the page. This is useful for showing the code of HTML elements in your page.

{{< doublecode lang="html" >}}

<div class="mydiv bg-primary shadow text-white p-3 m-4 border-primary">
	<p class="h4 title">Hi there</p>
	<p class="lead mb-0">I'm inside a doublecode shortcode, that's why I look so fancy.</p>
</div>
{{< /doublecode >}}

## Usage

Simply place the following shortcode on the page

#### Code in the shortcode

{{< code lang="html" >}}
{{</* doublecode lang="LANG" */>}} [your code] {{</* /doublecode */>}}
{{< /code >}}

### Parameters

#### _lang_

The lang parameter defines the language to be used for code highlighting. You can find a complete list of supported languages <a href="https://gohugo.io/content-management/syntax-highlighting/#list-of-chroma-highlighting-languages" target="_blank">here</a>.

Example: <code>lang="html"</code>

#### _file_

The file parameter allows you to define an external file that contains your code to be displayed. This is done by giving a path to that file, starting from the root directory of your site.
For example, a HTML file named _'mycode.html'_ you wish to link that is in the _docs/code/_ directory can be defined as follows: <code>file="code/mycode.html"</code>.
