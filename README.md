# Nishchal Bhandari — Portfolio

Static portfolio for https://nishchalbhandari.dev/.

## SEO setup

- `index.html` contains the page title, description, canonical URL, social preview metadata, and JSON-LD WebSite, ProfilePage, and Person data.
- `robots.txt` allows crawling and points to `sitemap.xml`.
- The sitemap lists only the homepage: section anchors are not separate pages.
- All portfolio content is in HTML and can be read without JavaScript.

Keep the canonical URL, structured data, social URLs, sitemap, and CNAME consistent if the domain changes. Keep structured data aligned with the visible portfolio; add only verified profile links to `sameAs`.

## After deployment

1. Confirm `/`, `/robots.txt`, `/sitemap.xml`, and `/assets/profile.jpg` return HTTP 200 on the custom domain. Confirm HTTPS is enabled and alternate hosts redirect to the canonical domain.
2. Verify ownership of `nishchalbhandari.dev` in [Google Search Console](https://search.google.com/search-console/) using its supplied DNS TXT record, or use a URL-prefix property and its supplied HTML verification method. No verification token is included in this repository.
3. Submit `https://nishchalbhandari.dev/sitemap.xml` in Search Console. Inspect the homepage URL and request indexing if needed.
4. Check the deployed homepage with [Google Rich Results Test](https://search.google.com/test/rich-results) and [PageSpeed Insights](https://pagespeed.web.dev/). Local JSON validation does not replace these live checks.
5. Monitor indexing, search queries, impressions, and clicks in Search Console over the following weeks. SEO changes do not guarantee indexing or rankings.

## Content improvements

Replace project repository/demo placeholders with working links when available. Add original project case studies explaining the problem, your contribution, implementation, and results; each real standalone page should have its own title, description, canonical URL, and sitemap entry. Replace the shortened LinkedIn URL with the confirmed public profile URL. Link to this portfolio from your GitHub and LinkedIn profiles.

Reference: [Google's SEO Starter Guide](https://developers.google.com/search/docs/fundamentals/seo-starter-guide).

