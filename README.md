[![forthebadge](https://forthebadge.com/images/badges/uses-html.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/uses-css.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/made-with-javascript.svg)](https://forthebadge.com)

# simple-component-library

A library of React components created using `create-react-app`.

modal-by-yflly is a modal library, Flexible, configurable and accessible way to display modals for your application.

## Installation

Install modal-by-yflly with npm

```bash
npm i modal-by-yflly
```

Install ReactLightModal with yarn

```bash
yarn add modal-by-yflly
```

## Usage/Examples

```javascript
import Modal from "modal-by-yflly";
import React, { useState } from "react";

const [modal, setModal] = useState(false);

const toggleModal = () => {
  setModal(!modal);
};

function App() {
  return <Modal />;
}
```

## Props

| Name            | Type          | Required | Description                                                              | Default value     |
| --------------- | ------------- | -------- | ------------------------------------------------------------------------ | ----------------- |
| canClose        | `boolean`     | `false`  | Display cross button on the top-right of the modal box                   | `true`            |
| closeBtnContent | `JSX.element` | `false`  | Custom content add on the close button (exemple: personalized icon, ...) | `{<span>X</span}` |
| footerContent   | `JSX.element` | `false`  | Custom content to add to the footer (exemple: action buttons, ...)       | `{}`              |
| haveFooter      | `boolean`     | `false`  | If his value is true, the modal have footer element                      | `false`           |
| isOpen          | `boolean`     | `true`   | If his value is true, the modal is displayed                             | `false`           |
| modalContent    | `JSX.element` | `true`   | Content of the modal                                                     | `{}`              |
| title           | `string`      | `false`  | Modal header title                                                       | `""`              |
