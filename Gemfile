source 'https://rubygems.org/'

ruby begin
  require 'yaml'
  YAML.safe_load(
    File.read(File.expand_path('dev.yml', __dir__)),
    symbolize_names: true
  ).fetch(:up).detect { _1.is_a?(Hash) && _1.key?(:ruby) }.fetch(:ruby)
end

gem 'google-protobuf'
gem 'rack'
