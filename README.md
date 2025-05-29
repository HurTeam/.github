# Roblox+ Editor SDK

Allows you to create plugins for Roblox+ Editor.
Framework version required : 4.7.2
LangVersion requried : latest

## Setup :

Right-click the project > Add Reference.

Go to Browse and select the Roblox+.Editor.SDK.dll file (or equivalent).

Click OK.

## Exemple of code :

```csharp

using Roblox__Editor_SDK___Version_1._0;
using Roblox__Editor_SDK___Version_1._0.Interfaces;
using System.Windows.Forms; -- only for (message box, etc..)

public class HelloPlugin : IPlugin
{
    public string Name => "Hello World";
    public string Description => "Displays a test message.";
    public string Version => "1.0";

    public void Execute(IEditorContext context)
    {
        MessageBox.Show("Hello from HelloPlugin!");
    }
}
