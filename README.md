## BC Sans

The standard font for B.C. Government digital services is BC Sans. BC Sans is an open source font family, and is a modified version of Noto Sans, developed by Google. BC Sans includes modifications to support Indigenous languages in British Columbia.

Font weights and styles included:

* BC Sans Regular - 400
* BC Sans Italic - 400
* BC Sans Bold - 700
* BC Sans Bold Italic - 700

Typography standards for print are on the [B.C. Visual Identity Program](https://www2.gov.bc.ca/gov/content/governments/services-for-government/policies-procedures/bc-visual-identity/design-guidelines#palette-typography) page.


### Download Files

If you are wanting the fonts in different file formats, here are all the options
* [Download files for web development](https://www2.gov.bc.ca/assets/gov/british-columbians-our-governments/services-policies-for-government/policies-procedures-standards/web-content-development-guides/corporate-identity-assets/visid-files/bc-sans-font-woff.zip) (.woff)
* [Download files for your local computer](https://www2.gov.bc.ca/assets/gov/british-columbians-our-governments/services-policies-for-government/policies-procedures-standards/web-content-development-guides/corporate-identity-assets/visid-files/bc-sans-font-otf.zip) (.otf)
* [Download all font files](https://www2.gov.bc.ca/assets/gov/british-columbians-our-governments/services-policies-for-government/policies-procedures-standards/web-content-development-guides/corporate-identity-assets/visid-files/bc-sans-font-all.zip) (.eot, .ttf, .otf, .woff, .woff2)


### Integration
`npm i --save @bcgov/bc-sans`

#### React

Embed into a root level component
`import '@bcgov/bc-sans/css/BCSans.css'`

#### Typography.js
>See Typography.js installation instructions [here](https://github.com/KyleAMathews/typography.js)
```js
import Typography from 'typography';
import '@bcgov/bc-sans/css/BCSans.css';

const typography = new Typography({
  baseFontSize: '16px',
  baseLineHeight: 1.25,
  headerFontFamily: ['BCSans', 'Noto Sans', 'Verdana', 'Arial', 'sans-serif'],
  bodyFontFamily: ['BCSans', 'Noto Sans', 'Verdana', 'Arial', 'sans-serif'],
  scaleRatio: 2.074,
});

export default typography;
```

#### Unpkg

Load your font from unpkg like by inserting a link element in the head of your website:

```html
<link rel="stylesheet" href="https://unpkg.com/@bcgov/bc-sans@1.0.2/css/BCSans.css"/>
```

Which will load regular, bold, italic, and bold-italic versions of the font. Alternatively you can load each one separately (or omit some) like so:

```html
<link rel="stylesheet" href="https://unpkg.com/@bcgov/bc-sans@1.0.2/css/BCSans-regular.css"/>
<link rel="stylesheet" href="https://unpkg.com/@bcgov/bc-sans@1.0.2/css/BCSans-bold.css"/>
<link rel="stylesheet" href="https://unpkg.com/@bcgov/bc-sans@1.0.2/css/BCSans-italic.css"/>
<link rel="stylesheet" href="https://unpkg.com/@bcgov/bc-sans@1.0.2/css/BCSans-bold-italic.css"/>
```


Integrating it differently? [Create a pull request](https://github.com/bcgov/bc-sans/pulls) to help us build out the documentation.


