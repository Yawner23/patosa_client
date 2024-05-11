<template>
    <div class="h-screen bg-gradient-to-b from-black to-black flex justify-center items-center">
        <div class="mx-auto max-w-7xl px-6 py-16 sm:py-24 lg:px-8">
            <h2 class="text-2xl font-bold leading-10 tracking-tight text-white">Frequently asked questions</h2>
            <p class="mt-6 max-w-2xl text-base leading-7 text-gray-300">Have a different question and can’t find the answer
                you’re looking for? Reach out to our support team by <a href="#"
                    class="font-semibold text-indigo-400 hover:text-indigo-300">sending us an email</a> and we’ll get back
                to you as soon as we can.</p>
            <div class="mt-20">
                <dl
                    class="space-y-16 sm:grid sm:grid-cols-2 sm:gap-x-6 sm:gap-y-16 sm:space-y-0 lg:grid-cols-3 lg:gap-x-10">
                    <div v-for="faq in faqs" :key="faq.id">
                        <dt class="text-base font-semibold leading-7 text-white">{{ faq.question }}</dt>
                        <dd class="mt-2 text-base leading-7 text-gray-300">{{ faq.answer }}</dd>
                        
                    </div>
                </dl>
            </div>
        </div>
    </div>
</template>
  
<script setup>
const faqs = [
    {
        id: 1,
        question: "Why do we form this band?",
        answer:
            "We form this band to entertain many people and we form this band to be well-known in the world",
    },
    {
        id: 2,
        question: "What genre do we usually play?",
        answer:
            "In the event we play alternative but we mostly play rock music in our practice",
    },
]
</script>