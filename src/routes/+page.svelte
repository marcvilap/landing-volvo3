<script lang="ts">
	import ia01 from '$lib/assets/images/ia01.jpg'
	import ia02 from '$lib/assets/images/ia02.jpg'
	import ia03 from '$lib/assets/images/ia03.jpg'
	import ia04 from '$lib/assets/images/ia04.jpg'
	import ia05 from '$lib/assets/images/ia05.jpg'
	import ia06 from '$lib/assets/images/ia06.jpg'
	import ia07 from '$lib/assets/images/ia07.jpg'
	import ia08 from '$lib/assets/images/ia08.jpg'
	import ia09 from '$lib/assets/images/ia09.jpg'
	import ia10 from '$lib/assets/images/ia10.jpg'
	import ia11 from '$lib/assets/images/ia11.jpg'
	import ia12 from '$lib/assets/images/ia12.jpg'
	import ia13 from '$lib/assets/images/ia13.jpg'
	import ia14 from '$lib/assets/images/ia14.jpg'
	import ia15 from '$lib/assets/images/ia15.jpg'
	import ia16 from '$lib/assets/images/ia16.jpg'
	import circle03 from '$lib/assets/images/circle03.png'
	import Intersection from '$lib/components/Intersection.svelte'
	import BlockHero from '$lib/components/BlockHero.svelte'
	import BlockTextBanner from '$lib/components/BlockTextBanner.svelte'
	import BlockHalf from '$lib/components/BlockHalf.svelte'
	import BlockCircle from '$lib/components/BlockCircle.svelte'
	import BlockNav from '$lib/components/BlockNav.svelte'
	let intersection01 = false
	let intersection02 = false
	let intersection03 = false
	let intersection04 = false
	let intersection05 = false
	let intersection06 = false
</script>

<svelte:head>
	<style>
		body {
			background: #e0f3fd;
		}
	</style>
</svelte:head>

