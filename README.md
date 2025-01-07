class Smartphone:
    def __init__(self, brand, model, battery_life):
        self.brand = brand
        self.model = model
        self.battery_life = battery_life  # in hours
    
    def make_call(self, number):
        print(f"Calling {number} from {self.brand} {self.model}.")
    
    def send_message(self, number, message):
        print(f"Sending message to {number}: '{message}'")

    def show_info(self):
        return f"{self.brand} - Model: {self.model}, Battery Life: {self.battery_life} hours"

# Example of creating an object of Smartphone.
my_phone = Smartphone("Apple", "iPhone 14", 20)
print(my_phone.show_info())
my_phone.make_call("+1234567890")

inheritance

class CameraSmartphone(Smartphone): 
    def __init__(self, brand ,model,battery_life,camera_megapixels):  
       super().__init__(brand ,model,battery_life)   
       self.camera_megapixels=camera_megapixels  

   # Overriding method for showing info with camera details     
   def show_info(self):      
      base_info=super().show_info()       
      return f"{base_info}, Camera Megapixels: {str( self.camera_megapixels)} MP"
        
camera_smartphone=my_camera_smartphones=("Samsung","Galaxy S21",25,"108")         
print(camera_smartphoneshowinfo())          

activity 2

class Animal:
     """Base animal class"""
     pass


class Dog(Animal):

def move():
         print("Running on four legs ")


Class Cat(Animal):

def Move(): 
          Print ("Jumping gracefully ")


Class Bird(animal)

Def Move()
           Print ("Flying high up in the sky ")

# Create instances for each animal type.
dog_instance=Dog ()
cat_instance=Cat () 
bird_Instance=Bird()

for instance In [ dog Instance cat_Instance bird_Instance]:
            instance.move()
