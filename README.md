**JS-Learning-Log**

Taking helpful notes while learning JS

**Table of Contents**

# 1. Javascript

# 2. CLI, GIT, VS Code

## 2.1 CLI

## 2.2 GIT

## 2.3 VS Code

# 3. HTML

 All page content elements that should be rendered to the page go inside the body element. However, other important information goes inside the head element.

The head element is used to contain metadata about the document, such as its title, links to stylesheets, and scripts. Metadata is information about the page that isn't displayed directly on the page.

```
<!DOCTYPE html>
<html lang="en">
<!--all other elements go here-->
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="styles.css">
    <title>I love fucking asses</title>
  </head>
</html>
```

## 3.1 General Syntax

**comments**

`<!-- comment here -->`

**open link in new tab**

`target="_blank"`

`<a href="https://www.freecodecamp.org" target="_blank">freeCodeCamp</a>`

**cursive - emphasize a specific word or phrase**

`<p>I <em>love</em> fucking assholes</p>`

**bold - strong importance**

`<p>I <strong>love</strong> fucking assholes</p>`

## 3.2 Forms and Input

**Form and Action**

The action attribute indicates where form data should be sent

The default behavior of clicking a form button without any attributes submits the form to the location specified in the form's action attribute

To clarify, add a type

```
<form action="sent data here url">
  <button>Submit</button>
</form>
```

Add **checked** to input attributes to make a radio button or checkbox selected by default

**Fieldset**

The fieldset element is used to group related inputs and labels together in a web form. fieldset elements are block-level elements, meaning that they appear on a new line

Use legends to clarify forms with captions

`<legend>form caption</legend>`

```
<form action="sent data here url">
  <fieldset>
    <legend>Is your cat an indoor or outdoor cat?</legend>
    <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor" checked> Indoor</label>
    <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
  </fieldset>
  <fieldset>
    <legend>What's your cat's personality?</legend>
    <input id="loving" type="checkbox" name="personality" value="loving"> <label for="loving" checked>Loving</label>
    <input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>
    <input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic"> Energetic</label>
  </fieldset>
  <button>Submit</button>
</form>
```

**Button types**

- Submit

`<button type="submit">Submit</button>`

**Input**

The input element allows you several ways to collect data from a web form

- Text

name, placeholder, required

`<input type="text" name="catphotourl" placeholder="cat photo URL" required>`

- radio

Only one out of multiple answers

To make it so selecting one radio button automatically deselects the other, both buttons must have a name attribute with the same value

For convenience, set the button's value attribute to the same value as its id attribute

```
<label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
<label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
```

- checkbox

check multiple options

```
<legend>What's your cat's personality?</legend>
<input id="loving" type="checkbox"> Loving
```

**articles**

Article elements commonly contain multiple elements that have related information

```
<article>
  <p>French Vanilla</p>
  <p>3.00</p>
</article>
```

## 3.3 Best Practices

**Descriptions for images**

`<img src="cat.jpg" alt="A cat">`

**Labeling**

label elements are used to help associate the text for an input element with the input element itself (especially for assistive technologies like screen readers)

`<label><input type="radio"> Indoor</label>`

There's another way to associate an input element's text with the element itself. 
You can nest the text within a label element and add a for attribute with the same value as the input element's id attribute.

```
<input id="loving" type="checkbox" name="personality"> <label for="loving">Loving</label>
<input id="lazy" type="checkbox" name="personality"> <label for="lazy">Lazy</label>
```

## 3.4 SEO Optimization

**Section Elements**

define sections in a document, such as chapters, headers, footers, or any other sections of the document

`<section></section>`

**Self-contained Content**

`<figure>self-contained content</figure>`

`<figcaption>content caption</figcaption>`

```
<figure>
  <img src="favicon-192x192.png" alt="The beautiful MDN logo." />
  <figcaption>MDN Logo</figcaption>
</figure>
```

# 4. CSS

## 4.1 Syntax

**comment**

`/* comment here */`

```
h1 {
  text-align: center;
}
h2 {
  text-align: center;
}
p {
  text-align: center;
}
```

```
h1, h2, p {
  text-align: center;
}
```

## 4.2 Responsiveness

Make styling of the page to look similar on mobile as it does on a desktop or laptop

```
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
</head>
```

**Margin**

When the shorthand margin property has two values, it sets margin-top and margin-bottom to the first value, and margin-left and margin-right to the second value.

```
.yourclass {
  margin: 10px auto;
}
```

**Gradient**

Make colors fade into eachother. More than two colors possible

```
direction: 90deg - 90 right, 180 down, 270 left, 360 up (standard 180)
first color: red
second color: green
third clor: blue
fading starts at 75% of width - standard is 0%, 50%, 100% (equal distribution)

.red {
  background: linear-gradient(90deg, rgb(255, 0, 0) 75%, rgb(0, 255, 0), rgb(0, 0, 255);
}

.green {
  background: linear-gradient(#55680D, #71F53E, #116C31);
}

.blue {
  background: linear-gradient(hsl(186, 76%, 16%), hsl(223, 90%, 60%), hsl(240, 56%, 42%));
}
```

## 4.3 Selectors

[Selectors](https://www.w3schools.com/cssref/css_selectors.php)

# 5. Other Technologies

## 5.1 Browsers

# 6. Resources

## 6.1 General

## 6.2 Specific
