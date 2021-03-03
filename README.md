# NexxUI (Open Beta)
A cross platform mobile GUI framework. NexxUI is built on top of Xamarin, which means your application can run on Android, iOS, and Windows. Support for MacOS X and Linux may be available in the future.

# NexxUI Syntax
NexxUI is very similar to JavaScript. It uses JSX like syntax to form GUI's. Here is a simple example of a NexxUI GUI:
example.nexx
```
// Create a component that inherits Button component to use in the UI
component CustomButton inherit Button {
  optional argument type = getArg(type);
  if type == "login" {
    override required argument text = "Login";
  }
}

UI ui = new UI();
ui.Define() {
  <CustomButton type="login">
}
```
