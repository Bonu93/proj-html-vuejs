<template>
    <div class="calendar d-flex flex-column">
        <div class="calendar-title p-4">
            <h3 class="m-0">Upcoming Events</h3>
        </div>
        <div class="calendar-event d-flex p-4"
        v-for="(event, i) in data.calendarData"
        :key="`event-${i}`"
        >
            <div class="date text-center">
                <span class="day">{{ event.day }}</span> {{ event.date }}
            </div>
            <div class="event-details d-flex flex-column mx-3">
                <h4>{{event.name}}</h4>
                <div class="time">
                    <span class="subtitle">
                        <i class="far fa-clock"></i> {{ event.time }}
                    </span>
                </div>
                <div class="location">
                    <span class="subtitle">
                        <i class="fas fa-map-marker-alt"></i>
                        {{ event.location }}
                    </span>
                </div>
                <a href="#" class="read-more">Read More</a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Calendar",
    props: {
        data: Object,
    },
};
</script>

<style lang="scss" scoped>
@import "@/styles/globals.scss";

.calendar {
    background-color: $white-alt;
}
.coaching {
    margin-right: 1rem;
    background-image: url("../assets/img/h1-img-09.jpg");
    background-position-y: 30%;
    background-size: cover;
    font-size: 12px;
    .calendar-title {
        box-shadow: rgba(33, 35, 38, 0.1) 0px 10px 10px -10px;
        background: $white-alt;
    }
    h4 {
        font-size: 1.2rem;
    }
    .date {
        background: $orange;
        color: white;
        height: 60px;
        width: 60px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        font-size: 10px;
        .day {
            display: block;
            font-size: 1rem;
        }
    }
}

.calendar-event {
    cursor: pointer;
    &:hover {
        background: white;
        box-shadow: rgba(33, 35, 38, 0.1) 0px 10px 10px -10px;
        h4 {
            color: $orange;
        }
    }
    i {
        color: $orange;
    }
}
</style>
