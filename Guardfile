# Reload the browser when a served file changes.
# See https://github.com/guard/guard#readme

guard 'livereload' do
  watch("index.html")
  watch(%r{^css/.+\.css$})
  watch(%r{^assets/.+\.(css|js)$})
  watch(%r{^assets/.+\.(jpg|jpeg|png|gif|svg|webp)$})
end
