# Flex Grid Sass

## Installation

NPM Install:

```
$ npm i sass-flex-grid --save
```

Import to your scss file:

```
@import '../node_modules/sass-flex-grid/index.scss';
```

## Defaults:

### Breakpoints

```
$grid-breakpoints: (
  extra-small: (
    name: xs,
    columns: 12,
    gutter: 16px,
    min-width: 0
  ),
  small: (
    name: sm,
    columns: 12,
    gutter: 16px,
    min-width: 36em
  ),
  medium: (
    name: md,
    columns: 12,
    gutter: 24px,
    min-width: 48em
  ),
  large: (
    name: lg,
    columns: 12,
    gutter: 24px,
    min-width: 64em
  ),
  extra-large: (
    name: xl,
    columns: 12,
    gutter: 24px,
    min-width: 90em
  )
);
```

### Prefixing

By default there is no prefix:

```
$grid-prefix: '';
```

## Customization:

### Breakpoints:

You can add as many or as few as you would like!

```
$grid-breakpoints: (: (
	extra-small: (
		name: xs, // ".col-xs-*"
		columns: 4, // 4 colums at this breakpoint
		gutter: 16px, // 16 pixels between each column
		min-width: 0 // default, no min width
	),
	small: (
		name: sm, // ".col-sm-*"
		columns: 4, // 4 colums at this breakpoint
		gutter: 16px, // 16 pixels between each column
		min-width: 36em // min-with 576px
	),
	medium: (
		name: md, // ".col-md-*"
		columns: 12, // 12 colums at this breakpoint
		gutter: 24px, // 24 pixels between each column
		min-width: 48em // min-with 768px
	),
	large: (
		name: foo, // ".col-foo-*"
		columns: 12, // 12 colums at this breakpoint
		gutter: 24px, // 24 pixels between each column
		min-width: 64em // min-with 1024px
	)
);
```


### Prefixing

YOu can add a prefix to all classes:

```
$grid-prefix: 'namespace-';
```

Example:

```
<div class="namespace-row">
	<div class="namespace-col-xs"><div class="box"></div></div>
	<div class="namespace-col-xs"><div class="box"></div></div>
	<div class="namespace-col-xs"><div class="box"></div></div>
	<div class="namespace-col-xs"><div class="box"></div></div>
</div>
```
