[Text within the brackets are comments]: #

Normal Text <br>
*Italic Text* <br>
**Bold Text** <br>
***Bold Italic***

# Heading 1
## Heading 2
### Heading 3



Here’s a step-by-step guide to preview your page locally with Jekyll so you can see exactly how it will look before publishing:

1️⃣ Install Ruby (if not installed)

Jekyll runs on Ruby, so first check if you have it:

ruby -v
If it prints a version (e.g., ruby 3.1.2), you’re good
If not, install Ruby from https://www.ruby-lang.org/en/documentation/installation/

2️⃣ Install Jekyll and Bundler

Run this in your terminal:

gem install jekyll bundler
Jekyll → converts your Markdown/YAML to HTML
Bundler → manages dependencies, including themes

3️⃣ Clone or create your repo locally
git clone https://github.com/yourusername/yourcompany.github.io.git
cd yourcompany.github.io

Or if you’re starting fresh:

mkdir yourcompany.github.io
cd yourcompany.github.io

Place your files (_config.yml, index.md, etc.) here.

4️⃣ Add your theme to the Gemfile

If you use a GitHub Pages theme (like cayman):

Create a Gemfile in the repo:
source "https://rubygems.org"
gem "github-pages", group: :jekyll_plugins
Install dependencies:
bundle install

This ensures your theme works locally just like on GitHub Pages.

5️⃣ Serve your site locally

Run:

bundle exec jekyll serve

You’ll see output like:

Configuration file: /path/to/_config.yml
Source: /path/to/repo
Destination: /path/to/repo/_site
Server address: http://127.0.0.1:4000/
Server running... press ctrl-c to stop.

6️⃣ Open your browser

Go to:

http://localhost:4000
You’ll see your finance company page with theme styling
Works exactly like GitHub Pages, but locally

7️⃣ Edit & auto-refresh
Change index.md, _config.yml, or other Markdown files
The site auto-refreshes at localhost:4000
Great for previewing updates before publishing

8️⃣ Stop the server

Press:

Ctrl + C

This stops the local server when you’re done testing.

⚡ Pro Tips
Use bundle exec jekyll serve --livereload to auto-refresh your browser whenever you save files.
Always test links, headers, and footers locally before deploying.
You can preview multiple pages if you add them as .md files with front matter.
