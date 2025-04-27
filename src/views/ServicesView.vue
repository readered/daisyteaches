<template>
    <div>
        <page-header>Services</page-header>
        <div class="mx-[25%] my-20">
            <section :class="serviceSectionClasses">
                <h3 :class="serviceHeaderClasses">Small Group Sessions</h3>
                <p>Boost your confidence and work towards your best grade with small group GCSE tuition!</p>
                <p>These interactive, highly engaging sessions focus on developing skills for both Literature and
                    Language and cover all key GCSE topics: from crafting a great piece of creative writing to mastering
                    close literary analysis. Group tuition students benefit from a collaborative, motivating environment
                    and a shared goal with their online classmates.</p>
                <p>Group sessions are capped at 5 students per class to ensure all can benefit from a suitably
                    personalised and supportive approach.</p>
                <p>Group sessions include a weekly piece of (optional) homework and feedback.</p>
                <hr>
                <p>£25 per session, one session per week.</p>
                <p>These sessions are only bookable in advance, in half-termly blocks.</p>
                <p class="italic bold">From September 2025 group sessions will run on Mondays and Tuesdays
                    17:15 –
                    18:15.</p>
            </section>
            <section :class="serviceSectionClasses">
                <h3 :class="serviceHeaderClasses">1-1 Sessions</h3>
                <p>Perfect for honing your general English skills, revising a topic, reviewing a piece of work,
                    practising exam technique... Or a combination of the above! All sessions are tailored to the needs
                    of
                    the student, with individual goals and timeframes in mind.</p>
                <p>All resources are provided for students to use during the session and take away afterwards.</p>
                <p>A weekly (optional) piece of homework and feedback is included.</p>
                <p>All sessions are taught online.</p>
                <p>1-1 tutoring is most impactful when booked as a regular session – as such I offer a 10% block booking
                    discount for students wanting to commit to 10 sessions up front.</p>
                <hr>
                <p>£50 per session for KS3 & GCSE</p>
                <p>£55 per session for A Level</p>
                <p>10% discount for block bookings of 10 sessions</p>
                <p>Please note that all sessions are payable in advance.</p>
                <p class="italic bold">Some limited availability remaining for September 2025 starters. Please contact
                    me to discuss.</p>
            </section>
            <section :class="serviceSectionClasses">
                <h3 :class="serviceHeaderClasses">Extra Marking</h3>
                <p>Struggling to master your exam responses? Unclear on where an all-important mock or piece of homework
                    went wrong? Or simply keen to get feedback on practise work you’re completing in your own time? I
                    offer detailed marking and feedback to suit every student, in written or video form to suit your
                    needs.</p>
                <p>Prices from £15.</p>
            </section>
        </div>
        <div class="w-full flex justify-center mb-30">
            <link-button link="/contact">Contact Me</link-button>
        </div>

    </div>
</template>

<script lang="ts" setup>
import LinkButton from '../components/LinkButton.vue'
import PageHeader from '../components/PageHeader.vue'
const serviceHeaderClasses = ["font-extrabold", "text-2xl", "mb-5"]
const serviceSectionClasses = ["mb-20"]
</script>

<style scoped>
p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
    font-family: Jost, sans-serif;
    font-weight: lighter;
}

p.bold {
    font-weight: bold;
}

hr {
    width: 50%;
    margin: 0 auto 2rem;
}
</style>