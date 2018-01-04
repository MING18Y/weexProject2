<template>
	<div class="hello1">
		<image :src="logoUrl" class="logo"></image>
		<text class="title">Hello {{target}}</text>
	</div>
	
</template>

<script>
	
	export default {
		
		data:{
			logoUrl: 'https://www.baidu.com/img/bd_logo1.png',
			target:"world 1.vue"
			
		}
		
	}
	
</script>

<style>
	.wrapper { align-items: center; margin-top: 120px; }
	.title { padding-top:40px; padding-bottom: 40px; font-size: 48px; }
	.logo { width: 300px; height: 150px; }
	
</style>