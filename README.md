# &lt;miller-columns&gt; element

Express a hierarchy by showing selectable lists of the items in each hierarchy level.

Selection of any item shows that item’s children in the next list.

## Installation

```
npm install --save miller-columns-element
```

## Usage

```html
<miller-columns class="miller-columns" for="taxonomy" selected="selected-items" id="miller-columns">
  <ul id="taxonomy">
    <li>
      <input type="checkbox" id="parenting-childcare-and-children-s-services">
      <label for="parenting-childcare-and-children-s-services">Parenting, childcare and children's services</label>
    </li>
    <ul>
      <li>
        <input type="checkbox" id="divorce-separation-and-legal-issues">
        <label for="divorce-separation-and-legal-issues">Divorce, separation and legal issues</label>
      </li>
      <li>
        <input type="checkbox" id="childcare-and-early-years">
        <label for="childcare-and-early-years">Childcare and early years</label>
      </li>
    </ul>
  </ul>
</miller-columns>

<miller-columns-selected id="selected-items" for="miller-columns" class="miller-columns-selected"></miller-columns-selected>

```

## Browser support

Browsers without native [custom element support][support] require a [polyfill][].

- Chrome
- Firefox
- Safari
- Internet Explorer 11
- Microsoft Edge

[support]: https://caniuse.com/#feat=custom-elementsv1
[polyfill]: https://github.com/webcomponents/custom-elements

## Development

```
npm install
npm test
```

To continuously build files while developing run:

```
npm run watch
```

## License

Distributed under the MIT license. See LICENSE for details.