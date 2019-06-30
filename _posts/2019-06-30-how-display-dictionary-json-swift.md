---
layout: "post"
title: "How to display a dictionary in JSON format"
---

If you want to show a Swift dictionary in JSON format you can use the following line that shows it by console.
* parameters is your dictionary

```swift
print(String(data: try! JSONSerialization.data(withJSONObject: parameters, options: .prettyPrinted), encoding: .utf8)!)
```

#Swift