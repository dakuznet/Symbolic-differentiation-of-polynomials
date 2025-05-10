# SymbolicDifferentiationOfPolynomials

Gem for symbolic differentiation of polynomials in Ruby. Convert string expressions of polynomials to their derivatives with automatic simplification. 

## Installation

Install the gem and add to the application's Gemfile by executing:

```bash
bundle add symbolic_differentiation_of_polynomials
```

If bundler is not being used to manage dependencies, install the gem by executing:

```bash
gem install symbolic_differentiation_of_polynomials
```

## Usage

```ruby
require 'symbolic_differentiation_of_polynomials'

# The derivative of x
puts SymbolicDiff.derive("x^2 + 4*x + 3", 'x') # => "2*x + 4"

# The derivative of y
puts SymbolicDiff.derive("x^3 + 2*y^2", 'y')   # => "4*y"
```

Examples

Expression 	  Variable 	  Result
x^2 + 3*x	  x	          2*x + 3
5*y^3 + 2*y	  y	          15*y^2 + 2
4*x^5 - x^2	  x	          20*x^4 - 2*x

Features
✅ Supported operations:

Addition (+)

Multiplication (*)

Degree (^)

Constants and variables

Unary minus

🔄 Automatic simplification:

x + 0 → x

3*x*2 → 6*x

x^1 → x

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and the created tag, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/dakuznet/Symbolic-differentiation-of-polynomials.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
