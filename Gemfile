source "https://rubygems.org"
ruby "3.1.4"

gem 'scan_left', '~> 0.2.1'
plugin 'bootboot', '~> 0.2.1' 

Plugin.send(:load_plugin, 'bootboot') if Plugin.installed?('bootboot')

if ENV['DEPENDENCIES_NEXT']
  enable_dual_booting if Plugin.installed?('bootboot')

  # Add any gem you want here, they will be loaded only when running
  # bundler command prefixed with `DEPENDENCIES_NEXT=1`.
end
