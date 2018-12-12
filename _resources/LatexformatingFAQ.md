---
title: LaTeX Formatting FAQ
order: 10
---

# FAQ on LaTeX formatting for UMM CSci senior seminar
{:.no_toc}

Feel free to add questions and answers and improve the current answers. 

* Do not remove this line (it will not be displayed)
{:toc}

### A `$` in my verbatim breaks TexMaker

Add a `%$` at the end of your verbatim environment.

### How do I format a url in a paper?

Include a url package in the beginning of the paper (before `\begin{document}`):

```latex
 \usepackage{url} 
```

 Then use `\url{...}` for urls.

### How do I add a url to a bibliography item?
If you are referencing an online article, use the following in your `.bib` file:

```latex
@misc{...,
  ...,
  howpublished = {\url{http://...}}
} 
```

[Here](https://texfaq.org/FAQ-citeURL.html) is more information (caution: you must use ACM bibliography style so suggestions to change the style aren't applicable).

### How do I balance the last two columns if `\balancecolumns` has no effect?

```latex
\usepackage{balance}
\begin{document}
...
\balance
\end{document} 
```

[Here](https://ctan.org/pkg/balance?lang=en) is more information.

### How do I check if my paper uses A4 or Letter Paper?
Using the templates from the senior seminar github fixes this issue Open it in Adobe Reader, go to File menu, and select Properties. In the tab Description it should show Paper Size as 8.5in by 11in (letter paper size). Otherwise it's A4. Note that the difference may not be visible on screen, but might show up when you are trying to print and A4 will mess up the final proceedings if left unchanged.

<div class="flash">
<b>Note that current senior seminar templates use letter paper</b>, so you don't need to worry about it if you use our templates (as you should). 
</div>

### How do change my page size from A4 to Letter Paper?

Using the templates from the senior seminar github fixes this issue Some LaTeX formatting programs allow you to set the paper size. For most of them, however, it's difficult to find and the setting may be overwritten later by A4 again. For the seminar proceedings use the sig-alternate.cls linked to the [resources page](seniorsemresources.md). It has a line

```latex
\usepackage[letterpaper]{geometry}
```

among its package declarations that fixes the problem.

If you are using a different document class, such as article (this wouldn't be for your senior seminar proceeding, but for something else that you might be using latex for), then use

```latex
\usepackage[letterpaper]{geometry}
```

after the document class.

### How do I preserve capitalization in titles in my bibliography?
If a paper title contains a word that needs to be capitalized, surround it by curly braces, e.g. `{CAPTCHA}` or `{Java}`.

### How do I get rid of the navigation icons in Beamer?

If you don't want those pesky presentation controls on your slides during your presentation, use this:

```latex
\setbeamertemplate{navigation symbols}{}
```

(Courtesy of Dillon Stenberg - 03 Dec 2015.)
