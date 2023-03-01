# ElDatePicker Patch

> build on ElementUI version: 2.5.17, code from [feat(date-picker): add yearrange type](https://github.com/ElemeFE/element/pull/17101/files)

## feature

+ support yearrange

## build

```
npm install
npm run lib
```

The built files are located in `dist/ElDatePicker`

## usage

### copy

+ dist/ElDatePicker/ElDatePicker.umd.min.js
+ dist/ElDatePicker/ElDatePicker.css
+ fonts/

### import

`ElDatePicker.umd.min.js` and `ElDatePicker.css`

```js
import ElDatePicker from '/yourpath/ElDatePicker.umd.min.js'
import '/yourpath/ElDatePicker.css'
Vue.component('ElDatePickerPatched', ElDatePicker)
```

### example

```vue
<template>
    <el-date-picker-patched
        v-model="value1"
        start-placeholder="start year"
        end-placeholder="end year"
        type="yearrange"
        range-separator="-"
        size="small"
    />
    ...
</template>

<script>
    ...
    data() {
        return {
            value1: '',
            ...
        }
    }
    ...
</script>
```

## known bug

If ElDatePicker is directly overridden, the z-index of the year picker in the popup will be incorrectly calculated.
