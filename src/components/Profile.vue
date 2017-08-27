<template>
	<section class="profile">
		<profile-avatar></profile-avatar>
		<profile-contact></profile-contact>
		<profile-skills></profile-skills>
	</section>
</template>

<script>

import ProfileAvatar from './ProfileAvatar';
import ProfileContact from './ProfileContact';
import ProfileSkills from './ProfileSkills';

export default {
	name: 'resume-profile',
	components: {
		ProfileAvatar,
		ProfileContact,
		ProfileSkills,
	},
};
</script>

<style lang="scss" scoped>
.profile {
	background: map-get($colors, blue-sky);
	border: 1px solid red;
	box-shadow: 0 2px 8px 0 map-get($colors, shadow-black);
}
</style>


