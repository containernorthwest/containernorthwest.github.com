task :deploy, :dist, :params do |t, args|
  rsync_params = args[:params] || "--rsh='ssh -p22'"
  exec("jekyll --no-auto && rsync -avz #{rsync_params} --delete _site/ #{args[:dist]}")
end
