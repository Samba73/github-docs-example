# Writing Good Documentation
Following some are ToDo and Not ToDo

> [!NOTE]
> Try to use codeblocks to maximum

> [!IMPORTANT]
> Keep documentation clean

> [!WARNING]
> Never use screenshot from mobile

GitHub supports formatting [<sup>[1]</sup>](#external-references)

## Step 1 - Using Codeblocks [^1]

- Codeblocks in markdown make it *very easy* for tech people to **copy, paste, share** code. 
- A good Cloud Engineer uses Codeblocks whenever possible.

Because it __allows others__ to copy and paste their code to replicate or research issues.

- In order to create codeblocks in markdown you need to use three backticks  (`)
- Not to be confused with quotation mark (')

```
private void buildLayout() {
        HorizontalLayout actions = new HorizontalLayout(filter, newContact);
        actions.setWidth("100%");
        filter.setWidth("100%");
        actions.setExpandRatio(filter, 1);

        VerticalLayout left = new VerticalLayout(actions, contactList);
        left.setSizeFull();
        contactList.setSizeFull();
        left.setExpandRatio(contactList, 1);

        HorizontalLayout mainLayout = new HorizontalLayout(left, contactForm);
        mainLayout.setSizeFull();
        mainLayout.setExpandRatio(left, 1);

        // Split and allow resizing
        setContent(mainLayout);
    }
    void refreshContacts() {
        refreshContacts(filter.getValue());
    }
```

- when you can you should attempt to apply syntax highlighting to your codeblocks

```java
private void buildLayout() {
      HorizontalLayout actions = new HorizontalLayout(filter, newContact);
      actions.setWidth("100%");
      filter.setWidth("100%");
      actions.setExpandRatio(filter, 1);

      VerticalLayout left = new VerticalLayout(actions, contactList);
      left.setSizeFull();
      contactList.setSizeFull();
      left.setExpandRatio(contactList, 1);

      HorizontalLayout mainLayout = new HorizontalLayout(left, contactForm);
      mainLayout.setSizeFull();
      mainLayout.setExpandRatio(left, 1);

      // Split and allow resizing
      setContent(mainLayout);
  }
  void refreshContacts() {
      refreshContacts(filter.getValue());
  }
```
- GitHub Flavored Markdown supports image
- Add folder to store images and reference in src as below in 1
- Also can use the markdown format for image as in 2
  
<img width="200px" src="assets/blackcat.jpg" />

![Black Cat](assets/c607a848-4988-4e01-8b0a-fe059fbeab7a.jpg)

Good Cloud Engineers use codeblocks for both Code and Errors that appear in the console.

```bash
Traceback (most recent call last):
  File "sample_code.py", line 7, in <module>
    result = divide(10, 0)
  File "sample_code.py", line 3, in divide
    return a / b
ZeroDivisionError: division by zero
```
> Here is an example of using codeblocks for an error that appear in bash

External References[^11]

## Step 3 - Use Task Lists

GitHub markdown supports creating Task Lists [<sup>[2]</sup>](#external-references)

## Task Lists[^2]

- [x] Start watching post live videos
- [x] Execute the work while watching videos
- [ ] Complete all the tasks before next session
- [ ] Take notes in class

## Step 4 - Use Emojis (Optional) [^3]

GitHub Flavored Markdown (GFM) supports emoji shortcodes.[<sup>[3]</sup>](#external-references)
- :cloud:
- :cloud_with_lightning_and_rain:

## Step 5 - How to create a table [^4]

GitHub Flavored Markdown (GGFM) supports table formatting [<sup>[4]</sup>](#external-references)

```md
|Name|Shortcode|Emoji|
|---|---|---|
|Cloud|`:cloud:`|:cloud:|
|Soon|`:soon:`|:soon:|
|Recycle|`:recycle:`|:recycle:|
|8:30|`:clock830:`|🕣|
|11:00|`:clock11:`|:clock11:|
```


[^1]: Using Codeblocks
[^2]: Task Lists
[^3]: Emoji
[^4]: Table


## External References

- [Basic writing and formatting syntax (Github Flavored Markdown)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)<sup>[1]</sup>
- [GFM - Task Lists](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists) <sup>[2]</sup>
- [GFM - Emoji CheatSheet](https://github/com/ikatyang/emoji-cheat-sheet)<sup>[3]</sup>
- > also refer [Emoji CheatSheet](https://gist.github.com/rxaviers/7360908)
- [GFM - Table (with extensions)](https://github.github.com/gfm/#tables-extension-)<sup>[4]</sup> 
