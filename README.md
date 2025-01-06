# InlineSvgLoader

A lightweight React component for dynamically fetching, modifying, and rendering inline SVGs with class support and error handling.

## Contributing

We welcome contributions to the `react-tailwind-svg` project! If you encounter any issues or would like to contribute, feel free to open an issue or a pull request on our GitHub repository.

[GitHub Repository](https://github.com/Pawan-Khushraho/react-tailwind-svg)

## Issues

If you face any issues or have suggestions for improvement, please [raise an issue](https://github.com/Pawan-Khushraho/react-tailwind-svg/issues) on GitHub.

## Features

- Fetch SVGs from a remote URL dynamically.
- Modify SVG paths to support `currentColor` for better theming.
- Remove hardcoded height and width for responsive rendering.
- Built-in loading and error handling.

## Installation

Install the package using NPM or Yarn:

```bash
npm install react-tailwind-svg
```

Or

```bash
yarn add react-tailwind-svg
```

## Usage

Here’s how you can use the `InlineSvgLoader` in your React project. It supports custom class names, including **Tailwind CSS** classes, for styling.

### Example

```tsx
import React from 'react';
import InlineSvgLoader from 'react-tailwind-svg';

const App = () => {
  return (
    <div>
      <h1>SVG Loader Example</h1>
      <InlineSvgLoader 
        src="/path/to/your/svg.svg" 
        className="h-10 w-10 text-blue-500 dark:text-red-500" 
      />
    </div>
  );
};

export default App;


### Props

| Prop       | Type     | Required | Description                                           |
|------------|----------|----------|-------------------------------------------------------|
| `src`      | `string` | Yes      | URL of the SVG to fetch.                              |
| `className`| `string` | No       | Custom class name for styling, including Tailwind CSS.|
