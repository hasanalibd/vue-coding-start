<script setup>
import people from './data/data'
</script>

<template>
    <section>
        <h1 style="text-align:center;margin:40px 0px;font-size:40px">Data Example</h1>
        <section class="grid md:grid-cols-3 gap-8">
            <!-- <section class="person">
                <img :src="people[0].image" alt="Jane Doe">
                <div>
                    <h1 class="text-3xl font-semibold py-2">{{ people[0].name }}</h1>
                    <h2 class="text-2xl font-normal">{{people[0].designation}}</h2>
                    <p class="text-xl py-2">{{ people[0].location }}</p>
                </div>
            </section>
            <section class="person">
                <img :src="people[1].image" alt="Jane Doe">
                <div>
                    <h1 class="text-3xl font-semibold py-2">{{ people[1].name }}</h1>
                    <h2 class="text-2xl font-normal">{{people[1].designation}}</h2>
                    <p class="text-xl py-2">{{ people[1].location }}</p>
                </div>
            </section>
            <section class="person">
                <img :src="people[2].image" alt="Jane Doe">
                <div>
                    <h1 class="text-3xl font-semibold py-2">{{ people[2].name }}</h1>
                    <h2 class="text-2xl font-normal">{{people[2].designation}}</h2>
                    <p class="text-xl py-2">{{ people[2].location }}</p>
                </div>
            </section>
             -->

             <!-- loops people -->
             <section v-for="(data, index) in people" :key="index">
                <img :src="data.image" alt="Jane Doe">
                <div>
                    <h1 class="text-3xl font-semibold py-2">{{ data.name }}</h1>
                    <h2 class="text-2xl font-normal">{{ data.designation }}</h2>
                    <p class="text-xl py-2">{{ data.location }}</p>
                </div>
            </section>
        </section>
</section>
</template>

