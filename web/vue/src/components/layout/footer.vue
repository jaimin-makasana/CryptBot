<template lang='pug'>
  footer.p2.bg--off-white
    .contain
      p
        em Use CryptBot at your own risk.
      p Using CryptBot v{{ version.gekko }} and CryptBot UI v{{ version.ui }}.
</template>

<script>
const gekkoPackage = require('../../../../../package.json');
const uiPackage = require('../../../package.json');

export default {
  data: () => {
    return {
      version: {
        gekko: gekkoPackage.version,
        ui: uiPackage.version
      }
    }
  }
}
</script>
