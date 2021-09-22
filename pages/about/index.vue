<template>
	<div class="test">
         <NuxtLink to="/">Home page</NuxtLink>
    </div>
</template>

<script>
export default {
	transition: 'page',
};
</script>

<style lang="scss" scoped>
.test {
	width: 400px;
	height: 400px;
	background-color: aqua;
}
</style>
