<template>
    <div>
         <b-nav tabs>
            <b-nav-item disabled><strong>Quiz App</strong></b-nav-item>
            <b-nav-item disabled>Counter {{ correctAnswers }}/ {{ totalAnswers }}</b-nav-item>
        </b-nav>
        <div v-show="totalAnswers === 10">
            Congrats! You answered them all
        </div>
    </div>

</template>

<script>
export default {
    props: {
        correctAnswers: Number,
        totalAnswers: Number
    },
}
</script>