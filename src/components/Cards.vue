<script setup>
import { ref } from 'vue';

const brokenLinkIcon = ref('/images/broken-chain-link.png');
const inboxIcon = ref('/images/inbox.png');
</script>

<template>
    <h1 style="color:gray;">Custom Card Design</h1>
    <div class="main-div">
        <div class="card">
            <div class="card-content">
                <div class="coming-soon">
                    <img v-bind:src="brokenLinkIcon" alt="Spinner Icon" />
                    <p class="cs-txt">Coming soon!</p>
                    <p>Stay tuned for future updates!</p>
                </div>
                <div class="inbox">
                    <div class="inbox-content">
                        <div class="ib-container">
                            <img v-bind:src="inboxIcon" class="ib-icon" height="100" alt="Inbox Icon" />
                        </div>
                        <div class="available">
                            <h3>Inbox</h3>
                            <div class="badge">Available</div>
                        </div>
                        <p>Manage support tickets, requests, and customer communication, all from one inbox</p>
                        <span>Customer support software</span>
                    </div>
                </div>
            </div>
        </div>

        <div class="card2">
            <div class="card-content">
                <div class="coming-soon">
                    <img v-bind:src="brokenLinkIcon" alt="Spinner Icon" />
                    <p class="cs-txt">Coming soon!</p>
                    <p>Stay tuned for future updates!</p>
                </div>
                <div class="inbox">
                    <div class="inbox-content">
                        <div class="ib-container">
                            <img v-bind:src="inboxIcon" class="ib-icon" height="100" alt="Inbox Icon" />
                        </div>
                        <div class="available">
                            <h3>Inbox</h3>
                            <div class="badge">Available</div>
                        </div>
                        <p>Manage support tickets, requests, and customer communication, all from one inbox</p>
                        <span>Customer support software</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
h1 {
    text-align: center;
    font-family: 'poppins';
    text-transform: uppercase;
}

.main-div {
    display: inline-flex;
    justify-content: center;
    width: 100%;
}

.ib-container {
    /* border:1px solid red; */
    margin-top: -50px;
}

.ib-icon {
    /* width: 200px; */
    margin-left: -40px;
}

.cs-txt {
    color: #1E1F24;
    text-align: center;
    font-family: "Inter Variable";
    font-size: 0.875rem;
    font-style: normal;
    font-weight: 600;
    line-height: 1.25rem;
}

.card {
    background-color: #ffffff;
    border-radius: 12px;
    /* box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); */
    overflow: hidden;
    width: 300px;
    margin: 20px;
}

.card2 {
    background-color: #ffffff;
    border-radius: 12px;
    /* box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); */
    overflow: hidden;
    width: 300px;
    margin: 20px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.card:hover {
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.card-content {
    padding: 1px;
}

.coming-soon {
    text-align: center;
    border-bottom: 1px solid #e0e0e0;
    padding: 2.25rem 0rem 3.125rem 0rem;
    /* margin-bottom: 20px; */
    /* border: 1px solid green; */
    background-color: rgb(241, 241, 241);
    border-radius: 10px;
    margin: 5px;
}

.coming-soon img {
    width: 24px;
    height: 24px;
    margin-bottom: 10px;
}

.coming-soon p {
    margin: 5px 0;
    color: #777777;
}

.inbox {
    display: flex;
    align-items: center;
}

.inbox-content {
    margin: 20px;
    display: flex;
    flex-direction: column;
}

.inbox-content h3 {
    margin: 0;
    font-size: 18px;
    color: #333333;
}

.inbox-content p {
    margin: 5px 0;
    font-size: 14px;
    color: #777777;
}

.inbox-content span {
    font-size: 12px;
    color: #aaaaaa;
}

.available {
    display: inline-flex;
    width: 260px;
    /* border: 1px solid red; */
    margin-top: -50px;
}

.badge {
    display: inline-block;
    background-color: #e0f7e0;
    color: #28a745;
    border-radius: 12px;
    padding: 2px 8px;
    font-size: 12px;
    margin-left: 140px;
    width: 50px;
}
/* ***********************Media Queries*********************** */
@media (max-width: 425px) {
    .main-div {
        display: block;
        text-align: center;
    }

    .card,
    .card2 {
        margin: 10px auto;
    }
}
</style>
