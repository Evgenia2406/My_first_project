

import pytest
dz = ["Россия", "Франция", "Великобритания"]
capital = [["Москва", "123.5678"], ["Париж" "344.674567"], ["Лондон", "567.97403"]]
my_dict = {}
for i in range(len(dz)):
    my_dict[dz[i]] = capital[i]

print(my_dict)

def test_one():
    assert 'Россия' in my_dict

def test_two():
    assert my_dict['Россия'] == ["Москва", "1235678"]

def test_three():
    assert dict(my_dict)

def test_four():
    assert 'Великобритания' in my_dict
