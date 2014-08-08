SVN = 'svn'
CO_DIR = 'box2d-read-only'
REPO_ADDR = 'http://box2d.googlecode.com/svn/trunk/'

task :default => [:init, :update]

task :init do
  unless Dir.exist?(CO_DIR)
    sh "#{SVN} checkout #{REPO_ADDR} #{CO_DIR}"
  end
end

task :update do
  cd "#{CO_DIR}"
  sh "#{SVN} update"
end
 
