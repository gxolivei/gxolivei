```ruby
class SoftwareEngineer
  attr_accessor :name, :current_work, :hobbies, :github_profile

  def initialize(name, current_work, hobbies, github_profile)
    @name = name
    @current_work = current_work
    @hobbies = hobbies
    @github_profile = github_profile
  end

  def get_city(city)
    city.call
  end

  def get_ambitions(ambitions)
    ambitions.map(&:call)
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

gabriel = SoftwareEngineer.new('Gabriel', 'Team Lead @ KIS', gabriel_hobbies, 'Personal')

city = -> { 'Florianópolis' }
ambitions = [-> { 'Building a SaaS' }, -> { 'Expanding knowledge' }]
```

```ruby
puts "City: #{gabriel.get_city(city)}"
puts "Ambitions:"
puts gabriel.get_ambitions(ambitions)
```

<div align="center">

<table>
  <tr style="background-color: #161B22;">
    <th style="color: white;;">Stats</th>
    <th style="color: white;">Languages</th>
  </tr>
  <tr>
    <td><a href=""> <img align="center" src="https://github-readme-stats-sigma-five.vercel.app/api?username=gxolivei&theme=react&bg_color=161B22&hide_border=true"/> </a></td>
    <td><a href=""> <img align="center" src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=gxolivei&layout=compact&theme=react&&bg_color=161B22&hide_border=true"/> </a></td>
  </tr>
</table>

</div>
