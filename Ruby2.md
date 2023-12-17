# クラスとインスタンス
```
class Human
 def hello
  puts "おはよう"
 end
end

human = Human.new
human.hello
```

# 呼び出す
```
def hello #①
  puts "Hello World"
end

class Human
  def self.hello #②
    puts "Hello World"
  end

  def hello #③
    puts "Hello World"
  end
end

①hello
②Human.hello
③human = Human.new
human.hello
```
