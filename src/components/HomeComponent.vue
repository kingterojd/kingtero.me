<template>
	<div>
		<v-img
	      	src="../assets/background_index.jpg"
	      	class="grey lighten-2"
	      	max-width="100%"
	      	max-height="100vh">
	    </v-img>
	    <v-container grid-list-md>
			<v-layout row wrap>
				<v-flex xs12>
					<h2 class="display-2 py-8">¿QUIÉN SOY YO?</h2>
				</v-flex>
				<v-flex xs12 sm7 md7 lg7 class="bg-img">
					<v-layout row wrap>
					  	<v-flex xs12 sm7 md7 lg7 >
					  		<p class="pr-8 text-justify">Soy desarrollador front-end especializado en desarrollo Vue y Veutify. Consectetur adipisicing elit, sed do eiusmod tempor. Quisque viverra quam urna, ac commodo augue convallis et. En vel nisl imperdiet, cursus elit ac, effitur sem. Nam liber tempor cum soluta nobis eleifend opción congue nihil imperdiet doming id quom placerat facer possim assum.</p>
					  	</v-flex>
					  	<v-flex xs12 sm5 md5 lg5 class="px-8">
					  		<v-simple-table class="transparent">
							    <template v-slot:default>
							      <tbody>
							        <tr v-for="(item,index) in information" :key="index">
							          <td class="text-left">{{ item.text }}</td>
							          <td class="text-right">{{ item.value }}</td>
							        </tr>
							      </tbody>
							    </template>
							  </v-simple-table>
						</v-flex>
					</v-layout>
				</v-flex>
				<v-flex xs12 sm5 md5 lg5 class="text-right">
					<h2 class="display-1">DESARROLLADOR FULL STACK</h2>
					<p class="headline">JESÚS QUINTERO</p>
				</v-flex>
			</v-layout>
	    </v-container>
	    <v-container grid-list-md>
			<v-layout row wrap>
				<v-flex xs12>
					<h2 class="display-2 py-8">What I can do for you.</h2>
				</v-flex>
				<v-flex xs12 sm12 md6>
					<v-expansion-panels class="mb-6">
						<v-expansion-panel v-for="(item,i) in 4" :key="i">
					        <v-expansion-panel-header disable-icon-rotate>
					          <v-subheader class="subheading font-weight-bold">Item</v-subheader>
					          <template v-slot:actions>
					            <v-icon color="white">mdi-check</v-icon>
					          </template>
					        </v-expansion-panel-header>
					        <v-expansion-panel-content>
					          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
					        </v-expansion-panel-content>
					    </v-expansion-panel>
					</v-expansion-panels>
				</v-flex>
				<v-flex xs12 sm12 md6>
					
				</v-flex>
			</v-layout>
	    </v-container>
	    <v-container grid-list-md>
			<v-layout row wrap>
				<v-flex xs12>
					<h2 class="display-2 py-8">Where I've been</h2>
				</v-flex>
				<v-flex xs12 class="px-4">
					<v-timeline>
				      	<v-timeline-item
					        v-for="n in 3"
					        :key="n"
					        icon="mdi-xml"
					        icon-color="white"
					        color="cyan">
					        <span slot="opposite">Tus eu perfecto</span>
					        <v-card class="elevation-2">
					          <v-card-title class="headline">Lorem ipsum</v-card-title>
					          <v-card-text>
					            Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.
					          </v-card-text>
					        </v-card>
				      	</v-timeline-item>
				    </v-timeline>
				</v-flex>
			</v-layout>
	    </v-container>
	    <v-container grid-list-md>
			<v-layout row wrap>
				<v-flex xs12 sm12 md6>
					<h2 class="display-2 py-8">Lo que sé</h2>
				</v-flex>
				<v-flex xs12 sm12 md6 class="text-right">
					<div class="subheading font-italic font-weight-medium">Some text..</div>
					<v-btn color="cyan">
						DESCARGAR CV
					</v-btn>
				</v-flex>
				<v-flex xs12 sm12 md6 class="px-12">
					<v-subheader class="display-1 pl-0">Mi educación</v-subheader>
					<v-alert
					v-for="n in 3"
				        :key="n"
					    color="cyan"
					    border="left"
					    elevation="2"
					    colored-border
					    icon="mdi-twitter">
					    <div>State University</div>
					    <div class="text-right title cyan--text">Bachelor of Computer Science</div>
					    <div class="text-right">Computer Sciences</div>
					    <div class="text-right">2013- 2017</div>
					</v-alert>
				</v-flex>
				<v-flex xs12 sm12 md6 class="px-12">
					<v-subheader class="display-1 pl-0">Mis habilidades</v-subheader>
					<div v-for="n in 3":key="n">
						<v-subheader>PROGRAMMING</v-subheader>
						<v-layout row wrap v-for="n in 3" :key="n">
						  	<v-flex xs12 sm12 md2 class="pt-4">
								<span class="pl-4">text</span>
							</v-flex>
							<v-flex xs12 sm12 md6>
								<v-rating
							      :value="4"
							      :length="5"
							      empty-icon="mdi-circle-outline"
							      full-icon="mdi-check-circle"
							      half-icon="mdi-heart-half-full"
							      :half-increments="false"
							      :hover="true"
							      :readonly="true"
							      :size="30"
							      color="cyan"
							      background-color="white">
							    </v-rating>
							</v-flex>
						</v-layout>
					</div>
				</v-flex>
			</v-layout>
	    </v-container>
	    <v-container>
			<v-layout row wrap>
				<v-flex xs12>
					<h2 class="display-2 py-8">Lo qué he hecho</h2>
				</v-flex>
				<v-flex xs12>
					<v-carousel :show-arrows="false">
					    <v-carousel-item v-for="(item,i) in 3" :key="i">
							<div>text</div>
					    </v-carousel-item>
					</v-carousel>
				</v-flex>
			</v-layout>
	    </v-container>
	    <v-container grid-list-lg>
			<v-layout row wrap>
				<v-flex xs12>
					<h2 class="display-2 py-8">Lo que dicen mis clientes.</h2>
				</v-flex>
				<v-flex xs12 sm12 md4
					v-for="(item,i) in 6" :key="i">
					<v-card
						flat
					    color="transparent"
					    dark>
					    <v-card-title>
						    <v-icon
						    	color="cyan"
						        large
						        left>
						        mdi-twitter
						    </v-icon>
					    </v-card-title>

					    <v-card-text class="subheading font-weight-bold">
					      	"Turns out semicolon-less style is easier and safer in TS because most gotcha edge cases are type invalid as well."
					    </v-card-text>
				    	<div class=" text-right">
				    		<span>Jesús Quintero</span>
				    		<v-avatar
              					size="36px">
					    		<img
						            src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light">							    
						    </v-avatar>
				    	</div>
					  </v-card>
				</v-flex>
			</v-layout>
	    </v-container>
	</div>
</template>

<script>
	export default{
		data(){
			return{
				information: [
		          	{
			            text: 'UBICACIÓN',
			            value: 'Lima, Perú.',
		          	},
		          	{
			            text: 'EMAIL',
			            value: 'kingtero.dev@gmail.com',
		          	},
		          	{
			            text: 'TELÉFONO',
			            value: '(51) 927 253 716',
		          	},
		        ],
			}
		}
	}
</script>

<style scoped>
	.v-responsive{
		height: 100vh !important;
	}
</style>