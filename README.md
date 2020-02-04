# rust-xcode-plugin

This plugin is provided as-is with no guarantees of any kind.

Syntax highlighting isn't great, but setting breakpoints in the GUI should work.

Based on: 
https://github.com/youknowone/rust-xcode-langspec
https://github.com/steventroughtonsmith/lua-xclangspec

If your Xcode UUID is not listed [here](https://github.com/mtak-/rust-xcode-plugin/blob/master/Plug-ins/Rust.ideplugin/Contents/Info.plist), please make an issue (or a pull request!) and I'll add it.

You can check your UUID with this command:
```sh
$ defaults read /Applications/Xcode.app/Contents/Info DVTPlugInCompatibilityUUID
```
Once the UUID is added, execute the `setup.sh` script

You may have to quit and reopen Xcode once or twice and click the `Load Bundle` button in a popup that should appear automatically.

## Manual Install
Place the `Plug-ins`  folders in `~Library/Developer/Xcode`

Place the `Rust.xclangspec` in `/Applications/Xcode.app/Contents/SharedFrameworks/SourceModel.framework/Versions/A/Resources/LanguageSpecifications`

Place `Xcode.SourceCodeLanguage.Rust.plist` in `/Applications/Xcode.app/Contents/SharedFrameworks/SourceModel.framework/Versions/A/Resources/LanguageMetadata`



