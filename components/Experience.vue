<template>
    <div class="main">
        <v-container class="container">
            <h1>Experience</h1>

            <div class="timeline">
                <v-timeline dense>
                    <v-timeline-item data-aos="fade-up" small v-for="item in list" :key="item.id">
                        <div class="py-4">
                            <h2 class="headline font-weight-light mb-4 blue--text">
                                {{ item.title }}
                            </h2>
                            <small class="font-weight-bold">{{ item.subtitle }}<v-icon small>mdi-map-marker</v-icon> {{ item.location }}</small>
                            <div style="color: #b2bec3;">
                                {{ item.detail }}
                            </div>
                        </div>
                    </v-timeline-item>
                </v-timeline>
            </div>
        </v-container>
    </div>
</template>

<script>
import aosMixin from "@/mixin/aos.js";

export default {
    name: "Experience",
    mixins: [aosMixin],
    data() {
        return {
            list: [
                {
                    id: 1,
                    title: "Senior Manager Data Engineer",
                    subtitle: "PWC | Jun 2022 | Present | ",
                    location: "London, United Kingdom",
                    detail: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta tempora officia asperiores quidem ipsam culpa tenetur voluptatum voluptatem nesciunt itaque eius consectetur velit ab iste tempore cumque nam non provident omnis, laboriosam iure nobis minus consequatur cum? Amet, autem dolore! Quos, placeat."
                },
                {
                    id: 2,
                    title: "Advisory Client Engineering Data Engineer",
                    subtitle: "IBM | 11 months | ",
                    location: "London, United Kingdom",
                    detail: "Working at IBM Client Engineering team to provide end-to-end model for accelerating digital transformation. Project involvement NHS, Lloyds banking group and HSBC. Skills – People management, structured data management, big data, data analysis & modelling, data quality, Data Governance, Data fabric, Watson AI and CP4D"
                },
                {
                    id: 3,
                    title: "Big Data Engineer- Manager",
                    subtitle: "Lloyds Banking Group | 3 years | ",
                    location: "London, United Kingdom",
                    detail: "Data Engineer Manager within the 'Machine Learning Lab' - a centre of excellence within Lloyds Banking Group tasked with delivering Data Science-based solutions to multiple business units across the Group. Having specific responsibilities for engineering the data pipelines to enable the Group's crucial business activities. These initiatives leverage Big Data (on a Hadoop-based stack)"
                },
                {
                    id: 3,
                    title: "Application Developer Specialist-Team Lead",
                    subtitle: "Accenture | 2 years 3 months | ",
                    location: "London, United Kingdom",
                    detail: "This role aimed to design and develop data Integration and ETL Frameworks to support the Advanced Analytics development life cycle. Design of Data Structures to support data supply chain through client data lake, interim staging, advanced analytics data ingestion and analytic data set management."
                },
                {
                    id: 4,
                    title: "Technical Consultant",
                    subtitle: "Accenture | 6 months | ",
                    location: "London, United Kingdom",
                    detail: "Project: AstraZeneca Role : Technical Consultant. My role involved Create visibility files from raw AZ-financial data (part of the Visibility work -phase ), files will later on provide transparency to ‘who-spends- how-much-on-what’ through transactional data analysis followed by Value Targeting and Budgeting stages (part of the standard ZBB approach) Creating the data repository and tracking tool. Load, transform and extract large financial data. Create advanced reports in excel and Qlik Sense."
                },
                {
                    id: 5,
                    title: "Sr. Software Engineer Analyst",
                    subtitle: "Accenture | 1 year | ",
                    location: "London, United Kingdom",
                    detail: "Project: HMRC-WMPlus2 Role: Data Meddler -BA My role involves scanning the databases to find different characteristics or cases based on set criteria. Skills: Data/Business Analysis, Stakeholder Management, HMRC Functional Knowledge. Tools & Software: UNIX, Sybase, SQL, Excel 2013, WinSCP."
                },
                {
                    id: 6,
                    title: "PHP Developer",
                    subtitle: "Solution 11 | 1 year 5 months | ",
                    location: "Leeds, United Kingdom",
                    detail: "Solutions 11 is a small IT company specialising in IP telephony and business-to-business service. The company also designs backup software for accountancy packages. Although I was recruited as a PHP developer, my role also involved additional duties to help with the launch of new products."
                },
            ]
        }
    }
}
</script>

<style scoped>
.main {
    border-bottom: 1px solid #4e4e4e7f;
}
.container {
    border-right: 1px solid #4e4e4e7f;
}
</style>
