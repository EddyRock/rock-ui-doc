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

## Paginator
* length - the length of pages - **Number**
* totalVisible - how many pages you can see on the paginator - **Number**
* isShortVersion - turns on a sort version of paginator - **Boolean**
* hasNextPage - shows is next page exist, if not next button will be disabled - **Boolean**


````vue
<template>
  <rock-paginator
      :length="10"
      :totalVisible="3"
      isShortVersion
      hasNextPage="true"
  />
</template>

<script>
import { RockPaginator } from '@eddy_rock_js/rock-ui';

export default {
  name: 'component',
  components: {
    RockPaginator
  },
  data: () => {
    return {};
  }
};
</script>
````

## Progressbar
No need any special props.

````vue
<template>
  <rock-progressbar v-model="value" />
</template>

<script>
import { RockProgressbar } from '@eddy_rock_js/rock-ui';

export default {
  name: 'component',
  components: {
    RockProgressbar
  },
  data: () => {
    return {
      value: 10,
    };
  }
};
</script>
````

## Radiobutton

* buttons - adds different possible values

````vue
<template>
  <rock-radiobutton
      v-model="radio"
      class="main__radiobuttons"
      :buttons="buttons"
  />
</template>

<script>
import { RockRadiobutton } from '@eddy_rock_js/rock-ui';

export default {
  name: 'component',
  components: {
    RockRadiobutton
  },
  data: () => {
    return {
      buttons: [
        {
          name: 'One',
          value: 'one',
          disabled: true,
          active: true,
        },
        {
          name: 'Two',
          value: 'two',
          disabled: false,
        },
        {
          name: 'Three',
          value: 'three',
        },
      ],
      radio: null,
    };
  }
};
</script>
````
