h1. How do I manage static pages? [todo]

The short answer: create a section, use an article form that doesn't include posted dates or permlinks, and post a single article in that section.

The long answer: when you view a URL like @http://example.com/contact/@, Textpattern will display the _section_ named *contact*, using the _page template_ selected for the *contact* section. (This assumes your Textpattern front page is @http://example.com/@).

The usual way to manage content on a "static" (single, stand-alone) page like this is as follows:

1. Create a new *article form* named @static_article@, with the following contents:

bq. @<h3><txp:title /></h3>@
@<p><i><txp:excerpt /></i></p>@
@<txp:body />@

This will be used to display the article contents on your static page. You can change the markup later if you want.

2. Copy your @default@ page template to a new template named @static_page@. Find the @<txp:article />@ tag in the @static_page@ template, and change it to look like this:

bq. @<txp:article limit="1" form="static_article" status="sticky" />@

This template will be used to display your static page.

3. Create a new *section* named @contact@ (or whatever you want your page to be called). Go to *presentation > sections* and set *Uses page* to @static_page@ for your new section.

4. Post a new *article* in the @contact@ section, with the article status set to *Sticky* instead of Live.

The most recent Sticky article will be displayed as the page contents when you view the URL @http://example.com/contact/@.

To create additional static pages, you can skip steps 1 and 2, and reuse the same @static_page@ template.

For the best way to create links to your static pages, see "How do I create navigation links?":https://textpattern.com/faq/92/how-do-i-create-navigation-links

For a more detailed description, read "Managing Static Pages With Textpattern":http://thresholdstate.com/articles/3667/managing-static-pages
