# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require File.expand_path('../config/application', __FILE__)

Rails.application.load_tasks

if Rails.env.development?
  begin
    require 'vlad'
    require 'vlad-extras'
    Vlad.load(scm: :git, app: :passenger, type: :rails)
  rescue
    puts 'Could not load Vlad'
  end
end

