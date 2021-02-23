<template>
<div class="w-screen h-screen flex flex-row justify-center items-center space-x-4 ">
    <Card v-for="(l, key) of list" :key="key" :value="l"/>
</div>
</template>

<script>
import Card from "./components/Card";
export default {
    components:{ Card},
    data()
    {
        return {
            //boton: "LEER MÁS",
            list:[
                {   
                    link:'https://web.whatsapp.com/',
                    texhover:'hover:shadow-2xl',  
                    hovertxt:'hover:text-black', //este hover lo deje para el caso del hover en el boton
                    butborder:'border-green-600', //borde para el boton
                    textcolor:'text-green-600',
                    border_color:'border-green-600', //borde de la tarjeta
                    name:'WhatsApp',
                    description:'WhatsApp es una aplicación de chat para teléfonos móviles de última generación, los llamados smartphones. Sirve para enviar mensajes de texto y multimedia entre sus usuarios.',
                    image:'https://www.logo.wine/a/logo/WhatsApp/WhatsApp-GreenSquare-Logo.wine.svg'
                },
                {
                    link:'https://telegram.org/?setln=es',
                    color:'bg-blue-500',
                    texhover:'hover:shadow-2xl',
                    hovertxt:'hover:text-black', //este hover lo deje para el caso del hover en el boton
                    butborder:'border-white', //borde para el boton
                    textcolor:'text-white',
                    border_color:'border-blue-500', //borde de la tarjeta
                    name:'Telegram',
                    description:'Telegram es una plataforma de mensajería y VOIP desarrollada por Nikolái y Pável Dúrov.La aplicación está enfocada en la mensajería instantánea, el envío de varios archivos y la comunicación en masa.',
                    image:'https://www.logo.wine/a/logo/Telegram_(software)/Telegram_(software)-Classic-Logo.wine.svg'
                },
                {
                    link:'https://www.tiktok.com/',
                    texhover:'hover:shadow-2xl',
                    hovertxt:'hover:text-pink-600', //este hover lo deje para el caso del hover en el boton
                    textcolor:'text-black',
                    butborder:'border-black', //borde para el boton
                    border_color:'border-black', //borde de la tarjeta
                    name:'TikTok',
                    description:'TikTok es una aplicación de medios de iOS y Android para crear y compartir vídeos cortos. La aplicación permite a los usuarios crear vídeos musicales cortos de 3–15 segundos.',
                    image:'https://www.logo.wine/a/logo/TikTok/TikTok-Logomark%26Wordmark-Vertical-Logo.wine.svg'
                },
                {
                    link:'https://www.snapchat.com/l/es/',
                    color:'bg-yellow-300',
                    texhover:'hover:shadow-2xl',
                    hovertxt:'hover:text-white', //este hover lo deje para el caso del hover en el boton
                    textcolor:'text-black',
                    butborder:'border-black', //borde para el boton
                    border_color:'border-black', //borde de la tarjeta
                    name:'Snapchat',
                    description:'Snapchat es una aplicación de mensajería para teléfonos inteligentes con soporte multimedia de imagen, video y filtros para fotos de realidad aumentada. Su mayor característica es la mensajería.',
                    image:'https://www.logo.wine/a/logo/Snapchat/Snapchat-Logo.wine.svg'
                },
                {
                    link:'https://www.messenger.com/',
                    texhover:'hover:shadow-2xl',
                    hovertxt:'hover:text-black', //este hover lo deje para el caso del hover en el boton
                    textcolor:'text-blue-400',
                    butborder:'border-blue-400', //borde para el boton
                    border_color:'border-blue-300', //borde de la tarjeta
                    name:'Messenger',
                    description:'Facebook Messenger es una aplicación de mensajería. Originalmente desarrollada como Facebook Chat en 2008 y posteriormente lanzó la nueva aplicación en agosto de 2012.',
                    image:'https://www.logo.wine/a/logo/Facebook_Messenger/Facebook_Messenger-Logo.wine.svg'
                }
            ]
        };
    },
};
</script>