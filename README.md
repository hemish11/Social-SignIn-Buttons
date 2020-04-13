# social_signin_buttons

A Flutter package for both android and iOS which provides Social signIn Buttons

## Screenshots

![Image](screenshots/ss.png =200x350)
## Usage

[Example]()

To use this package :

* add the dependency to your [pubspec.yaml]() file.

```yaml
  dependencies:
    flutter:
      sdk: flutter
    social_signin_buttons:
```

### How to use

```dart
class Test extends StatelessWidget {
 
  void _showButtonPressDialog(BuildContext context, String btn) {
    Scaffold.of(context).showSnackBar(SnackBar(
      content: Text('$btn Button Pressed!'),
      backgroundColor: Colors.black26,
      duration: Duration(milliseconds: 400),
    ));
  }

  @override
  Widget build(BuildContext context) {
    return Container(
      child: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: <Widget>[
            SignInButton(
              Buttons.Google,
              onPressed: () {
                _showButtonPressDialog(context, 'Google');
              },
            ),
            Divider(),
            SignInButton(
              Buttons.Facebook,
              onPressed: () {
                _showButtonPressDialog(context, 'Facebook');
              },
            ),
            Divider(),
            SignInButton(
              Buttons.Apple,
              onPressed: () {
                _showButtonPressDialog(context, 'Apple');
              },
            ),
            Divider(),
            SignInButton(
              Buttons.Microsoft,
              onPressed: () {
                _showButtonPressDialog(context, 'Microsoft');
              },
            ),
            Divider(),
            SignInButton(
              Buttons.GitHub,
              text: "Sign up with GitHub",
              onPressed: () {
                _showButtonPressDialog(context, 'Github');
              },
            ),
            Divider(),
            SignInButton(
              Buttons.Twitter,
              text: "Sign In with Twitter",
              onPressed: () {
                _showButtonPressDialog(context, 'Twitter');
              },
            ),
            Divider(),
          ],
        ),
      ),
    );
  }
}

```


# License
Copyright (c) 2020 Parth Patel

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


## Getting Started

For help getting started with Flutter, view our online [documentation](https://flutter.io/).

For help on editing package code, view the [documentation](https://flutter.io/developing-packages/).