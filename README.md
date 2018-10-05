# Gatsby Plugin Tailwind CSS

## What

A Gatsby plugin to use Tailwind CSS with css-in-js. Like styled-components or emotion.js

## Usage

Inside your Gatsby project

```bash
npm install --save gatsby-plugin-tailwindcss tailwindcss
```

Init Tailwind configuration
```
npx tailwindcss init
```
It will add `tailwind.js` to your root project

Add this plugin to your gatsby-config.js.

```
module.exports = {
  plugins: ['gatsby-plugin-tailwindcss],
}
```

Add `tw` global to your `.eslintrc`

```
{
 ...
  "globals": {
    "tw": true
  },
 ...
}
```

You can now use Tailwind CSS with your favorite CSS-in-JS

### With Emotion

Install [gatsby-plugin-emotion](https://www.gatsbyjs.org/packages/gatsby-plugin-emotion/)

In your React Component

```javascript
import React from 'react'
import styled from 'react-emotion'


const Container = styled.div`
  ${tw`py-8`};
`
const Text = styled.p`
  ${tw`bg-black text-white`};
`

const Home = () => (
  <Container>
    <Text>I am Text component made with Tailwind CSS + EmotionJS</Text>
  </Container>
)

export default Home
```

### With Styled Components
Install [gatsby-plugin-styled-components](https://www.gatsbyjs.org/packages/gatsby-plugin-styled-components/).

In your React Component

```javascript
import React from 'react'
import styled from 'styled-components'


const Container = styled.div`
  ${tw`py-8`};
`
const Text = styled.p`
  ${tw`bg-black text-white`};
`

const Home = () => (
  <Container>
    <Text>I am Text component made with Tailwind CSS + Styled Components</Text>
  </Container>
)

export default Home
```

## Using Vscode

Try this snippet plugin [vscode-tailwind-styled-snippets](https://github.com/muhajirframe/vscode-tailwind-styled-snippets)

## For more information

- [Github](https://github.com/muhajirframe/gatsby-plugin-tailwindcss/)
- Got a question? [Submit an issue](https://github.com/muhajirframe/gatsby-plugin-tailwindcss/issues/new)

## Contributing

- [Submit an idea](https://github.com/muhajirframe/gatsby-plugin-tailwindcss/issues/new)
- Make a pull request

## Related
- [react-tailwind-emotion-starter](https://github.com/muhajirframe/react-tailwind-emotion-starter) A React + Tailwind + EmotionJs starter based on [create-react-app](https://github.com/facebook/create-react-app)
- [vscode-tailwind-styled-snippets](https://github.com/muhajirframe/vscode-tailwind-styled-snippets) A Snippet Plugin For VSCode. Made with Tailwind + CSS-in-JS in mind.


**Enjoy!**
