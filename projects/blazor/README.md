# Blazor (9)

You will find samples for Blazor, a .NET application framework for Web Assembly here. To run the sample, simply type `dotnet watch run` at the folder of each project. All these samples run on Blazor experimental release version 0.7. Make sure you pay attention which port Kestrel is running on.

  * [Hello World](https://github.com/dodyg/practical-aspnetcore/tree/master/projects/blazor/hello-world)

    The smallest Blazor app you can create.

  * [Component](https://github.com/dodyg/practical-aspnetcore/tree/master/projects/blazor/Component)

    This sample shows the simplest demonstration of a component (which is just a .cshtml file) that accept a string parameter. Notice that the folder name of the project is capitalized. That's due to this [limitation](https://github.com/aspnet/Blazor/issues/854)  e.g. the name of your folder is currently the name of the namespace used in a blazor app.

    A component is represented by a `<componentname></componentname>` in the markup. 

  * [Component Two - Reference and Call](https://github.com/dodyg/practical-aspnetcore/tree/master/projects/blazor/ComponentTwo)
  
    This sample shows how to refer to a component using `ref` property and call a public method of the component. We use the method `this.StateHasChanged();` to tell the component that its value has changed.

    Side note: If you are using `ref` without providing corresponding property at `functions`, the compilation will fail.
    
  * [Component Three - Child Content](https://github.com/dodyg/practical-aspnetcore/tree/master/projects/blazor/ComponentThree)

    Implement a component that takes one or more child content e.g. `<parentcomponent><childcomponent1/><childcomponent2/><parentcomponent>` and renders it. 

    You have to provide a parameter called `ChildContent` of type `RenderFragment`. The parameter name must be `ChildContent` otherwise it won't work.

  * [Component Four - Handling Custom Event from Component](https://github.com/dodyg/practical-aspnetcore/tree/master/projects/blazor/ComponentFour)

    This sample shows how to raise a custom event from a component and how to handle them.
   
  * [Component Five - Inherit from a BlazorComponent class](https://github.com/dodyg/practical-aspnetcore/tree/master/projects/blazor/ComponentFive)

    This sample shows how to inherit from a `BlazorComponent` class. This allows you to share common code across components. You can also use this technique to have a 'Code Behind' experience if that's your thing.

  * [Component Six - When to call StateHasChanged](https://github.com/dodyg/practical-aspnetcore/tree/master/projects/blazor/ComponentSix)

    This sample shows different behaviors by the component depending on where you call the method from. Note: __this is still tentative. It needs more exploration__. 


  * [Component Seven - Plain C#](https://github.com/dodyg/practical-aspnetcore/tree/master/projects/blazor/ComponentSeven)

    This sample demonstrates that you can use and organize your C# classes like in an ordinary C# app.

  * [Component Eight - Interactions between two components](https://github.com/dodyg/practical-aspnetcore/tree/master/projects/blazor/ComponentEight)

    This samples demonstrates the two way (__currently__) of facilitating interaction between two components.
