<div align="center">
  
  |   Stats   |   Languages    |
  | :---: | :---: |
  | <a href=""> <img align="center" src="https://github-readme-stats-sigma-five.vercel.app/api?username=gxolivei&hide=contribs,prs&theme=react&bg_color=00000000&hide_border=true"/> </a> | <a href=""> <img align="center" src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=gxolivei&layout=compact&theme=react&&bg_color=00000000&hide_border=true"/> </a> |

</div>

```
I am Gabriel, a software developer with a passion for all things computer-related.
Always looking for new projects to work on and expand my knowledge and skills
```

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
```

```ruby
gabriel_hobbies = [
  'Creating all things computer-related',
  'Reading', 
  'Listening to Classical Music', 
  'Studying New Technologies', 
  'Going Out with Family', 
  'Meeting Friends', 
  'Laughing as Much as Possible'
]
gabriel = Person.new('Gabriel', 'Software Developer at Twygo', gabriel_hobbies)

city = -> { 'Florianópolis' }
ambitions = [-> { 'Getting better at coding' }, -> { 'Building a SaaS' }, -> { 'Expanding knowledge' }]
```

```ruby
puts "City: #{gabriel.get_city(city)}"
puts "Ambitions:", gabriel.get_ambitions(ambitions)
```
