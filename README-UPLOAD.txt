www.venkatakishorekothapudi.com - upload package
=================================================

Files (all go in the website's root folder, usually public_html):
  index.html   - the complete website (photo and styles built in)
  robots.txt   - lets Google index the site
  sitemap.xml  - tells Google the page address

OPTION A - GoDaddy Web Hosting (cPanel)
  1. GoDaddy > My Products > Web Hosting > Manage > cPanel Admin.
  2. Open File Manager and go to public_html.
     (If the domain is an add-on domain, open its own folder instead.)
  3. Delete or rename any old index.html / default.html placeholder.
  4. Upload > select the zip > Extract, or upload the three files directly.
     index.html, robots.txt and sitemap.xml must sit directly in public_html,
     not inside a sub-folder.
  5. In cPanel > Domains (or SSL/TLS Status), make sure the free SSL
     certificate is active so https:// works.
  6. Open https://www.venkatakishorekothapudi.com and check every tab.

OPTION B - free hosting on GitHub Pages, domain stays at GoDaddy
  1. Create a public GitHub repository and upload the three files.
  2. Settings > Pages > Deploy from branch (main, root).
  3. Settings > Pages > Custom domain: www.venkatakishorekothapudi.com
  4. GoDaddy > Domain > DNS: delete the old A record for "@", then add
       A     @    185.199.108.153
       A     @    185.199.109.153
       A     @    185.199.110.153
       A     @    185.199.111.153
       CNAME www  <your-github-username>.github.io
  5. When DNS has updated (minutes to 48 hours), tick "Enforce HTTPS".

GoDaddy Website Builder (Airo) cannot host an uploaded HTML file.
If the domain is attached to Website Builder, use Option A or B.

After it is live: add the site in Google Search Console and submit
https://www.venkatakishorekothapudi.com/sitemap.xml
