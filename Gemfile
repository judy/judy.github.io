source "https://rubygems.org"

ruby "~> 4.0"

# Local development only. The site is static HTML; GitHub Pages serves it
# verbatim (see .nojekyll). Nothing here runs in production.
group :development do
  gem "guard-livereload", "~> 2.5"  # reloads the browser on file changes
  gem "webrick", "~> 1.9"           # backs `ruby -run -e httpd`
  gem "base64", "~> 0.3"            # em-websocket needs it; not bundled since Ruby 3.4
end
