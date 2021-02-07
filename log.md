# log
Notes of the version and other things


## Version 0.0.0 (2021-02-07)
`url` <https://rubygems.org/gems/butiran>

### Create folders and files
```
> md butiran
> cd butiran
> md lib
```

```
> type butiran.gemspec
% cat hola.gemspec
Gem::Specification.new do |s|
  s.name        = 'butiran'
  s.version     = '0.0.0'
  s.summary     = "Butiran"
  s.description = "A simple hello world gem"
  s.authors     = ["Sparisoma Viridi"]
  s.email       = 'dudung@gmail.com'
  s.files       = ["lib/butiran.rb"]
  s.homepage    = 'https://rubygems.org/gems/butiran'
  s.license     = 'MIT'
end
```

```
> dir lib
 Volume in drive L is Linux
 Volume Serial Number is DC0D-53EE

 Directory of L:\home\butiran-rb\lib

2021-02-07  04:41 PM    <DIR>          .
2021-02-07  04:41 PM    <DIR>          ..
2021-02-07  04:45 PM                64 butiran.rb
               1 File(s)             64 bytes
               2 Dir(s)  64,118,218,752 bytes free
```

```
> type lib\butiran.rb
class Butiran
  def self.hi
    puts "butiran 0.0.0"
  end
end
```

```
> tree/f
Folder PATH listing for volume Linux
Volume serial number is DC0D-53EE
L:.
│   .gitignore
│   butiran.gemspec
│
└───lib
        butiran.rb
```

### Build gem
```
> gem build butiran.gemspec
  Successfully built RubyGem
  Name: butiran
  Version: 0.0.0
  File: butiran-0.0.0.gem
```

### Install gem
```
> gem install butiran-0.0.0.gem
Successfully installed butiran-0.0.0
Parsing documentation for butiran-0.0.0
Installing ri documentation for butiran-0.0.0
Done installing documentation for butiran after 3 seconds
1 gem installed
```

### Push out the gem
```
> gem push butiran-0.0.0.gem
Enter your RubyGems.org credentials.
Don't have an account yet? Create one at https://rubygems.org/sign_up
   Email:   dudung@gmail.com
Password:

Signed in.
Pushing gem to https://rubygems.org...
Successfully registered gem: butiran (0.0.0)
```

### Check the remote gem
```
> gem list -r butiran

*** REMOTE GEMS ***

butiran (0.0.0)
```

### Install it from RubyGems.org
```
> gem install butiran
Successfully installed butiran-0.0.0
Parsing documentation for butiran-0.0.0
Done installing documentation for butiran after 1 seconds
1 gem installed
```

### Sign out
```
> gem signout
You have successfully signed out from all sessions.
```

### Uninstall gem
```
> gem uninstall butiran
Successfully uninstalled butiran-0.0.0
```

## References
1. -, "Make you own gem", Guides, url <https://guides.rubygems.org/make-your-own-gem/> [20210207].
