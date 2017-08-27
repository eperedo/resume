<template>
	<section class="profile-contact">
		<div class="profile-contact-item">
			<a class="btn btn-icon" href="#" title="call me anything, Just kidding.">
				<img src="/static/img/svg/phone-icon.svg" alt="phone" width="18" height="18">
			</a>
			<p class="contact-item-value">966-568-536</p>
		</div>
		<div class="profile-contact-item">
			<a class="btn btn-icon" href="mailto:jrperedo@gmail.com" title="call me anything, Just kidding.">
				<img src="/static/img/svg/email-icon.svg" alt="email" width="18" height="18">
			</a>
			<p class="contact-item-value">
				<a href="mailto:jrperedo@gmail.com">jrperedo@gmail.com</a>
			</p>
		</div>
		<div class="profile-contact-item">
			<a class="btn btn-icon" href="https://github.com/eperedo" target="_blank" title="check my open source repos">
				<img src="/static/img/svg/link-icon.svg" alt="github link" width="18" height="18">
			</a>
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
.btn {
	background: #256FE4;
	box-shadow: 0 2px 8px 0 rgba(0, 0, 0, 0.30);
}

.btn-icon {
	border-radius: 50%;
	height: 48px;
	position: relative;
	width: 48px;
	margin-left: 100px;

	img {
		position: absolute;
		right: 32%;
		top: 32%;
	}
}

.profile-contact {
	align-items: center;
	display: flex;
	flex-direction: column;
	margin-top: 50px;

	.profile-contact-item {
		display: flex;
		width: 100%;
	}

	.contact-item-value {
		font-size: map-get($sizes, medium);
		margin-left: 15px;
	}
}
</style>


