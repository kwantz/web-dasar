<template>
    <v-layout>
        <v-tabs fixed centered>
            <v-tabs-bar dark class="green darken-1">
                <v-tabs-slider class="blue"/>
                <v-tabs-item :key="1" :href='"#tab1"'>
                    Income
                </v-tabs-item>
                <v-tabs-item :key="2" :href='"#tab2"'>
                    Expense
                </v-tabs-item>
            </v-tabs-bar>
            <v-tabs-items>
                <v-tabs-content :key="1" :id='"tab1"'>
                    <form-wallet name="income"/>
                </v-tabs-content>
                <v-tabs-content :key="2" :id='"tab2"'>
                    <form-wallet name="expense"/>
                </v-tabs-content>
            </v-tabs-items>
        </v-tabs>
    </v-layout>
</template>

<script>
import FormWallet from './FormWallet'

export default {
    components: { FormWallet }
}
</script>
