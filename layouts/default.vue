<template>
	<div>
		<div id="drag-space"></div>
		<nuxt/>
	</div>
</template>

<style>
#drag-space {
	-webkit-app-region: drag;
	height: 20px;
	width: 100%;
}
</style>
