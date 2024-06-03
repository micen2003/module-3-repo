# module-3-repo
class Octopus
{
    public string Name;
    public readonly int Age = 10;
    public static readonly int Legs = 8, Eyes = 1;

    public Octopus(string name)
    {
        Name = name;
    }
}

var o = new Octopus("Jack");
o.Name.Dump();  // Output: Jack
o.Age.Dump();   // Output: 10
o.Legs.Dump();  // Output: 8

// Error: Cannot assign to readonly field
// o.Legs = 20;
