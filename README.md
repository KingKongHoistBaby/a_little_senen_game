"""定义一个学生类，实例属性有name(姓名)，age（年龄），提示用户分别输入3个学生信息（姓名以及年龄），根据用户输入的信息创建3个学生对象，将这3个学生对象存入列表，遍历列表删除年龄小于18岁的学生对象，最后输出列表中剩余的学生信息"""
class Studentes:
    def __init__(self, name, age):
        self.name = name
        self.age = age
for i in range(0, 3):
    name = input("请输入姓名:")
    age = input("请输入年龄:")
    student = Studentes(name, age)
    list.append(student)
for student in list:
    if student.age < 18:
        list.remove(student)
for student in list:
    print("姓名:" + student.name + "年龄:%s" % student.age)
