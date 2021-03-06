[![Build Status](https://buildhive.cloudbees.com/job/nicerobot/job/xupl/badge/icon)](https://buildhive.cloudbees.com/job/nicerobot/job/xupl/) [![endorse](https://api.coderwall.com/nicerobot/endorsecount.png)](https://coderwall.com/nicerobot)

# See the [`xupl`](https://github.com/nicerobot/xupl/wiki) wiki

Let's return to a sane world where opening and closing blocks is as simple and easy as matching curly braces `{}` and all the words with meaning in the text are not hidden beneath cruft `</>`.

Xupl enables the writing of HTML like this:

    html {
    	head {title{"Xupl"}}
	    body {
	    	div #xuplid .xuplclass {
	    		a //github.com/nicerobot/text-plain/wiki {"text-plain.org"}

and getting this:

    <html>
      <head>
        <title>Xupl</title>
      </head>
      <body>
        <div id="xuplid" class="xuplclass">
          <a href="//github.com/nicerobot/text-plain/wiki">text-plain.org</a>
        </div>
      </body>
    </html>

Coming soon, the above can be written using only indentations for blocks:

    html
    	head
    		title
    			"Xupl"
	    body
	    	div #xuplid .xuplclass
	    		a //github.com/nicerobot/text-plain/wiki
	    			"text-plain.org"
	    		"And any quoted text
					is naturally
					multi-line."

or compact:

    html
    	head: title: "Xupl"
	    body: div #xuplid .xuplclass
	    	a //github.com/nicerobot/text-plain/wiki: "text-plain.org"
    		"And any quoted text\ncan embed\ncarriage returns."
