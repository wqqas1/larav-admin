<template>
  <card :title="$t('home')">
	{{ $t('you_are_logged_in') }}
  </card>
</template>

<script>
export default {
  	middleware: 'auth',
	layout: 'basic',
  	metaInfo () {
		return { title: this.$t('home') }
  	}
};
</script>
