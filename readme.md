# js-match-height

Dependency-free vanilla js plugin to match element heights, in a tiny file (2kb).

## Getting Started

```
npm i js-match-height --save
```

### Use

Import the library and simply instatiate with your elements, no options required. MatchHeight will correct heights if needed on window resize, using a debounce method to improve performance. 

```
import { MatchHeight } from 'js-match-height';
```

Pass your elements. 

```
const matchHeight = new MatchHeight('ul.list-items  li');
```

The timeout for the debounce method is defaulted at 250. You can set your time if needed. 

```
const matchHeight = new MatchHeight('ul.list-items  li', { timeout:400 });
```

You can manually trigger a height recalculation with the update method. This is useful if the DOM itself changes without a window resize. 

```
matchHeight.update();
```

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE) file for details

## Acknowledgments

* jquery match height
