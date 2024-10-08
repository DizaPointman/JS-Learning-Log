**JS-Learning-Log**

Taking helpful notes while learning JS

**Table of Contents**

# 1. Javascript

# 2. CLI, GIT, VS Code

## 2.1 CLI

## 2.2 GIT

## 2.3 VS Code

# 3. HTML

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

**Fieldset**

The fieldset element is used to group related inputs and labels together in a web form. fieldset elements are block-level elements, meaning that they appear on a new line

Use legends to clarify forms with captions

`<legend>form caption</legend>`

```
<form action="sent data here url">
  <fieldset>
    <legend>form caption</legend>
    <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
    <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
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

## 3.3 Best Practices

**Descriptions for images**

`<img src="cat.jpg" alt="A cat">`

**Labeling**

label elements are used to help associate the text for an input element with the input element itself (especially for assistive technologies like screen readers)

`<label><input type="radio"> Indoor</label>`

There's another way to associate an input element's text with the element itself. 
You can nest the text within a label element and add a for attribute with the same value as the input element's id attribute.

```
<input id="loving" type="checkbox">
<label for="loving"> Loving </label>
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

# 5. Other Technologies

## 5.1 Browsers

# 6. Resources

## 6.1 General

## 6.2 Specific
