# Xcoed

Xcoed (Xcode co-ed) - Use a `Package.swift` manifest for an Xcode project.

**Currently, only libraries that have the same name as their package are supported.**
**Currently, only packages with range version requirements are supported.**

## Installation:

* Meant to be used with [Xcake](https://github.com/igor-makarov/xcake) or some other Xcodeproj generator.
* Add `gem 'xcoed'` in your Gemfile
* Add a `before_save` hook:  
```ruby
project.before_save do |project|
  Xcoed::integrate_package_swift! project
end
```

For more info, look at [DemoXcoed](https://github.com/igor-makarov/DemoXcoed) project.