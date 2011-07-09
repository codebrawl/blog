require 'net/ssh'

desc 'update site from remote repo'
task :update do
  puts `rm -rf _site/ && jekyll && rsync -r _site/* codebrawl@codebrawl.com:shared/blog`
end