<script>
export default {
    data() {
        return {
            
        };
    },
    methods: {
        
    }
}
</script>

<template>
    <section id="section-1">
        <div class="row align-items-center">
            <div class="col-md-4 col-sm-12 px-5">
                <div class="mb-5">
                    <h3>Lunga durata della batteria</h3>

                    <p>
                        Goditi ore di assistenza continua nella risoluzione dei bug grazie alla lunga durata della "batteria" (ovvero, la tua pazienza) della paperella di gomma.
                    </p>
               </div>

                <div class="mb-5">
                    <h3>Compatibilità universale</h3>
                    
                    <p>
                        Funziona con tutti i linguaggi di programmazione e sistemi operativi, la paperella di gomma è l'unico strumento di debugging che non necessita di aggiornamenti.
                    </p>
               </div>

               <div>
                    <h3>Design Elegante</h3>
                    
                    <p>
                        Mostra con orgoglio il design elegante e raffinato della tua paperelladi gomma, disponibile in vari colori per abbinarsi al tuo stile di programmatore.
                    </p>
               </div>
            </div>

            <div class="col-md-4 col-sm-12">
                <div class="img-invisible w-75 mx-auto py-5">
                    <img class="img-fluid" src="../assets/imgs/invisible.png" alt="invisible">
                </div>
            </div>

            <div class="col-md-4 col-sm-12 px-5">
                <div class="mb-5">
                    <h3>Resistenza agli spruzzi</h3>

                    <p>
                        Perfetta per resistere ai piccoli incidenti con caffè e bevande, la tua paperella di gomma non teme schizzi, mantenendoti sempre pronto per il debugging.
                    </p>
               </div>

                <div class="mb-5">
                    <h3>Portabilità</h3>
                    
                    <p>
                        Leggera e facile da trasportare, la paperella di gomma può essere il tuo compagno di lavoro ovunque tu vada. Portala con te per un supporto costante.
                    </p>
               </div>

               <div>
                    <h3>Promemoria Anti-Stress</h3>
                    
                    <p>
                        Quando lo stress del codice diventa troppo, spremi la tua paperella di gomma per un rapido sollievo anti-stress, senza bisogno di software complicati.
                    </p>
               </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    // importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    // GENERAL
    .row {
        padding: 80px 50px;
        text-align: center;
    }

    // mediaquery 
    @media (max-width: 991px) {
        #section-1 {
            padding-top: 600px;
        }
    }
</style>
