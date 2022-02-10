# Installation

To install the library, use the command below

````
    npm i @eddy_rock_js/rock-ui
````
# Basic usage

````
<template>
    <div>
        <rock-input v-model="value" />
    </div>
</template>

<script>
import { RockInput } from '@eddy_rock_js/rock-ui';

module.exports = {
    components: {
        RockInput
    },
    data: () => {
        return {
            value: '',
        }
    }
};

</script>

````
