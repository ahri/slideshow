task :default => :generate

SLIDESHOW = "slideshow.html"

desc "Generate slideshow (default)"
task :generate => SLIDESHOW
file SLIDESHOW => "slideshow.md" do |t| 
  sh "pandoc --self-contained -t revealjs --section-divs --variable theme=solarized --variable transition=concave -o #{t.name} #{t.source}"
end

desc "Start the slideshow"
task :start => :generate do
  sh "google-chrome --incognito #{SLIDESHOW}"
end

desc "Switch on the VGA output"
task :screen_on do
  sh "xrandr --output VGA1 --auto --above LVDS1"
end
 
desc "Switcon off the VGA output"
task :screen_off do
  sh "xrandr --output VGA1 --off"
end
