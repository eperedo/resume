<template>
	<section class="profile-skills">
		<profile-skill-item v-for="skill in skills" v-bind:key="skill.id" v-bind:skill="skill"></profile-skill-item>
	</section>
</template>

<script>

import ProfileSkillItem from './ProfileSkillItem';

function data() {
	return {
		skills: [
			{
				id: 1,
				title: 'Front-End',
				description: 'Javascript, CSS, HTML, Vue, Angular 1.x, React, SCSS, Progressive Web Apps, WebPack, Babel',
			},
			{
				id: 2,
				title: 'Back-End',
				description: 'C#, NodeJs, HapiJs, Objection, JWT',
			},
			{
				id: 3,
				title: 'Others',
				description: 'Postgres, MySql, Mongo, Redis, REST',
			},
		],
	};
}

export default {
	name: 'resume-skills',
	components: {
		ProfileSkillItem,
	},
	data,
};
</script>

<style lang="scss" scoped>
.profile-skills {
	align-items: center;
	display: flex;
	flex-direction: column;
	margin-bottom: 20%;
}
</style>


