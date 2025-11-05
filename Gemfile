source 'https://rubygems.org'

# You may use http://rbenv.org/ or https://rvm.io/ to install and use this version
ruby ">= 3.0.0"

# Cocoapods 1.15 introduced a bug which break the build. We will remove the upper
# bound in the template on Cocoapods with next React Native release.
gem 'cocoapods', '>= 1.13', '< 1.15'
gem 'activesupport', '>= 6.1.7.5', '< 7.1.0'
# concurrent-ruby v1.3.5 has removed the dependency on logger
# https://stackoverflow.com/a/79361034
gem 'concurrent-ruby', '1.3.4'
# https://github.com/fastlane/fastlane/issues/20960#issuecomment-1413333159
# https://github.com/fastlane/fastlane/pull/21442
# gem "fastlane", "= 2.210.1"
# https://github.com/fastlane/fastlane/discussions/21178
# gem "fastlane", :git => "https://github.com/fastlane/fastlane.git", :branch => "joshdholtz/apple-auth-sirp"
gem 'fastlane', '= 2.225.0'
#
# Add bigdecimal explicitly due to Ruby 3.4.0 changes
gem 'bigdecimal' # Ensure to specify a version compatible with your needs

plugins_path = File.join(File.dirname(__FILE__), 'fastlane', 'Pluginfile')
eval_gemfile(plugins_path) if File.exist?(plugins_path)
