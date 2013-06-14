# Botscout [![Build Status](https://travis-ci.org/parallel588/botscout.png?branch=master)](https://travis-ci.org/parallel588/botscout)


## Installation

Add this line to your application's Gemfile:

    gem 'botscout'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install botscout

## Usage

    botscout = Botscout::Client.new("key")
    result = botscout.test mail: email
    if result.success?
        Logger.info "Email address is spam: #{email}" if result.bot?
    else
        Logger.info "Servis is not available: #{result.error}"
    end


## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
