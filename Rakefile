# Look in the tasks/setup.rb file for the various options that can be
# configured in this Rakefile. The .rake files in the tasks directory
# are where the options are used.

begin
  require 'bones'
  Bones.setup
rescue LoadError
  load 'tasks/setup.rb'
end

ensure_in_path 'lib'
require 'juicer'

task :default => 'spec:run'

PROJ.name = 'Juicer'
PROJ.authors = 'Christian Johansen'
PROJ.email = 'christian@cjohansen.no'
PROJ.url = 'http://www.cjohansen.no/en/projects/juicer'
PROJ.version = Juicer::VERSION
PROJ.rubyforge.name = 'juicer'

PROJ.spec.opts << '--color'

# EOF