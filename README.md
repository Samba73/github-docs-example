# Writing Good Documentation

GitHub supports formatting [<sup>[1]</sup>](#references)

## Step 1 - Using Codeblocks

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
The references has here <sup>[1]</sup>

<img width="200px" src="https://github.com/Samba73/github-docs-example/assets/90577515/1dd03ee5-d534-4095-8a9d-41eeba2b5f59" />

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



## Step 3 - Use Task Lists

GitHub markdown supports creating Task Lists <sup>[2]</sup>

## Task Lists

- [x] Start watching post live videos
- [x] Execute the work while watching videos
- [ ] Complete all the tasks before next session
- [ ] Take notes in class

## Step 4 - Use Emojis (Optional)

GitHub Flavored Markdown (GFM) supports emoji shortcodes.<sup>[3]</sup>
- :cloud:
- :cloud_with_lightning_and_rain:

## Step 5 - How to create a table 

GitHub Flavored Markdown (GGFM) supports table formatting [<sup>[4]</sup>](#references)

```md
|Name|Shortcode|Emoji|
|---|---|---|
|Cloud|`:cloud:`|:cloud:|
|Soon|`:soon:`|:soon:|
|Recycle|`:recycle:`|:recycle:|
|8:30|`:clock830:`|🕣|
|11:00|`:clock11:`|:clock11:|
```



## References

- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/)
- [Basic writing and formatting syntax (Github Flavored Markdown)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)<sup>[1]</sup>
- [GFM - Task Lists](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists) <sup>[2]</sup>
- [GFM - Emoji CheatSheet](https://github/com/ikatyang/emoji-cheat-sheet)<sup>[3]</sup>
- > also refer [Emoji CheatSheet](https://gist.github.com/rxaviers/7360908)
- [GFM - Table (with extensions)](https://github.github.com/gfm/#tables-extension-)<sup>[4]</sup> 
