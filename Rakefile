#!/usr/bin/env rake

namespace :brew do
  task :enviroment do #FIXME
    ENV['HOMEBREW_CASK_OPTS'] = "--appdir=/Applications"
  end

  desc 'Setup homebrew'
  task setup: :enviroment  do
    `ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"`
  end

  desc 'Bundle'
  task bundle: :enviroment  do
    `brew bundle`
  end
end

namespace :nodebrew do
  desc 'Setup nodebrew'
  task :setup do
    `curl -L git.io/nodebrew | perl - setup`
  end

  desc 'Install nodejs v0.10.x'
  task :install do
    `~/.nodebrew/current/bin/nodebrew install-binary v0.10.x`
  end
end
