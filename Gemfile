source "https://rubygems.org"

# Hello! This is where you manage which Jekyll version is used to run.
# When you want to use a different version, change it below, save the
# file and run `bundle install`. Run Jekyll with `bundle exec`, like so:
#
#     bundle exec jekyll serve
#
# This will help ensure the proper Jekyll version is running.
# Happy Jekylling!

# علقنا السطر الخاص بـ minima theme لأننا نستخدم github-pages
# gem "minima", "~> 2.5"

# استخدم gem الخاص بـ GitHub Pages لضمان التوافق
gem "github-pages", group: :jekyll_plugins

# إذا لديك أي إضافات plugins أخرى، اكتبها هنا
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
end

# لأن ويندوز و JRuby لا تشمل ملفات zoneinfo، نضيف هذه الـ gems
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# لتحسين الأداء عند المراقبة على ويندوز
gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]
