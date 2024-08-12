"""1 задание"""

# class Fruit:
#     def __init__(self, name , color, weight):
#         self.name = name
#         self.color = color
#         self.weight = weight
#     def info(self):
#       print(f'название-{self.name}, цвет-{self.color}, weight-{self.weight}')
# frukt = Fruit('авакадо супер пупер сигма фрукт', 'зелены цвет крутой авакадо', '1кг это очень много для авакадо')
# frukt.info()

#2 задание
# class Book:
#     def __init__(self, title , author, pages):
#         self.title = title
#         self.author = author
#         self.pages = pages
        
        
#     def info(self):
#       print(f'название-{self.title}, автор-{self.author}, страницы-{self.pages}')
#     def check_pages(self):
#        if self.pages < 100:
#           print("тонка книжка она не сигма")
#        elif self.pages <= 200:
#           print("средная она средне сигма")
#        else: 
#           print("она супер пупер мега сигма она большая")

# kniga = Book('kniga suli sigmy', 'suli sigmsa krutoi avtor', 100)
# kniga.info()
# kniga.check_pages()
"""второе"""
#1# задание "в нутри этого задание несколько заданий"
# class Person:
#     def __init__(self, fullname , age, is_married):
#         self.fullname = fullname
#         self.age = age
#         self.is_married = is_married
        
#     def introduce_myself(self):
#         print(f" Имя {self.fullname}, Возраст {self.age}, вторая половина {self.is_married}")
        
# people = Person("Султан", 13, "Не женат")
# people.introduce_myself()
# #2#задание и в нем тоже несколько заданий
# class Teacher(Person):
#     def __init__ (self, experience):
#         self.experience = experience
#         self.salary = 0
#         for i in range(self.experience):
#             self.salary += 3000
#         print(f'Зарплата {self.salary}')
#     def experiance(self):
#         print(f"опыт работы у этой тичер {self.experience} лет и зарплата {self.salary}")
# teach = Teacher(13)
# teach.experiance()
        
        
        
        
        
"""третье"""
# class Computer:
#     def __init__(self, cpu, memory):
#         self.__cpu = cpu
#         self.__memory = memory
        
#     @property
#     def cpu(self):
#         return self.__cpu
    
#     @property
#     def memory(self):
#         return self.__memory
    
#     def __make_computations(self):
#         cpu = self.__cpu
#         memory = self.__memory
        
#     @property
#     def make_computations(self):
#         return self.__make_computations

#     def ekran_vyvod(self):
#         print(f"Вычитание {self.__cpu - self.__memory}\nПрибавление {self.__cpu + self.__memory}\nУмножение {self.__cpu * self.__memory}\nДеление {self.__cpu / self.__memory}")
        
# computer = Computer(8, 4)
# computer.ekran_vyvod()
# print(f'cpu: {computer.cpu}')
# print(f'Memory: {computer.memory}')



# class Laptop(Computer):
#     def __init__(self, cpu, memory, memory_card):
#         super().__init__(cpu, memory)  
#         self.__memory_card = memory_card

#     @property
#     def memory_card(self):
#         return self.__memory_card

#     def info(self):
#         print(f"Карта памяти: {self.__memory_card} гб, Процессор: {self.cpu}, Память: {self.memory}")

#     def vyvod_na_ekran(self):
#         print(f"Карта памяти: {self.memory_card}")


# laptop = Laptop(4,8,50)
# laptop.info()
# print(f'Memory Card: {laptop.memory_card}')
# laptop.vyvod_na_ekran()
# laptop.ekran_vyvod()
# laptop.make_computations()
"""четвертое"""
# class Vehicle:
#     def move(self, transport,bak):
#         pass

# class Car(Vehicle):
#     def move(self, transport):
#         return f"машина {transport} по дороге"
    
#     def fuel(self, bak):
#         return f"машина {bak} топливо"

# class Bicycle(Vehicle):
#     def move(self, transport):
#         return f"велосипед {transport} по дороге"
#     def fuel(self,bak):
#         return f"велосипед {bak} силу"
# class Boat(Vehicle):
#     def move(self, transport):
#         return f"корабль {transport} по воде"
    
#     def fuel(self, bak):
#         return f"корабль {bak} дизель"

# transportlist = [Bicycle(), Boat(), Car()]

# for vehicle in transportlist:
#     print(vehicle.move('движется'))

# for km in transportlist:
#     print(km.fuel('расходует'))
