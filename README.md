# class
class Equipment:
    def __init__(self, name, equipment_type, capacity, power, cost, section, surface_type, depth, length, width):
        self.name = name
        self.type = equipment_type
        self.capacity = capacity
        self.power = power
        self.cost = cost
        self.section = section
        self.surface_type = surface_type
        self.depth = depth
        self.length = length
        self.width = width
    def __str__(self):
        return f"{self.name} - {self.type} - {self.capacity} - {self.power} - {self.cost} - {self.section} - {self.surface_type} - {self.depth} - {self.length} - {self.width}"
class Environment:
    def __init__(self, equipment_name, utilization, mtbf, mttr):
        self.equipment_name = equipment_name
        self.utilization = utilization
        self.mtbf = mtbf
        self.mttr = mttr
    def __str__(self):
        return f"{self.equipment_name} - Utilization: {self.utilization}, MTBF: {self.mtbf}, MTTR: {self.mttr}"
# Example Usage
drill1 = Equipment("Drill1", "Rotary", "2000m", "4500kW", "NA", "East", "Surface", "200m", "1000m", "800m")
truck1_utilization = Environment("Truck1", 0.75, "200hrs", "1 day")
# Print the details
print(drill1)
print(truck1_utilization)
