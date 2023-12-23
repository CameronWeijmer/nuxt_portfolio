<template>
    <div>

        <div>
            <Landing title="meine services" desc1="Entdecken Sie eine breite Palette an Web-Services unten"
                desc2="aufgelistet: Design, Hosting, IT - Support und mehr." :isButton="false" />
        </div>

        <Heading title="Webdesign für Ihren Erfolg"
            text="Entdecken Sie meine individuellen Web-Dienstleistungen, um Ihre digitale Reichweite zu stärken und Ihr Publikum zu begeistern." />

        <div>
            <ServiceCards title="Webseiten-Design und Entwicklung" description="Ich unterstütze Sie von der ersten Idee bis zur fertigen Webseite, 
            mit einem ansprechenden Design und reibungsloser technischer Umsetzung. Das Ergebnis 
            ist eine beeindruckende Webseite, die gut aussieht und einwandfrei funktioniert."
                desc1="Präzises Webdesign" desc2="Technische Expertise" desc3="Langfristige Unterstützung"
                desc4="Anpassung an Ihre Ideen" payment="Preis auf Anfrage" heading="Einmal zahlen, immer besitzen." />

            <ServiceCards title="IT-Support und Dienstleistungen"
                description="Ich stehe Ihnen zur Verfügung, um sämtliche IT-Herausforderungen zu bewältigen. Egal, ob Ihr Drucker streikt, Ihr PC Probleme bereitet oder Sie allgemeine IT-Beratung benötigen."
                desc1="Computerpflege" desc2="Problembehebung und Support" desc3="Netzwerkmanagement" desc4="Datensicherung"
                payment="80" heading="IT-Support pro Stunde" currency="CHF" />
        </div>
    </div>
</template>

<script setup>
definePageMeta({
    layout: "navigation"
})

</script>

<style scoped></style>