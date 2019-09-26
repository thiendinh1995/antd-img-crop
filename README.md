# fit-img-crop

An image cropper for Ant Design [Upload](https://ant.design/components/upload/).

[![npm](https://img.shields.io/npm/v/antd-img-crop.svg?style=flat-square)](https://www.npmjs.com/package/antd-img-crop)
[![npm](https://img.shields.io/npm/dt/antd-img-crop?style=flat-square)](https://www.npmtrends.com/antd-img-crop)
[![npm bundle size](https://img.shields.io/bundlephobia/minzip/antd-img-crop?style=flat-square)](https://bundlephobia.com/result?p=antd-img-crop)
[![GitHub](https://img.shields.io/github/license/nanxiaobei/antd-img-crop?style=flat-square)](https://github.com/nanxiaobei/antd-img-crop/blob/master/LICENSE)

English | [简体中文](./README.zh-CN.md)

## Demo

[![Edit fit-img-crop](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/antd-img-crop-4qoom5p9x4?fontsize=14)

## Install

```sh
yarn add fit-img-crop
```

## Usage

```jsx harmony
import ImgCrop from 'fit-img-crop';
import { Upload } from 'antd';

const Demo = () => (
  <ImgCrop>
    <Upload>+ Add image</Upload>
  </ImgCrop>
);
```

## Props

| Name          | Type       | Default        | Description                                                                                                                                                                   |
| ------------- | ---------- | -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| width         | `number`   | `100`          | Crop width in `px`. If `useRatio` is `true`, it'll be ratio.                                                                                                                  |
| height        | `number`   | `100`          | Crop height in `px`. If `useRatio` is `true`, it'll be ratio.                                                                                                                 |
| useRatio      | `boolean`  | `false`        | If use `width` and `height` as ratio, not real `px`. And crop will fill the width or height. e.g. `width={500} height={400}` and `width={5} height={4}` are exactly the same. |
| resize        | `boolean`  | `true`         | If crop can resize.                                                                                                                                                           |
| resizeAndDrag | `boolean`  | `true`         | If crop can resize and drag.                                                                                                                                                  |
| modalTitle    | `string`   | `"Edit image"` | Modal title.                                                                                                                                                                  |
| modalWidth    | `number`   | `520`          | Modal width in `px`.                                                                                                                                                          |
| beforeCrop    | `function` | -              | Execute before crop, if return `false`, modal will not open (Not support `Promise`). Ant Design Upload `beforeUpload` prop will execute after crop, before upload.            |

## License

[MIT License](https://github.com/nanxiaobei/antd-img-crop/blob/master/LICENSE) (c) [nanxiaobei](https://mrlee.me/)