<main class="overflow-hidden">
	<BlockHero
		image={ia01}
		text1="Inteligencia Artificial"
		text2="¿Cómo se usa la Inteligencia Artificial en la movilidad?"
		text3="Tres tecnologías de la IA que van a salvar vidas (y a mejorarlas)"
		text4="Los avances en tecnología, especialmente en áreas como la inteligencia artificial o las redes neuronales, están redibujando el paisaje de la movilidad en los últimos años a una velocidad inusitada."
	/>

	<div class="py-24">
		<div class="container">
			<Intersection bind:intersecting={intersection01}>
				<div
					class="prose prose-capitalize mx-auto max-w-xl transition duration-1000"
					class:opacity-0={!intersection01}
					class:translate-y-24={!intersection01}
				>
					<p>
						La transición hacia el coche eléctrico acapara titulares en la actualidad, pero solo es la punta de lanza de
						una serie de innovaciones pensadas para transformar. Esto incluye no solo la experiencia a bordo de un
						coche, sino incluso los procesos de compra, la manera en que trabajan las líneas de producción o las <strong
							>aplicaciones para el transporte</strong
						>. Y
						<a target="_blank" rel="sponsored" href="https://ad.doubleclick.net/ddm/clk/561637283;371095440;j"
							>Volvo Cars</a
						> es experto en cada una de estas etapas.
					</p>
					<p>
						En la actualidad se están probando avances para poder cargar los coches de manera inalámbrica, una
						tecnología que también se utiliza de manera satisfactoria para actualizar el software que mueve a los
						vehículos.
					</p>
				</div>
			</Intersection>
			<Intersection class="mx-auto mt-24 max-w-3xl" bind:intersecting={intersection02}>
				<img
					class="w-full transition duration-1000"
					class:opacity-0={!intersection02}
					class:scale-50={!intersection02}
					src={ia02}
					loading="lazy"
					decoding="async"
					alt=""
				/>
			</Intersection>
		</div>
	</div>

	<BlockTextBanner
		image={ia03}
		text="Que un coche se parezca cada vez más a un ordenador implica que la industria del automóvil puede también <a class='underline' rel='sponsored' target='_blank' href='https://ad.doubleclick.net/ddm/clk/561626030;371095443;a'>acceder a innovaciones</a> que antes parecían reservadas al ámbito informático"
	/>

	<Intersection bind:intersecting={intersection03} class="container mt-24">
		<p
			class="mx-auto max-w-xl transition duration-1000"
			class:opacity-0={!intersection03}
			class:translate-y-24={!intersection03}
		>
			Con la inteligencia artificial en el centro de un acalorado debate acerca de sus usos, aplicaciones y límites,
			repasamos los usos que esta tecnología ofrece a la industria y <strong
				>cómo va a ayudar a moldear el sector a medio y largo plazo</strong
			>.
		</p>
	</Intersection>

	<BlockHalf
		image1={ia04}
		image2={ia05}
		title="Un diseñador virtual que genera coches <a class='underline' href='https://www.volvocars.com/es/cars/ex30-electric/interior-design/' target='_blank' rel='sponsored'>más sostenibles</a>"
		invert
	>
		<p>
			Pongámonos en el cuerpo de un fabricante de automóviles que quiere diseñar un nuevo vehículo y quiere que sus
			formas tengan un impacto en la resistencia que el coche opone al aire para, así, ahorrar combustible. En el
			pasado, un equipo de diseñadores trabajaba el tiempo que hiciera falta para visualizar y trazar nuevas ideas sobre
			el papel, <strong>un primer paso se puede agilizar gracias a una inteligencia artificial</strong> a la que se le haya
			enseñado previamente, a base de alimentarla con imágenes de automóviles ya existentes.
		</p>
		<p>
			El resultado de este proceso, que apenas puede tardar unos minutos, son una serie de propuestas sobre las que el
			equipo de diseño puede comenzar a trabajar e iterar. Añadir inteligencia artificial a esas propuestas iniciales
			permite obtener un número ingente de ideas a las que se pueden añadir ligeras variaciones sobre las formas de
			diferentes piezas (guardabarros, alerones) para producir modelos sobre los que, ahora sí, pueden trabajar los
			diseñadores.
		</p>
	</BlockHalf>

	<div class="relative flex min-h-screen items-center py-24 text-white">
		<img class="absolute left-0 top-0 h-full w-full object-cover" src={ia06} loading="lazy" decoding="async" alt="" />
		<Intersection bind:intersecting={intersection04} class="container relative">
			<p
				class="max-w-xs transition duration-1000"
				class:opacity-0={!intersection04}
				class:translate-y-24={!intersection04}
			>
				Es en este punto donde entra el <strong>factor humano</strong> para unir forma y función y lograr un resultado
				que sea atractivo a los ojos y que también sea <strong>eficiente en términos energéticos</strong>. Por el
				camino, la inteligencia artificial le ha ahorrado a la empresa un buen pellizco económico y ha liberado a los
				diseñadores de tareas repetitivas en la mesa de trabajo.
			</p>
		</Intersection>
	</div>

	<BlockHalf image1={ia07} image2={ia08} title="Coches que salvan vidas mientras te llevan por la autovía" invert>
		<p>
			La seguridad a bordo es una de las principales preocupaciones que tienen en cuenta los conductores a la hora de
			comprar un vehículo, así como el impacto ambiental. En los últimos años, <strong
				>fabricantes como Volvo Cars ofrecen <a
					target="_blank"
					rel="sponsored"
					href="https://ad.doubleclick.net/ddm/clk/561778222;371095449;r">medidas cada vez más completas</a
				> para el día a día en la carretera</strong
			>: alianzas climáticas, cámaras, sensores, LIDARs unidos a computación en la nube y herramientas de inteligencia
			artificial permiten a algunos vehículos leer lo que sucede en el asfalto en tiempo real y anticiparse a futuros
			problemas.
		</p>
	</BlockHalf>

	<BlockTextBanner
		image={ia09}
		text="<a href='https://ad.doubleclick.net/ddm/clk/561778231;371095455;o' class='underline' target='_blank' rel='sponsored'>Ya existen soluciones</a> para que un vehículo pueda tomar el control en determinadas situaciones para evitar a otro conductor que invade nuestro carril u otro que ha frenado en seco enfrente nuestro"
	/>

	<BlockHalf image1={ia10} image2={ia11}>
		<p>
			Todavía estamos lejos de la conducción autónoma total, pero ya existen en el mercado opciones que permiten ceder
			al vehículo cierto control de las operaciones. <strong
				>El uso de tecnología permite circular por autovía acorde a los límites de velocidad</strong
			>, siempre por los carriles adecuados y ejecutando las maniobras necesarias para sortear el tráfico. Y todo ello
			sin que el conductor tenga que pisar un pedal o controlar el volante aunque siempre se recomienda que con la vista
			y la atención puestas en la carretera por si es necesario tomar el control en cualquier momento.
		</p>
		<p>
			No está de más recordar que ya contamos con herramientas en la palma de nuestra mano que nos permiten calcular las
			mejores rutas en tiempo real teniendo en cuenta factores como el tráfico, posibles accidentes u obras en la
			carretera.
		</p>
	</BlockHalf>

	<BlockCircle image={circle03} />

	<BlockHalf image1={ia12} image2={ia13} title="Conducción autónoma para el sector industrial" invert>
		<p>
			Hoy en día ya disfrutamos de cierto grado de autonomía en la conducción, aunque todavía estamos lejos del nivel 5,
			ese que permitirá entregar el control al vehículo. Algunas firmas trabajan en llevar esa autonomía a sectores
			industriales, de manera que la implantación de estas tecnologías potencie la <strong
				>seguridad, <a
					class="underline"
					rel="sponsored"
					target="_blank"
					href="https://ad.doubleclick.net/ddm/clk/561633980;371095452;m">productividad</a
				> y sostenibilidad de la actividad industrial</strong
			>.
		</p>
		<p>
			Es el caso de Volvo Cars, firma cuyas soluciones se pueden implantar en tres etapas diferentes del proceso
			productivo.Una de ellas está dirigida a la extracción minera, ya que aplica conducción autónoma para transportar
			materias primas, reduce emisiones y aumenta la seguridad laboral ya que elimina el factor humano de la ecuación.
			En el sector logístico, esta tecnología pretende eliminar cuellos de botella mediante la conducción autónoma de
			camiones o la instalación de infraestructura adaptada para estas tecnologías.
		</p>
	</BlockHalf>

	<BlockTextBanner
		image={ia14}
		text="El transporte de mercancías también se beneficia de la automatización, ya que permite un transporte por carretera durante las 24 horas mientras los conductores pueden encargarse de rutas más cercanas a su hogar sin tener que conducir durante jornadas maratonianas"
	/>

	<div class="py-24">
		<Intersection bind:intersecting={intersection05} class="container grid items-center gap-y-24 md:grid-cols-2">
			<div
				class="transition duration-1000 md:pr-8 xl:pr-24"
				class:opacity-0={!intersection05}
				class:-translate-x-24={!intersection05}
			>
				<p>
					No obstante, hay que puntualizar que todas las firmas deben adaptarse a la legislación vigente de cada país,
					de la cual depende fundamentalmente el desarrollo de esta área. Desde 2022, todos los modelos que se
					encuentren equipados con los <strong>sistemas y la tecnología de nivel 3 son legales en Europa</strong>, una
					modificación que desde Naciones Unidas pretenden extender a nivel internacional.
				</p>
			</div>
			<div class="transition duration-1000" class:opacity-0={!intersection05} class:translate-x-24={!intersection05}>
				<img class="w-full" src={ia15} loading="lazy" decoding="async" alt="" />
			</div>
		</Intersection>
	</div>

	<div class="relative flex min-h-[32rem] items-center py-24 text-center text-white">
		<img class="absolute left-0 top-0 h-full w-full object-cover" src={ia16} loading="lazy" decoding="async" alt="" />
		<Intersection bind:intersecting={intersection06} class="container relative">
			<p
				class="mx-auto max-w-lg transition duration-1000"
				class:opacity-0={!intersection06}
				class:translate-y-24={!intersection06}
			>
				Inteligencia artificial, automatización de procesos, eficiencia, sostenibilidad y seguridad son algunos de los
				conceptos que van a definir muchos sectores industriales en las próximas décadas. El automóvil no es una
				excepción y la implantación actual de estas tecnologías demuestra no solo que el cambio es imparable sino que,
				además, va a tener un impacto desde el primer día.
			</p>
		</Intersection>
	</div>
	<BlockNav />
</main>
