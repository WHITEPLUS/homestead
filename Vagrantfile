VAGRANTFILE_API_VERSION = "2"

path = "#{File.dirname(__FILE__)}"

require 'yaml'
require path + '/server/infrastructure.rb'

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  Infrastructure.configure(config, YAML::load(File.read(path + '/Infrastructure.yml')))
end
