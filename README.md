# Build
bundle exec jekyll build

# Server the content
cd _site
bundle exec jekyll serve

# Access the website
http://localhost:4000

# For production build with analytics-scripts.js

JEKYLL_ENV=production bundle exec jekyll build

# 
{% if jekyll.environment == "production" %}
  <script src="my-analytics-script.js"></script>
{% endif %}
