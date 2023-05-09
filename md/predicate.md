# Predicate Methods

```ruby
# Using nil?
nil.nil?           # => true
"foo".nil?         # => false

# Using blank?
"".blank?          # => true
"  ".blank?        # => true
[].blank?          # => true
[1, 2, 3].blank?   # => false
{}.blank?          # => true
{foo: "bar"}.blank? # => false

# Using present?
nil.present?           # => false
"foo".present?         # => true

# Using empty?
"".empty?          # => true
"  ".empty?        # => false
[].empty?          # => true
[1, 2, 3].empty?   # => false
{}.empty?          # => true
{foo: "bar"}.empty? # => false

# Using any?
[].any?          # => false
[1, 2, 3].any?   # => true
{}.any?          # => false
{foo: "bar"}.any? # => true
