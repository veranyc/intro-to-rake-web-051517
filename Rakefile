namespace :greeting do

  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hola to the terminal'
  task :hola do
    puts "hola de Rake!"
  end

end

desc 'migrate changes to your datebase'
  namespace :db do
    task :migrate => :environment do
      Student.create_table
    end
  end

desc 'allow connection to the DB'
  task :environment do
    require_relative './config/environment.rb'
  end

  desc 'seed the database with some dummy data'
  namespace :db do
    task :seed do
      require_relative './db/seeds.rb'
    end
  end

  desc 'drop into the Pry console'
    task :console => :environment do
      Pry.start
    end
