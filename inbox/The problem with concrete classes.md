#SolidPrinciples #DependencyInversionPrinciple

"When Gear hard-codes a reference to Wheel deep inside its gear_inches method, it is explicitly declaring that it is only willing to calculate gear inches for instances of Wheel. Gear refuses to collaborate with any other kind of object, even if that object has a diameter and uses gears."

Sandi Metz, Practical Object-Oriented Design, p42