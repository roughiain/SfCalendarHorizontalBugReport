# README.md

Repo showing out of range exception on SFCalendar with `NavigationDirection="Horizontal"`

```text

System.Reflection.TargetInvocationException: Exception has been thrown by the target of an invocation.
 ---> System.ArgumentOutOfRangeException: Index was out of range. Must be non-negative and less than the size of the collection. (Parameter 'index')
   at Microsoft.Maui.Controls.Xaml.ApplyPropertiesVisitor.SetPropertyValue(Object xamlelement, XmlName propertyName, Object value, Object rootElement, INode node, HydrationContext context, IXmlLineInfo lineInfo)
   at Microsoft.Maui.Controls.Xaml.ApplyPropertiesVisitor.Visit(ValueNode node, INode parentNode)
   at Microsoft.Maui.Controls.Xaml.ValueNode.Accept(IXamlNodeVisitor visitor, INode parentNode)
   at Microsoft.Maui.Controls.Xaml.ElementNode.Accept(IXamlNodeVisitor visitor, INode parentNode)
   at Microsoft.Maui.Controls.Xaml.ElementNode.Accept(IXamlNodeVisitor visitor, INode parentNode)
   at Microsoft.Maui.Controls.Xaml.ElementNode.Accept(IXamlNodeVisitor visitor, INode parentNode)
   at Microsoft.Maui.Controls.Xaml.RootNode.Accept(IXamlNodeVisitor visitor, INode parentNode)
   at Microsoft.Maui.Controls.Xaml.XamlLoader.Visit(RootNode rootnode, HydrationContext visitorContext, Boolean useDesignProperties)
   at Microsoft.Maui.Controls.Xaml.XamlLoader.Load(Object view, String xaml, Assembly rootAssembly, Boolean useDesignProperties)
   at Microsoft.Maui.Controls.Xaml.XamlLoader.Load(Object view, String xaml, Boolean useDesignProperties)
   at Microsoft.Maui.Controls.Xaml.XamlLoader.Load(Object view, Type callingType)
   at Microsoft.Maui.Controls.Xaml.Extensions.LoadFromXaml[MainPage](MainPage view, Type callingType)
   at SfCalendarHorizontal.MainPage.InitializeComponent() in SfCalendarHorizontal/SfCalendarHorizontal/Microsoft.Maui.Controls.SourceGen/Microsoft.Maui.Controls.SourceGen.CodeBehindGenerator/MainPage.xaml.sg.cs:line 30
   at SfCalendarHorizontal.MainPage..ctor() in SfCalendarHorizontal/SfCalendarHorizontal/MainPage.xaml.cs:line 9
   at System.Reflection.MethodBaseInvoker.InterpretedInvoke_Constructor(Object obj, IntPtr* args)
   at System.Reflection.MethodBaseInvoker.InvokeWithNoArgs(Object obj, BindingFlags invokeAttr)
   --- End of inner exception stack trace ---
   at System.Reflection.MethodBaseInvoker.InvokeWithNoArgs(Object obj, BindingFlags invokeAttr)
   at System.RuntimeType.CreateInstanceMono(Boolean nonPublic, Boolean wrapExceptions)
   at System.RuntimeType.CreateInstanceDefaultCtor(Boolean publicOnly, Boolean wrapExceptions)
   at System.Activator.CreateInstance(Type type, Boolean nonPublic, Boolean wrapExceptions)
   at System.Activator.CreateInstance(Type type, Boolean nonPublic)
   at System.Activator.CreateInstance(Type type)
   at Microsoft.Maui.Controls.ShellContent.<>c__DisplayClass19_0.<Microsoft.Maui.Controls.IShellContentController.GetOrCreateContent>b__0()
   at Microsoft.Maui.Controls.ElementTemplate.CreateContent()
   at Microsoft.Maui.Controls.Internals.DataTemplateExtensions.CreateContent(DataTemplate self, Object item, BindableObject container)
   at Microsoft.Maui.Controls.ShellContent.Microsoft.Maui.Controls.IShellContentController.GetOrCreateContent()
   at Microsoft.Maui.Controls.Platform.Compatibility.ShellSectionRootRenderer.LoadRenderers()
   at Microsoft.Maui.Controls.Platform.Compatibility.ShellSectionRootRenderer.ViewDidLoad()
   at UIKit.UIApplication.UIApplicationMain(Int32 argc, String[] argv, IntPtr principalClassName, IntPtr delegateClassName) in /Users/builder/azdo/_work/1/s/xamarin-macios/src/UIKit/UIApplication.cs:line 58
   at UIKit.UIApplication.Main(String[] args, Type principalClass, Type delegateClass) in /Users/builder/azdo/_work/1/s/xamarin-macios/src/UIKit/UIApplication.cs:line 94
   at SfCalendarHorizontal.Program.Main(String[] args) in SfCalendarHorizontal/SfCalendarHorizontal/Platforms/iOS/Program.cs:line 13

```

## NB Licence key is not commited to the repo.
