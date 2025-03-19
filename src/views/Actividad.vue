<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <Actividad :cuestionario="cuestionario"/>
  
  </template>

<script>
import Actividad from 'ecored-pkg-fliz/plugin/components/actividad/Actividad.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    Actividad,
  },
  data: () => ({
    cuestionario: {
      tema: 'Ecología y legislación ambiental.',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> Validar el conocimiento adquirido sobre la legislación vigente aplicada a la pedagogía.',
      barajarPreguntas: true,
      preguntas: [
        {
          id: 1,
          texto: '¿Qué es un recurso natural?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Un material artificial creado por humanos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Un recurso que no se puede reutilizar.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Un elemento de la naturaleza utilizado por el hombre.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Un recurso que solo se encuentra en ecosistemas acuáticos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 2,
          texto:
            '¿Cuál es el propósito de la conservación de los recursos naturales?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Aumentar el turismo.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Preservar los recursos para futuras generaciones.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Maximizar su explotación económica.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Eliminar especies invasoras.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 3,
          texto: '¿Qué es la biodiversidad?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'La variedad de climas en una región.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'La variedad de especies en un ecosistema.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'La mezcla de culturas en un país.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'La cantidad de plantas en un área urbana.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 4,
          texto: '¿Cuál de las siguientes es una práctica sostenible?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'La tala masiva de árboles.', esCorrecta: false },
            {
              id: 'b',
              texto: 'La caza de especies en peligro de extinción.',
              esCorrecta: false,
            },
            { id: 'c', texto: 'La agricultura de rotación.', esCorrecta: true },
            {
              id: 'd',
              texto: 'El uso excesivo de pesticidas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 5,
          texto: '¿Qué es el cambio climático?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Una modificación temporal del clima.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Un fenómeno natural sin intervención humana.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Alteraciones en el clima debido a actividades humanas.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Un cambio de temperatura local.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 6,
          texto: '¿Cuál es un aspecto fundamental del turismo sostenible?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'La explotación intensiva de recursos naturales.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'La participación de la comunidad local.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'La construcción de grandes complejos hoteleros.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'La promoción de destinos lejanos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 7,
          texto: '¿Cuál de los siguientes es un ejemplo de turismo cultural?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Visitar un parque de diversiones.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Hacer senderismo en una montaña.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Explorar sitios arqueológicos.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Nadar en una playa.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 8,
          texto: '¿Qué es el patrimonio natural?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Un conjunto de sitios históricos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'La biodiversidad y paisajes de una región.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Solo los parques nacionales.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Monumentos arquitectónicos de una región.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 9,
          texto:
            '¿Cuál de las siguientes es una característica del turismo ecológico?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Favorece las zonas urbanas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Evita la interacción con la naturaleza.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Promueve la conservación ambiental.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Incrementa la urbanización.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 10,
          texto: '¿Qué establece el Decreto Ley 2811 de 1974 en Colombia?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Reglas para la minería', esCorrecta: false },
            {
              id: 'b',
              texto: 'Normas de protección de recursos naturales.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Códigos de construcción.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Normas de comercio exterior.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 11,
          texto: '¿Cuál es la función de un parque nacional?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Facilitar la expansión urbana.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Preservar el medio ambiente y la biodiversidad.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Aumentar las áreas para construcción.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Promover la agricultura intensiva.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 12,
          texto: '¿Qué es un área protegida?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Un espacio designado para la explotación minera.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Una región con restricciones para preservar la naturaleza.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Una zona para el turismo masivo.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Una región urbana con leyes ambientales especiales.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 13,
          texto: '¿Cuál es el principal objetivo de la legislación ambiental?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Desarrollar la infraestructura urbana.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Establecer normas de conservación y protección ambiental.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Aumentar la industria turística.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Regular la caza y pesca exclusivamente.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 14,
          texto: '¿Qué filósofo es conocido como el “padre de la ecología”?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Aristóteles',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Alexander von Humboldt',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Sócrates',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Descartes',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 15,
          texto:
            '¿Cuál es uno de los principios de la metodología “No Deje Rastro”?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Dejar las sobras de comida en el lugar.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Minimizar el impacto en el medio ambiente.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Recolectar flora y fauna local.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Crear senderos improvisados.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 16,
          texto: '¿Qué significa “Planifica y prepárate” en “No Deje Rastro”?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Ir a la aventura sin guía',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Planear y llevar equipo adecuado para reducir el impacto ambiental.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Llevar solo comida enlatada.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Viajar en grupo numeroso.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 17,
          texto:
            '¿Cuál es la mejor práctica para los desechos en zonas naturales?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Enterrarlos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Dejarlos en un rincón del sitio.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Llevarlos de regreso para disponerlos adecuadamente.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Quemarlos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 18,
          texto:
            '¿Por qué es importante mantener los senderos en zonas naturales?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Facilita la creación de nuevos caminos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Reduce la erosión y el daño a la vegetación.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Ayuda a la reforestación.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Crea espacios de reunión.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 19,
          texto: '¿Qué significa “No Deje Rastro”?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Limpiar solo cuando sea necesario.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Minimizar la huella humana en el ambiente.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Solo dejar residuos biodegradables.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Crear refugios en áreas naturales',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 20,
          texto: '¿Qué significa "sostenibilidad" en un contexto ecológico?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Maximizar el uso de recursos para obtener beneficios.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Utilizar recursos de manera que se mantengan a largo plazo.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Priorizar el crecimiento económico.',
              esCorrecta: false,
            },
            { id: 'd', texto: 'Producir más desechos.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
