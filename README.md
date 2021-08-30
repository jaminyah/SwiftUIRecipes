# SwiftUI Recipes

```bash
1. Button

```

1. Button - Center Aligned

```swift
import SwiftUI

struct ContentView: View {
 
    var body: some View {
        Button(action: { print("Hello, World!")}) {
                    Text("Greet")
                        .font(.system(size: 16))
                        .fontWeight(.bold)
                        .foregroundColor(.blue)
                        .padding(10)
                        .background(RoundedRectangle(cornerRadius: 10).stroke().foregroundColor(Color.red))
                        .cornerRadius(10)
                }
        .buttonStyle(DefaultButtonStyle())
    }
}
```