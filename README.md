```ruby
class Person
  attr_accessor :name, :current_work, :hobbies

  def initialize(name, current_work, hobbies)
    @name = name
    @current_work = current_work
    @hobbies = hobbies
  end

  def get_city(city)
    city.call
  end

  def get_ambitions(ambitions)
    ambitions.map do |ambition|
      ambition.call
    end
  end
end

gabriel_hobbies = [
  'Reading', 
  'Listening to Classical Music', 
  'Studying New Technologies', 
  'Going Out with Family', 
  'Meeting Friends', 
  'Laughing as Much as Possible'
]
gabriel = Person.new('Gabriel', 'Coding at Twygo', gabriel_hobbies)

city = -> { 'Florianópolis' }
ambitions = [-> { 'Getting better at coding' }, -> { 'Building a SaaS' }]

puts "City: #{gabriel.get_city(city)}"
puts "Ambitions:", gabriel.get_ambitions(ambitions)
``` 

