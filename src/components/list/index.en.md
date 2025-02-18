# List

Generic list.

## When to use

Carry text, lists, pictures, paragraphs, etc. cleanly and efficiently in the form of a list.

<code src="./demos/demo1.tsx"></code>

<code src="./demos/demo3.tsx"></code>

<code src="./demos/demo2.tsx"></code>

<code src="./demos/demo4.tsx"></code>

<code src="./demos/demo5.tsx"></code>

## List

### Props

| Name   | Description                          | Type                  | Default     |
| ------ | ------------------------------------ | --------------------- | ----------- |
| header | The title of list.                   | `ReactNode`           | -           |
| mode   | Support two modes: default and card. | `'default' \| 'card'` | `'default'` |

### CSS Variables

| Name                      | Description                                                                                     | Default                             |
| ------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------- |
| --header-font-size        | The font-size of the header                                                                     | `15px`                              |
| --prefix-width            | Width of the prefix part.                                                                       | `auto`                              |
| --prefix-padding-right    | The padding-right of the prefix part                                                            | `12px`                              |
| --active-background-color | The background color when clicked.                                                              | `var(--adm-border-color)`           |
| --align-items             | The [align-item](https://developer.mozilla.org/en-US/docs/Web/CSS/align-items) of the list item | `center`                            |
| --border-inner            | Border style of the list item bottom                                                            | `solid 1px var(--adm-border-color)` |
| --border-top              | Border style of the list top                                                                    | `solid 1px var(--adm-border-color)` |
| --border-bottom           | Border style of the list bottom                                                                 | `solid 1px var(--adm-border-color)` |
| --padding-left            | The padding-left of list item and header                                                        | `12px`                              |
| --padding-right           | The padding-right of list item and header                                                       | `12px`                              |
| --font-size               | The font-size of the list body                                                                  | `17px`                              |

## List.Item

### Props

| Name        | Description                                                                                                 | Type                            | Default                                                                              |
| ----------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------- | ------------------------------------------------------------------------------------ |
| title       | The title area in the upper middle of the list item.                                                        | `ReactNode`                     | -                                                                                    |
| children    | The main content area in the middle of the list item.                                                       | `ReactNode`                     | -                                                                                    |
| description | The description area in the lower middle of the list item.                                                  | `ReactNode`                     | -                                                                                    |
| prefix      | The left area of the list item.                                                                             | `ReactNode`                     | -                                                                                    |
| extra       | The right area of the list item.                                                                            | `ReactNode`                     | -                                                                                    |
| clickable   | Whether to show click effect.                                                                               | `boolean`                       | Defaults to `true` when the `onClick` prop is present, otherwise defaults to `false` |
| arrow       | Whether to show the arrow icon on the right side, also supports passing `ReactNode` to customize the icon.  | `boolean \| ReactNode`          | same as `clickable`                                                                  |
| disabled    | Is the list item disabled                                                                                   | `boolean`                       | `false`                                                                              |
| onClick     | The click event of the list item. When the `onClick` property is set, the list item will have click effect. | `(e: React.MouseEvent) => void` | -                                                                                    |

### CSS Variables

Support following css variables in List: `--prefix-width`, `--active-background-color` and `--align-items`

## FAQ

### Whether to support virtualized list?

List will not support virtualized list, you can implement it via using [react-virtualized](https://github.com/bvaughn/react-virtualized).

### Whether to support drag and drop the sorting?

List will not support Drag and drop the sorting, you can implement it via using [react-beautiful-dnd](https://github.com/atlassian/react-beautiful-dnd).
