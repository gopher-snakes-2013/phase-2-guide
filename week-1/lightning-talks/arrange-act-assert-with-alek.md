# Arrange Act Assert with Alek

1. When you're writing your code and you're stranded, call triple
1. Arrange, Act, Assert

## Arrange

Set up your context for your test. Set up the information (declaring variables,
instantiating collaborators, etc.)

```
describe "Welcome to the Jungle" do
  it "likes fun and games" do
    jungle = Jungle.new
  end
end
```

## Act

This is where you call the method you're testing

```
describe "Welcome to the Jungle" do
  it "likes fun and games"  do
    jungle = Jungle.new
    jungle.add_monkey("Bonzo")
  end
end
```

## Assert

This is where you check to ensure the method under test did what it was supposed
to do

```
describe "Welcome to the Jungle" do
  it "likes fun and games"  do
    jungle = Jungle.new
    jungle.add_monkey("Bonzo")
    expect(jungle.monkeys).to include("Bonzo")
  end
end
```
