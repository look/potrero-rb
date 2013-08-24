desc 'Build and deploy to web server'
task :deploy do
  server = 'potrerorb.org'
  sh "jekyll build"
  sh "rsync --recursive --times --compress --human-readable --progress --delete _site/ lukefrancl@#{server}:~/potrerorb.org/"
end
