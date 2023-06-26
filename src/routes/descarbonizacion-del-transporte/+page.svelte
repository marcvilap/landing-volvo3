<script lang="ts">
	import transporte01 from '$lib/assets/images/transporte01.jpg'
	import transporte02 from '$lib/assets/images/transporte02.jpg'
	import transporte03 from '$lib/assets/images/transporte03.jpg'
	import transporte04 from '$lib/assets/images/transporte04.jpg'
	import transporte05 from '$lib/assets/images/transporte05.jpg'
	import transporte06 from '$lib/assets/images/transporte06.jpg'
	import transporte07 from '$lib/assets/images/transporte07.jpg'
	import transporte08 from '$lib/assets/images/transporte08.jpg'
	import transporte09 from '$lib/assets/images/transporte09.jpg'
	import transporte10 from '$lib/assets/images/transporte10.jpg'
	import transporte11 from '$lib/assets/images/transporte11.jpg'
	import circle02 from '$lib/assets/images/circle02.svg'
	import Intersection from '$lib/components/Intersection.svelte'
	import BlockHero from '$lib/components/BlockHero.svelte'
	import BlockTextBanner from '$lib/components/BlockTextBanner.svelte'
	import BlockCircle from '$lib/components/BlockCircle.svelte'
	import BlockNav from '$lib/components/BlockNav.svelte'
	let intersection01 = false
	let intersection02 = false
	let intersection03 = false
	let intersection04 = false
	let intersection05 = false
	let intersection06 = false
	let intersection07 = false
	let intersection08 = false
	let intersection09 = false
</script>

<svelte:head>
	<style>
		body {
			background: #f8ebc0;
		}
	</style>
</svelte:head>

