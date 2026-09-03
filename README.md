# BC Sans

The standard font for B.C. Government digital services is BC Sans. BC Sans is an open source font family, and is a modified version of Noto Sans, developed by Google. BC Sans includes modifications to support Indigenous languages in British Columbia. B.C. Government is currently working to include Indigenous languages in government records, systems and services. Find out what steps are being taken and how you can stay informed at [Including Indigenous languages in government records, systems and services](https://www2.gov.bc.ca/gov/content?id=666A1FD778FA437994E419A98662ED5C#new).

Font weights and styles included:

- BC Sans Regular - 400
- BC Sans Italic - 400
- BC Sans Bold - 700
- BC Sans Bold Italic - 700
- BC Sans Light - 300
- BC Sans Light Italic - 300

### Typography

For digital typography guidance, please see [B.C. Design System > Foundations > Typography](https://www2.gov.bc.ca/gov/content?id=72C2CD6E05494C84B9A072DD9C6A5342).

For print typography guidance, please see [B.C. Visual Identity Program > Design Guidelines](https://www2.gov.bc.ca/gov/content?id=CCB4862101CD43C195FF395CAED00F95#palette-typography).

### Download Files

If you are wanting the fonts in different file formats, here are all the options

- [Download all font files](https://www2.gov.bc.ca/assets/gov/british-columbians-our-governments/services-policies-for-government/policies-procedures-standards/web-content-development-guides/corporate-identity-assets/bcsansfont_web.zip) (.eot, .ttf, .otf, .woff, .woff2)
- [Download files for your local computer](https://www2.gov.bc.ca/assets/gov/british-columbians-our-governments/services-policies-for-government/policies-procedures-standards/web-content-development-guides/corporate-identity-assets/bcsansfont_print.zip) (.otf, .ttf)

### Integration

`npm i --save @bcgov/bc-sans`

In a root-level component: `import "@bcgov/bc-sans/css/BC_Sans.css";`

Reference `BC Sans` in your CSS `font-family` rules. Consider using the typography tokens from [@bcgov/design-tokens](https://www.npmjs.com/package/@bcgov/design-tokens).

### Why are there two similar CSS files in this package?

You only need to include one of the two CSS files: `css/BC_Sans.css`.

> [!WARNING]
> ⚠️ **Beginning with version 3 of the BC Sans, [support for the incorrect `BCSans` font name will be dropped](https://github.com/bcgov/bc-sans/issues/28).** ⚠️

Projects that use the legacy `css/BCSans.css` file should **migrate to `css/BC_Sans.css`** and update their CSS rules to reference the correct `BC Sans` as font name.

Versions of this package up to v2.0.0 shipped with only `css/BCSans.css`. This file uses the incorrect name `BCSans` (no space) as the `font-family` name in its `@font-face` declarations.

The correct font name (matching the metadata in the font files) is `BC Sans` (with a space). `css/BC_Sans.css` uses `BC Sans` for its CSS `font-family` names. UI design tools like Figma output code using the `BC Sans` name from the font files.

### Contributing

Integrating it differently? [Create a pull request](https://github.com/bcgov/bc-sans/pulls) to help us build out the documentation.
