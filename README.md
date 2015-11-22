# Jal.AssemblyFinder
Just another library to find assemblies

## How to use?
Tag your assembly adding the next attribute in your AssemblyInfo.cs file:

    [assembly: AssemblyTag("Tag")]
    
Initiate the finder

    var directory = AppDomain.CurrentDomain.BaseDirectory;
    AssemblyFinder.Current = new AssemblyFinder(directory);
    
Search the assemblies

    var assemblies = AssemblyFinder.Current.GetAssemblies("Tag");





