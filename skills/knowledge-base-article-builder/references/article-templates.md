# Knowledge-Base Article Templates

Replace bracketed placeholders only with information supported by the supplied or approved source.

## Standard informational article

```html
<h1>[Article title]</h1>
<p>[Brief overview or purpose.]</p>

<h2>[Primary topic]</h2>
<p>[Main information.]</p>

<h2>[Requirements or important details]</h2>
<ul>
<li>[Supported detail]</li>
<li>[Supported detail]</li>
</ul>

<h2>Common Questions</h2>
<h3>[Natural reader question]</h3>
<p>[Concise answer supported by the source.]</p>
```

## Process article

```html
<h1>[Article title]</h1>
<p>[Who the process is for and what it accomplishes.]</p>

<h2>Before You Begin</h2>
<ul>
<li>[Prerequisite or required item]</li>
<li>[Important limitation or qualification]</li>
</ul>

<h2>Steps</h2>
<ol>
<li>[First action]</li>
<li>[Second action]</li>
<li>[Final action]</li>
</ol>

<h2>Important Notes</h2>
<ul>
<li>[Restriction, deadline, exception, or outcome]</li>
</ul>

<h2>Common Questions</h2>
<h3>What happens after I complete the process?</h3>
<p>[Answer supported by the source.]</p>
```

## Reference or comparison article

```html
<h1>[Article title]</h1>
<p>[Brief explanation of the reference information.]</p>

<table border="1" cellpadding="6" cellspacing="0">
<thead>
<tr>
<th>[Column 1]</th>
<th>[Column 2]</th>
<th>[Column 3]</th>
</tr>
</thead>
<tbody>
<tr>
<td>[Value]</td>
<td>[Value]</td>
<td>[Value]</td>
</tr>
</tbody>
</table>
```

## Default response format

For article-creation requests, return:

1. Recommended title
2. One-sentence summary
3. Clean article content in the requested format
4. Any unresolved source gaps or local configuration placeholders
