# blog (for practicing purpose)

# Technical Notes
 - Using canonical URLs for models
   - `A website might have different pages that display the same content. In our application, the initial part
of the content for each post is displayed both on the post list page and the post detail page. A canonical
URL is the preferred URL for a resource. You can think of it as the URL of the most representative
page for specific content. There might be different pages on your site that display posts, but there is a
single URL that you use as the main URL for a post. Canonical URLs allow you to specify the URL for
the master copy of a page. Django allows you to implement the get_absolute_url() method in your
models to return the canonical URL for the object.`
 - Creating SEO-friendly URLs for posts 
   - `we will make a post detail URL to look like
/blog/2022/1/1/some-slug-string/ . We will provide search engines with friendly URLs
to index, containing both the title and date of the post.`
 - Recommending posts by email
 - Creating a comment system
 - Adding the tagging functionality
 - Retrieving posts by similarity
 - Adding a sitemap to the site
 - Creating feeds for blog posts
 - Adding full-text search to the blog
   - Stemming and ranking results
     - Stemming is the process of reducing words to their word stem, base, or root form. Stemming is used
by search engines to reduce indexed words to their stem, and to be able to match inflected or derived
words. For example, the words “music”, “musical” and “musicality” can be considered similar words
by a search engine. The stemming process normalizes each search token into a lexeme, a unit of
lexical meaning that underlies a set of words that are related through inflection. The words “music”,
“musical” and “musicality” would convert to “music” when creating a search query.
   - Searching with trigram similarity