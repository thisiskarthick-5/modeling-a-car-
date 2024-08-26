# modeling-a-car-
modeling a car with python classes : attribute , method and object behavior



    class car:
    
        def __init__(self,brand,model,year):
            self.brand = brand
            self.model = model
            self.year = year
            self.mileage =0
            self.is_started = False
            
        def display(self):
            print(f"car brand : {self.brand}")
            print(f"car model : {self.model}")
            print(f"manufactured year : {self.year}")
            print(f"current mileage : {self.mileage} km")
            
         
        def start(self):
            if not self.is_started:
                self.is_started= True
                print(f"{self.brand} {self.model} is started ..")
            else:
                print("car is not starting")
                
        def drive(self,distance):
            if self.is_started:
                self.mileage += distance
                print(f"drove {distance} km.total mileage is now {self.mileage} km")
            else:
                print("first start the car") 
        
        def stop(self):
            if self.is_started:
                self.is_started=False
                print(f"{self.brand} {self.model} is stoped..")
            else:
                print("car is already stoped ") 
                
            
    car1 = car("bmw","tooto",2001)
    car1.display()
    car1.drive(50)
    car1.stop()
        
        
        
        




                           
            
            
        
