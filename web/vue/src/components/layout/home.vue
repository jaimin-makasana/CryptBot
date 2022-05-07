<template lang='pug'>
  section.contain.grd-row
    .grd-row-col-3-6(v-html='left')
    .grd-row-col-3-6.txt--center
      p
</template>

<script>
import marked from '../../tools/marked';

const left = marked(`

## CryptBot

CryptBot is a Bitcoin trading bot and backtesting platform that
connects to popular Bitcoin exchanges. It is written in javascript
and runs on nodejs.


*CryptBot is 100% free (open source), So give it a try now.*

`);

export default {
  data: () => {
    return {
      left
    }
  }
}
</script>
