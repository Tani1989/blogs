# Create your first Blazor Apps

Required Steps


Creating my first Blazor App

Bootstrap of Razor
Upon building of A Razor Application, the Script tag replaced with another script tag containing the Blazor and other dependent dll


Following highligted  replaced with the Code for the DLL Loading..



when you build the blazor app this script tag will actually get replaced. it'll get replaced with another script tag that references the a piece of JavaScript that's used to bootstrap the donet runtime within the browser and also to point it at the applications entry points.  
so you see this script tag here  so here it got that that's the blazer blazer boot script that got replaced and it's we replaced it with a reference to this blazer that j/s file "<script src="_framework/blazor.js" " this is what's gonna get the web assembly code for the.net runtime up and running.

 it also has the main entry point for the application  main="FirstBlazor.dll" entrypoint="FirstBlazor.Program::Main"  so there's the web application - is the DLL that was built from my project and then as all the references that are needed by the application this is all the references that were specified as part of the compilation step trimmed down -






 just the things that that we know are absolutely needed so we actually do on every build aisle stripping will remove assemblies that aren't used and il code from assemblies that aren't actually used at all in fact so if we go back to the app and try to build again make it the output up let's see if we can do a rebuild we should see that so if we watch the the output spew by hopefully. t's like pulling out all this stuff that my app doesn't actually need and that helps reduce the size of the the application payload and I'll reduce load times now this is just saying that reducing the load time




Every Blazor Component is defined by any CSHTML File. IT generates a strongly typed name..


Why do we have this?
    <app>Loading...</app>

App is the root component.

    <!-- The DOM element selector argument determines where the root component will get rendered.
        In our case, the app element in index.html is used. 
        This gets displayed only till the time the blazor component is loading..
        -->

Where is the .Net Runtime getting loaded?
Mono.wasm. A lot of optimizations coming, which will remove the code..





Tooling
Intellisense available for components..

Note: Live Reload not yet there..

Components
Can be paramererize like Attributes, and defined like properties in the blazor componennt


How do you do Layout in Blazor?

<!-- TO define the layout of all the pages.-->
@layout MainLayout



@bind syntax is going to Change..


