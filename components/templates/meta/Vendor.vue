<template>
    <v-container>
        <v-row>
            <v-col class="mt-0">
                <MM_Rating 
                    :value = 'data.rating'
                    :action = 'action' 
                    :title = '"Rating"' 
                    :action_key = '"rating"'
                />
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
    import MM_Input from '~/components/lib/MM_Input'
    import MM_Rating from '~/components/lib/MM_Rating'
    export default {
        name: "vendorMeta",
        props: ['data', 'action'],
        components: {MM_Input, MM_Rating},
        data() {
            return {}
        },
    }
</script>