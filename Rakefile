# -*- ruby -*-

require 'rubygems'
Gem::manage_gems
require 'rake/gempackagetask'

spec = Gem::Specification.new do |s|
  s.name = "keychain"
  s.version = "0.2.2"
  s.author = "Mikio L. Braun"
  s.email = "mikiobraun@gmail.com"
  s.homepage = "http://ml.cs.tu-berlin.de/~mikio"
  s.platform = Gem::Platform::RUBY
  s.summary = "A simple shell tool for managing passwords"
  s.files = Dir['bin/*']
  s.executables = 'keychain'
  s.add_dependency("crypt", ">= 1.1.4")
  s.add_dependency("highline", ">= 1.4.0")
  s.extra_rdoc_files = ["README", "ChangeLog"]
  s.rubyforge_project = 'keychain'
end

Rake::GemPackageTask.new(spec) do |pkg|
  pkg.need_tar = true
end
