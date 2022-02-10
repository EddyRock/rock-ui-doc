# UI Components

## Button

* disabled - makes the button not clickable - **Boolean**
* secondary - makes the button lighter - **Boolean**

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

* disabled - makes the checkbox not clickable - **Boolean**
* default - default value - **Boolean** 
* title - adds label to the checkbox - **String**

````vue
<template>
  <rock-checkbox
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
      disabled: false,
      default: false,
      title: 'Title',
    };
  }
};
</script>
````

## Icon-button

* disabled - makes the button not clickable - **Boolean**

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
