<template>
        under construction. trying to get a timeline component that i made to work, but it's being stubborn.
        <div class="card">
            <Timeline :items="items"></Timeline>
        </div>
</template>

<script>
import Timeline from '../components/Timeline.vue'
export default {
    name: 'Work',
    components: {
        Timeline
    },
    data() {
        return {
            items: [
                {
                    date: "2001",
                    description: "Moved from Japan to Singapore"
                },
                {
                    date: "2018",
                    description: "Having a crisis"
                }
            ]
        }  
    }
}
</script>

<style>
.card {
    width: 448px;
    height: 600px;
    padding: 32px;
}
  
</style>