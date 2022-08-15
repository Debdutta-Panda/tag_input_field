Flutter package to create easily customizable tag input field.

![image](https://user-images.githubusercontent.com/92369023/184599618-f9c6516e-7d09-4fd0-9ad7-bc602dade902.png)


<a href="https://www.buymeacoffee.com/debduttapanda" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

## Features

- Put tag by pressing comma after tag content.
- Put tag(s) by pasting comma separated contents.
- Autocomplete feature.
- Fully customizable. Almost every part can be customized.
- delete tag(s) by backspace. Not possible in iOS with soft keyboard.

## Support

PRs Welcome

Discord [Channel](https://rebrand.ly/yozuou8)

Check the [repo](https://github.com/Debdutta-Panda/tag_input_field) to contribute

Don't forget to give a ⭐

## Have a look
![tag_input_field](https://user-images.githubusercontent.com/92369023/184590173-c309247f-7a1f-4275-bb89-36d5adb99d94.png)


## Demo
[Live Demo](https://tag_input_field.codemagic.app/#/)

![device-2022-08-15-124047](https://user-images.githubusercontent.com/92369023/184592891-f8c39595-2552-4f17-8f2c-23266a126150.gif)

## Getting Started

```
TagInputField(
  hint: "Tags",
  onBeforeTagAdded: (_)=>true,
  onBeforeTagsAdded: (_)=>true,
  onItemWillBeDeleted: (_)=>true,
  onTagAdded: (_){},
  onTagsAdded: (_){},
  onTagDeleted: (_){},
  autocomplete: true,
  optionBuilder: (tev){
    var text = tev.text;
    if(text.isEmpty){
      return [];
    }
    return [
      "$text 1",
      "$text 2",
      "$text 3",
      "$text 4",
    ];
  },
)
```
