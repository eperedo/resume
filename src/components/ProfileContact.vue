<template>
	<section class="profile-contact">
		<div class="profile-contact-item">
			<i>phone icon</i>
			<p class="contact-item-value">966-568-536</p>
		</div>
		<div class="profile-contact-item">
			<i>mail icon</i>
			<p class="contact-item-value">
				<a href="mailto:jrperedo@gmail.com">jrperedo@gmail.com</a>
			</p>
		</div>
		<div class="profile-contact-item">
			<i>github icon</i>
			<p class="contact-item-value">
				<a href="https://github.com/eperedo">github/eperedo</a>
			</p>
		</div>
	</section>
</template>

<script>
export default {
	name: 'profile-contact',
};
</script>

<style lang="scss" scoped>
.profile-contact {

	.profile-contact-item {
		display: flex;
	}

	.contact-item.value {
		font-size: map-get($sizes, regular);
	}
}
</style>


