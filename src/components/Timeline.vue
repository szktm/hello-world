<template>
    <div>
        <div class="TimelineItem" v-for="(item, index) in items" :key="index">
                <div id="date"> {{item.date}} </div>
                <!-- Length of vertical line changes based on position in array-->
                <div> 
                    <div class="firstline" v-if="index == 0"></div>
                    <div class="lastline" v-else-if="index == items.length - 1"></div>
                    <div class ="line" v-else></div>
                    <!-- If a student has dropped out, white dot is rendered -->
                    <div class ="dot"></div>
                </div>
                <div id="description"> {{item.description}} </div>
        </div>
    </div>

</template>

<script>
export default {
    name: "Timeline",
    props: {
        items: {
            type: Array,
            default: () => []
            /*
            * item: { date: Date, description: String, status: Number }
            */ 
        }
    }
    
    
}
</script>

<style>

.TimelineItem {
/* Blue Rectangle Background */
    width: 384px;
    height: 56px;
    
/*Font styling*/
    font-size: 14px;
    line-height: 20px;

/* identical to box height, or 143% */
    display: flex;
    align-items: center;

/* Font colour: Primary Dark */
    color: #2F4858; 
    }

#date {
    margin: auto;
    margin-right: 9px;
    width: 85px;
    height: 20px;
    
}
#description {
    margin-top: 8px;
    margin-bottom: 8px;
    margin-right: 24px;
    margin-left: 9px;
    width: 225px;
    height: 40px;
    overflow: auto;
}
.dot {
    height: 16px;
    width: 16px;
    background: #2F4858;
    border-radius: 50%;
    text-align: centre;
    z-index: 2;
}

.line {
    background: #2F4858;
    width:1px;
    height:56px;

    z-index: 0;
    }

.firstline {
    background:  #2F4858;
    width:1px;
    height:35px;
    margin-top: 20px;
    position:absolute;
    left: 146px;
    z-index:1;
    }

.lastline {
    background:  #2F4858;
    width:1px;
    height:35px;
    margin-bottom: 24px;
    position:absolute;
    left: 146px;
    z-index:1;
    }
</style>