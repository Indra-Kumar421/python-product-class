# python-product-class
class Product:
  def __init__(self,name,price,category):
    self.name = name
    self.price = price
    self.category = category
  def get_info(self):
    print(f"Name of the product: {self.name}")
    print(f"Price of the product: {self.price}")
    print(f"Category of the product: {self.category}")
    print()
  def apply_discount(self,discount):
    return self.price-self.price*discount/100

Book1 = Product("OOPs with java",500,"A+")
Book1.get_info()

Book2 = Product("Python",599,"A+")
Book2.get_info()

print("Discounted price of Book1 (20% discount):", Book1.apply_discount(20))
print("Discounted price of Book2 (10% discount):", Book2.apply_discount(10))
