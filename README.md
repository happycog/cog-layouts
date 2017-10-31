# Coglayouts

## Learn more
http://cognition.happycog.com/article/autolayout

## How to install
With [yarn](https://github.com/yarnpkg/yarn) do:

`yarn add cog-layouts`

With [npm](https://github.com/npm/npm) do:

`npm install -g cog-layouts`

## Usage

HTML
```
<section class="layout-split-2--sidebar">
  <main class="column">
  ...
  </main>
  <aside class="column">
  ...
  </aside>
</section>
```

SASS

`@import 'node_modules/dist/coglayouts';`

Custom Gutter
```
@import 'node_modules/dist/coglayouts';
// This line below will overwrite the default gutter of 20px;
$autolayoutDefaultGutter: 100px;
```


SASS Module
```
.layout-split-2 {
  @include autolayout('|-[]-[]-|');
  &--sidebar {
    @include autolayout('|-[75%]-[25%]-|');
    @include autolayout('|-[3/4]-[1/4]-|');
  }
}
```

## Example
[Codepen Example](http://codepen.io/markhuot/pen/kXJjWR)
