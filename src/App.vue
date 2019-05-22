<template>
	<v-app>
		<!--v-toolbar app>
			<v-toolbar-title class="headline text-uppercase">
				<span>Vuetify</span>
				<span class="font-weight-light">MATERIAL DESIGN</span>
			</v-toolbar-title>
			<v-spacer></v-spacer>
			<v-btn
				flat
				href="https://github.com/vuetifyjs/vuetify/releases/latest"
				target="_blank"
			>
				<span class="mr-2">Latest Release</span>
			</v-btn>
		</v-toolbar-->

		<v-content>
			<v-container grid-list-lg>
				<v-layout>
					<v-flex sm9>
						<v-tabs>
							<v-tab>Szakmai tapasztalat</v-tab>
							<v-tab>Tanulmányok</v-tab>
							<v-tab>Nyelvismeret</v-tab>
							<v-tab>Egyéb</v-tab>
							<v-tab>Hobbi</v-tab>

							<v-tab-item>
								<ExperienceTimeline/>
							</v-tab-item>

							<v-tab-item>
								<StudyTimeline/>
							</v-tab-item>

							<v-tab-item>
								<v-card class="ma-3">
									<v-card-title primary-title>Angol középfok</v-card-title>

									<v-card-text>
										<p>Nyelvvizsga dátuma: 2010.12.</p>
										<p>Szóban ritkán, írásban és olvasásban napi szinten használom</p>
									</v-card-text>
								</v-card>
							</v-tab-item>

							<v-tab-item>
								<v-card class="ma-3">
									<v-card-text>
										<p>B kategóriás jogosítvány (2008)</p>
										<p>A1 kategóriás jogosítvány (2011)</p>
									</v-card-text>
								</v-card>
							</v-tab-item>

							<v-tab-item>
								<v-card class="ma-3">
									<v-card-text>
										<p>Modellezés (egytemi kurzus, Autodesk Maya szoftver).</p>
										<p>Biciklizés, motorozás.</p>
										<p>Okostelefonra applikáció fejlesztés – android, ios.</p>
										<p>IOT, Raspberry Pi (médiaszerver, digitális képkeret, robotika)</p>
										<p>Új technológiák megismerése</p>
									</v-card-text>
								</v-card>
							</v-tab-item>
						</v-tabs>
					</v-flex>

					<v-flex sm3>
						<v-card>
							<v-img src="profile.jpg"></v-img>

							<v-card-title primary-title>
								<h2>Gergely Dávid</h2>
							</v-card-title>
							<v-card-title>Végzettség: Programozó informatikus</v-card-title>
							<v-card-title>Születési hely, idő: Budapest, 1991. június 17.</v-card-title>

							<v-card-text>
								<a href="https://sourcerer.io/5upermario" target="_blank">
									<img alt="Sourcerer" height="32px" src="https://sourcerer.io/icons/logo-sharing.svg">
								</a>
							</v-card-text>

							<v-card-actions>
								<v-btn
									href="https://www.linkedin.com/in/d%C3%A1vid-gergely-23329399/"
									target="_blank"
								>LinkedIn</v-btn>

								<v-btn href="https://jsfiddle.net/user/5upermario/fiddles/" target="_blank">jsfiddle</v-btn>

								<v-btn href="https://profile.codersrank.io/user/5upermario" target="_blank">Codersrank</v-btn>
							</v-card-actions>
						</v-card>
					</v-flex>
				</v-layout>
			</v-container>
		</v-content>
	</v-app>
</template>

<script>
import ExperienceTimeline from './components/ExperienceTimeline';
import StudyTimeline from './components/StudyTimeline';

export default {
	name: 'App',
	components: {
		ExperienceTimeline,
		StudyTimeline
	},
	data() {
		return {
			//
		};
	}
};
</script>
