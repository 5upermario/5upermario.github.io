<template>
	<v-timeline>
		<v-timeline-item large v-for="(experience, index) in experiences" :key="index" color="red lighten-2">
			<template v-slot:opposite>
				{{ experience.from }} - {{ experience.to }}
			</template>

			<v-card class="elevation-2">
				<v-card-title class="headline">{{ experience.company }}</v-card-title>
				<v-card-title>{{ experience.position }}</v-card-title>

				<v-card-text>
					{{ experience.description }}
				</v-card-text>
			</v-card>
		</v-timeline-item>
	</v-timeline>
</template>

<script>
export default {
	data() {
		return {
			experiences: [
				{company: 'SalesAutopilot Kft.', position: 'PHP Full Stack webfejlesztő', from: '2018. 01.', to: 'jelenleg is', description: 'A webes szoftver továbbfejlesztése, unit tesztek írása, apróbb feladatok elvégzése a szoftverhez kapcsolódóan. Felhasznált technológiák: Docker, PHP, MySql, Smarty, Jquery, PDO'},
				{company: 'NNG Kft.',            position: 'UI Developer',                from: '2017. 11.', to: '2018. 01.',   description: 'Navigációs szoftver megjelenésének kivitelezése'},
				{company: 'Leopoly Kft.',        position: 'PHP Full Stack webfejlesztő', from: '2015. 08.', to: '2017. 10.',   description: 'Feladatok: Külső rendszerek integrálása többnyire REST API segítségével, 3D-s motorhoz GUI tervezés és kivitelezés webre. Általános backend feladatok, pl. user kezelés, MVC, Általános frontend feladatok, pl. landing page megvalósítás. Felhasznált keretrendszerek: Bootstrap, Jquery, Céges fejlesztésű PHP keretrendszer'},
				{company: 'Kitchen Budapest',    position: 'PHP webfejlesztő',            from: '2015. 03.', to: '2015. 05.',   description: 'Wordpress alapú weboldal készítése'},
				{company: 'everda.hu',           position: 'PHP webfejlesztő',            from: '2014. 11.', to: '2015. 01.',   description: 'Wordpress bővítmény készítése php nyelven'},
			]
		}
	}
}
</script>
