<template>
	<section class="profile-skills">
		<profile-skill-item></profile-skill-item>
		<profile-skill-item></profile-skill-item>
		<profile-skill-item></profile-skill-item>
	</section>
</template>

<script>

import ProfileSkillItem from './ProfileSkillItem';

export default {
	name: 'resume-skills',
	components: {
		ProfileSkillItem,
	},
};
</script>

<style lang="scss" scoped>
.skills {
	border: 1px solid red;
}
</style>


