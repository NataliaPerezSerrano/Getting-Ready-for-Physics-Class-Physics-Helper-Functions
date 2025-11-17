# Getting-Ready-for-Physics-Class-Physics-Helper-Functions
Getting Ready for Physics Class — Physics Helper Functions

#temperature converter
def f_to_c(f_temp):
  c_temp = (f_temp - 32)*5/9
  return (c_temp)
#test de function with a variable
f100_in_celsius= 100

print(f_to_c(f100_in_celsius))

#new fonction

def c_to_f(c_temp):
  f_temp = ((c_temp*9/5) +32)
  return(f_temp)

#test of the function
c0_in_fahrenheit = 0
print(c_to_f(c0_in_fahrenheit))

# Uncomment this when you reach the "Use the Force" section
train_mass = 22680
train_acceleration = 10
train_distance = 100
bomb_mass = 1

# Write your code below: 
def get_force(mass, acceleration):
  force = mass*acceleration
  return force

#calling the function
train_force = get_force(train_mass, train_acceleration )
print(f'The GE train supplies {train_force} Newtons of force.')

#calcul of energy

def get_energy (mass, c=3*10**8):
  energy=mass * c**2
  return energy

#call the function
bomb_energy = get_energy(bomb_mass)
print(f'A 1kg bomb supplies {bomb_energy} Joules')

#Final function: Work

def get_work (mass, acceleration, distance):
  work= get_force(mass, acceleration) * distance
  return work

train_work = get_work(train_mass, train_acceleration, train_distance)

print(f'The GE train does {train_work} Joules of work over {train_distance} meters."')
