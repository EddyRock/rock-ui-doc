# UI Components

## Button

* disabled - makes the button not clickable, optional - **Boolean**
* secondary - makes the button lighter, optional - **Boolean**

````vue
<template>
  <rock-button
      :disabled="disabled"
      :secondary="secondary"      
  />
</template>

<script>
import { RockButton } from '@eddy_rock_js/rock-ui';

export default {
  name: 'component',
  components: {
    RockButton
  },
  data: () => {
    return {
      disabled: false,
      secondary: false
    };
  }
};
</script>
````

## Checkbox

* disabled - makes the checkbox not clickable, optional - **Boolean**
* default - default value, mandatory - **Boolean** 
* title - adds label to the checkbox, optional - **String**

````vue
<template>
  <rock-checkbox
      v-model="value"
      :disabled="disabled"
      :default="default"
      :title="title"
  />
</template>

<script>
import { RockCheckbox } from '@eddy_rock_js/rock-ui';

export default {
  name: 'component',
  components: {
    RockCheckbox
  },
  data: () => {
    return {
      value: false,
      disabled: false,
      default: false,
      title: 'Title',
    };
  }
};
</script>
````

## Icon-button

* disabled - makes the button not clickable, optional - **Boolean**

````vue
<template>
  <rock-icon-button
      :disabled="disabled"
  />
</template>

<script>
import { RockIconButton } from '@eddy_rock_js/rock-ui';

export default {
  name: 'component',
  components: {
    RockIconButton
  },
  data: () => {
    return {
      disabled: false,
    };
  }
};
</script>
````

## Input

* small - makes the input small size, optional - **Boolean**
* medium - makes the input medium size, optional - **Boolean**
* large - makes the input large size, optional - **Boolean**
* type - changes type of the input, accepts text, email, password. Optional - **String** 
* tip - adds small test under the input, optional - **String**
* subtitle - adds subtitle on the  of the input, optional - **String**
* placeholder - adds placeholder to the input, optional - **String**
* disabled - makes the input unavailable, optional - **String**
* error - adds on the bottom of the input red label, optional - **String**
* warning - adds orange border to the input, optional - **String**

````vue
<template>
  <rock-input
      v-model="value"
      :disabled="false"
      :small="false"
      :medium="false"
      :large="false"
      :warning="false"
      type="text"
      tip="some tip"
      subtitle="some subtitle"
      placeholder="placeholder"
      error="error"
  />
</template>

<script>
import { RockInput } from '@eddy_rock_js/rock-ui';

export default {
  name: 'component',
  components: {
    RockInput
  },
  data: () => {
    return {
      value: '',
    };
  }
};
</script>
````

## Label

* theme - changes theme of the label, mandatory - **String**

````vue
<template>
  <rock-label
    theme="success"
  >
    label
  </rock-label>
</template>

<script>
import { RockLabel } from '@eddy_rock_js/rock-ui';

export default {
  name: 'component',
  components: {
    RockLabel
  },
  data: () => {
    return {};
  }
};
</script>
````

## Loader

* line - thickness of the circle, optional - **Number**
* size - size of the circle, optional - **Number**
* speed - speed of loader spinning, optional - **Number**

````vue
<template>
  <rock-loader
    line="0.4"
    size="2"
    speed="1.1"
  >
    label
  </rock-loader>
</template>

<script>
import { RockLoader } from '@eddy_rock_js/rock-ui';

export default {
  name: 'component',
  components: {
    RockLoader
  },
  data: () => {
    return {};
  }
};
</script>
````
