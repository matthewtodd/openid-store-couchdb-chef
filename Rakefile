this_rakefile_uses_shoe = <<END
----------------------------------------
Please install Shoe:
gem sources --add http://gems.github.com
gem install matthewtodd-shoe
----------------------------------------
END

begin
  gem 'matthewtodd-shoe'
rescue Gem::LoadError
  abort this_rakefile_uses_shoe
else
  require 'shoe'
end

Shoe.tie('openid-store-couchdb-chef', '0.1.0', 'A Chef-specific OpenID store for CouchDB.') do |spec|
  spec.add_dependency 'chef'
end