<main class="overflow-hidden">
	<BlockHero
		image={transporte01}
		text1="Descarbonización del transporte"
		text2="¿Qué tiene que ver un embalse o la arena con crear un coche 100% neutro en emisiones?"
		text3=""
		text4="La emergencia climática ha empujado a gobiernos y empresas a apostar por la innovación tecnológica para encontrar alternativas que permitan reducir la huella de carbono hasta llegar al objetivo de neutralidad de CO2 en 2050. Y el transporte es uno de los sectores que tiene que realizar un mayor ajuste para cumplir con esos objetivos."
	/>

	<div class="py-24">
		<Intersection bind:intersecting={intersection01} class="container">
			<div
				class="prose mx-auto max-w-xl transition duration-1000"
				class:opacity-0={!intersection01}
				class:translate-y-24={!intersection01}
			>
				<p>
					En 2018, el tráfico por carretera significaba el 26% de las emisiones de dióxido de carbono en la Unión
					Europea, una subida de diez puntos respecto al 16% de 1990. Por ello, los fabricantes de automóviles, como
					<strong>Volvo Cars</strong>, se han lanzado a una carrera para
					<a target="_blank" href="https://link.com">democratizar el vehículo eléctrico</a> y otras formas de movilidad sostenible.
				</p>
				<p>
					Y aunque pueda parecer que la solución pasa exclusivamente por electrificar el parque automóvil, el problema
					va más allá.
				</p>
			</div>
		</Intersection>
	</div>

	<BlockTextBanner
		image={transporte02}
		text="Los fabricantes de automóviles, como Volvo Cars, se han lanzado a una carrera para democratizar el vehículo eléctrico y otras formas de movilidad sostenible"
	/>

	<div class=" py-24">
		<div class="container">
			<Intersection bind:intersecting={intersection02} class="mb-24">
				<div
					class="mx-auto max-w-xl transition duration-1000"
					class:opacity-0={!intersection02}
					class:translate-y-24={!intersection02}
				>
					<p class="mb-4">
						Tanto el proceso productivo como la generación de la energía que alimenta dichos vehículos pueden formar
						parte del problema si se emplean fuentes de origen fósil. Es en este punto en el que la <strong
							>innovación llega para jugar un papel esencial, y Volvo Cars lo sabe</strong
						>: proveer la energía limpia suficiente que no solo mueva a los coches del mañana sino que también impulse
						su fabricación. Porque la sostenibilidad es tan importante como el costo y la calidad.
					</p>
					<p>
						A continuación, vemos solo algunos ejemplos de cómo <strong
							>tecnologías innovadoras están ayudando a descarbonizar la economía</strong
						>, ya sea a corto o a medio plazo.
					</p>
				</div>
			</Intersection>

			<Intersection bind:intersecting={intersection03} class="mb-24 grid gap-y-8 lg:grid-cols-2">
				<div
					class="transition duration-1000 lg:pr-24"
					class:opacity-0={!intersection03}
					class:-translate-x-24={!intersection03}
				>
					<div>
						<img
							class="relative z-10 -mb-[40%] w-full px-[14%]"
							src={transporte03}
							loading="lazy"
							decoding="async"
							alt=""
						/>
						<img class="w-full" src={transporte04} loading="lazy" decoding="async" alt="" />
					</div>
				</div>
				<div
					class="relative transition duration-1000"
					class:opacity-0={!intersection03}
					class:translate-x-24={!intersection03}
				>
					<span class="text-7xl font-bold text-[#07AAA2] md:text-[15rem] lg:absolute lg:-left-32 lg:-top-10">1</span>
					<h2 class="mb-4 font-display text-3xl md:text-4xl">Utilizar la arena para almacenar energía</h2>
					<p class="mb-4">
						Uno de los problemas a los que se enfrentan las energías renovables está relacionado con el almacenamiento
						de la energía generada para no malgastar la producción que se da cuando el viento sopla más fuerte de lo
						normal o las placas fotovoltaicas trabajan a pleno rendimiento en verano.
					</p>
					<p>
						Las baterías todavía siguen siendo una tecnología costosa, y que ha mostrado algunos problemas de
						eficiencia, pero la compañía finlandesa Polar Night Energy cree haber dado con <strong
							>una solución para almacenar el calor generado</strong
						>. La tecnología de esta empresa transfiere el calor que luego se transformará en electricidad a un banco de
						arena, que puede llegar a calentarse hasta a 1000º de temperatura y donde se encuentran unos receptores de
						calor. Estos receptores son capaces de mantener la energía almacenada durante meses con pérdidas mínimas.
					</p>
				</div>
			</Intersection>

			<Intersection bind:intersecting={intersection04} class="mb-24 grid gap-y-8 lg:grid-cols-2">
				<div
					class="relative transition duration-1000 lg:mt-96"
					class:opacity-0={!intersection04}
					class:-translate-x-24={!intersection04}
				>
					<span class="text-7xl font-bold text-[#07AAA2] md:text-[15rem] lg:absolute lg:-left-16 lg:-top-10">2</span>
					<div class="lg:translate-x-24">
						<h2 class="mb-4 font-display text-3xl md:text-4xl">Placas solares que flotan en el agua</h2>
						<p class="mb-4">
							A diferencia de los molinos de viento, las placas solares necesitan espacio. Mucho espacio. Y aunque en
							países como España con grandes zonas despobladas no debería ser un problema, si puede suponer una pega en
							áreas donde se pueda necesitar ese suelo para fines agrícolas.
						</p>
						<p class="mb-4">
							Ya existen alternativas que proponen construir placas solares encima de infraestructuras cubiertas por
							agua (desde acueductos hasta canales o embalses) de manera que se logran varios beneficios a la vez: los
							paneles proporcionan sombra y evitan que el agua se evapore, esta enfría los paneles ayudando a una mayor
							eficiencia energética y se libera espacio que se puede dedicar a la agricultura.
						</p>
						<p>
							En España ya existen algunos ejemplos de esta tecnología, como en la Comunidad Valenciana, y en Portugal <strong
								>se inauguró en 2022 la mayor planta europea fotovoltaica sobre un embalse</strong
							>. Esta medida, además, aprovecha la conexión eléctrica de la central situada a escasos metros y que estas
							plantas no utilizan de manera constante.
						</p>
					</div>
				</div>
				<div
					class="transition duration-1000 lg:pl-24"
					class:opacity-0={!intersection04}
					class:translate-x-24={!intersection04}
				>
					<img class="relative -ml-[40%] w-full" src={transporte05} loading="lazy" decoding="async" alt="" />
					<div class="-mt-[20%] pl-[20%]">
						<img class="w-full" src={transporte06} loading="lazy" decoding="async" alt="" />
						<p class="mt-4 text-sm">
							Paneles solares fotovoltaicos instalados por EDP flotan sobre la laguna artificial del embalse del
							Alqueva, en el río Guadiana, en Portugal. (Vía El País)
						</p>
					</div>
				</div>
			</Intersection>
			<Intersection bind:intersecting={intersection05} class="grid gap-y-8 lg:grid-cols-2">
				<div
					class="transition duration-1000 lg:pr-24"
					class:opacity-0={!intersection05}
					class:-translate-x-24={!intersection05}
				>
					<img class="w-full pr-[20%]" src={transporte07} loading="lazy" decoding="async" alt="" />
					<img class="-mt-[20%] w-full pl-[20%]" src={transporte08} loading="lazy" decoding="async" alt="" />
				</div>
				<div
					class="relative transition duration-1000"
					class:opacity-0={!intersection05}
					class:translate-x-24={!intersection05}
				>
					<span class="text-7xl font-bold text-[#07AAA2] md:text-[15rem] lg:absolute lg:-left-40 lg:-top-10">3</span>
					<h2 class="mb-4 font-display text-3xl md:text-4xl">Hidrógeno limpio para impulsar la industria</h2>
					<p class="mb-4">
						Uno de los grandes retos a los que se enfrenta el planeta para abastecer la producción industrial es la
						generación de grandes volúmenes de energía de origen limpio. La Unión Europea estima que la <strong
							>electricidad será la principal fuente de energía en 2050</strong
						> con una cuota de mercado superior al 50% (respecto al 22% que tenía en 2015). Esto implica que es necesario
						dar con una alternativa sostenible para cumplir con los objetivos de neutralidad de carbono de cara a mediados
						del siglo XXI.
					</p>
					<p>
						Desde Volvo Cars, lo tienen claro: es necesario pasarse a la <a
							class="text-[#07AAA2] underline"
							href="https://link.com">economía circular</a
						>, y para ello hay que actuar ya. La circularidad es buena tanto para el planeta como para el negocio,
						comenzando a plantear cómo se pueden reducir las emisiones en
						<strong>2,5 millones de toneladas mediante iniciativas circulares.</strong>
					</p>
				</div>
			</Intersection>
		</div>
	</div>

	<div class="bg-white py-24">
		<Intersection bind:intersecting={intersection06} class="container grid items-center gap-8 gap-x-24 lg:grid-cols-2">
			<div
				class="transition duration-1000"
				class:opacity-0={!intersection06}
				class:-translate-x-24={!intersection06}
				class:-skew-x-12={!intersection06}
				class:-skew-y-12={!intersection06}
			>
				<h3 class="mb-4 text-4xl font-bold">
					“Si queremos alcanzar nuestros objetivos, tenemos que pasarnos a la economía circular”
				</h3>
				<p class="font-bold">Anders Kärrberg, director de sostenibilidad global</p>
			</div>
			<div class="transition duration-1000" class:opacity-0={!intersection06} class:translate-x-24={!intersection06}>
				<img src={transporte09} loading="lazy" decoding="async" alt="" />
			</div>
		</Intersection>
	</div>

	<div class=" py-24">
		<div class="container">
			<Intersection bind:intersecting={intersection07}>
				<div
					class="mx-auto max-w-xl text-center transition duration-1000"
					class:opacity-0={!intersection07}
					class:translate-y-24={!intersection07}
				>
					<p>
						El hidrógeno que se utiliza en la actualidad se extrae del gas natural, el carbón o de la biomasa, con una
						huella de carbono notable. Pero es posible producir hidrógeno a partir de un elemento tan abundante como el
						agua. Mediante electrólisis, que también se debe producir con energías renovables, se pueden separar las
						moléculas de hidrógeno de las de oxígeno presentes en el agua. Este proceso <a
							class="text-[#07AAA2] underline"
							target="_blank"
							href="https://link.com">abriría la puerta a una forma de energía limpia</a
						> y para la que, en España, ya tenemos proyectos aprobados para construir gasoductos que puedan transportar este
						gas a todo el continente europeo.
					</p>
				</div>
			</Intersection>
			<div class="pb-24" />
			<BlockCircle image={circle02} />
		</div>
	</div>

	<div class="relative flex min-h-screen items-center bg-gray-800 py-24 text-white">
		<img
			class="absolute left-0 top-0 h-full w-full object-cover"
			src={transporte10}
			loading="lazy"
			decoding="async"
			alt=""
		/>
		<Intersection bind:intersecting={intersection08} class="container relative">
			<div
				class="max-w-xs transition duration-1000"
				class:opacity-0={!intersection08}
				class:-translate-x-24={!intersection08}
			>
				<p class="mb-4">
					El sector de la automoción es uno en los que mejor se puede observar la importancia de la innovación en la
					producción energética. No se trata solo de que los vehículos que circulan por las carreteras no contaminen,
					sino de que tanto el proceso de manufactura como sus recargas estén <strong
						>alimentadas por electricidad verde</strong
					>.
				</p>
				<p>
					Un informe de Volvo Cars sobre la <a class="text-[#07AAA2] underline" href="https://link.com"
						>Evaluación del Ciclo de Vida del C40 Recharge</a
					> ha demostrado que la huella de carbono del vehículo durante todos sus años de uso es de 27 toneladas de CO2 siempre
					que se recarga con energías alternativas. El mismo modelo, con motor de combustión, emite 59 toneladas. Pero existe
					otro dato significativo: las 27 toneladas de un eléctrico aumentan hasta 50 si el vehículo se recarga con electricidad
					que proviene de combustibles fósiles.
				</p>
			</div>
		</Intersection>
	</div>

	<div class="relative flex min-h-screen items-center py-24 text-center text-white">
		<img
			class="absolute left-0 top-0 h-full w-full object-cover"
			src={transporte11}
			loading="lazy"
			decoding="async"
			alt=""
		/>
		<Intersection bind:intersecting={intersection09} class="container relative">
			<p
				class="mx-auto max-w-xl transition duration-1000"
				class:opacity-0={!intersection09}
				class:translate-y-24={!intersection09}
			>
				La innovación no solo es necesaria en la carretera sino en toda la cadena productiva. Desde las factorías hasta
				las fuentes de energía, la única manera de alcanzar un futuro libre de emisiones de CO2 es actuando sobre todo
				el ciclo de fabricación. Y para acelerar el crecimiento sostenible, Volvo Cars abrirá una nueva fábrica de
				vehículos eléctricos en Eslovaquia, un paso fundamental para el camino hacia la electrificación total para 2030.
			</p>
		</Intersection>
	</div>

	<BlockNav />
</main>
