# react-native-carousel-view

react-native carousel, work on both `iOS` and `android`, test on RN 0.46.1

## Demo
<table>
  <tr>
    <th>
      Android
    </th>
    <th>
      iOS
    </th>
  </tr>
  <tr>
    <td>
      <img src="./example/android.gif" width="300" style="float: left;">
    </td>
    <td>
      <img src="./example/ios.gif" width="300" style="float: left;">
    </td>
  <tr>
</table>

## Props

```js
type Props = {
  hideIndicators: boolean,
  indicatorColor: string,
  indicatorSize: number,
  inactiveIndicatorColor: string,
  indicatorAtBottom: boolean,
  indicatorOffset: number,
  indicatorText: string,
  inactiveIndicatorText: string,
  width: ?number,
  initialPage: number,
  indicatorSpace: number,
  animate: boolean,
  delay: number,
  loop: boolean,
  contentContainerStyle?: {[attr: string]: any},
  children: any,
  onPageChange?: (number) => void,
}
```

default props:

```js
static defaultProps = {
  hideIndicators: false,
  indicatorColor: '#000000',
  indicatorSize: 20,
  inactiveIndicatorColor: '#999999',
  indicatorAtBottom: true,
  indicatorOffset: 0,
  indicatorText: '•',
  inactiveIndicatorText: '•',
  width: null,
  initialPage: 0,
  indicatorSpace: 10,
  animate: true,
  delay: 1000,
  loop: true,
}
```

## Examples

- Android: [Example](./example/index.android.js)

- iOS: [Example](./example/index.ios.js)

## Develop

go to `example` folder and enter `yarn install` and `yarn run haul`

select your platform:

```
➜  example git:(master) yarn run haul
yarn run v0.27.5
$ haul start
? Select platform to bundle for (Use arrow keys)
❯ ios - Serves iOS bundle
  android - Serves Android bundle
  all - Serves both platforms
```

and run `react-native run-ios` or `react-native run-android` to open simulators.

**TIPS** if you want to live reload `example` when modified `react-native-carousel-view`, use `yarn link`!

## NOTE

this repo is original from https://github.com/nick/react-native-carousel with lots of improvements.

## License

Apache 2.0