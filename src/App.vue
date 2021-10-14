<template>
  <div id="app">
    <Header :infoNav="linkNav" :infoMed="media" :infoShop="shop"/>
    <Main :infoCourses="courses" :infoCarosel="carosel"/>
    <Footer :infoMed="media" :infoLinkFooter="footerLink"/>
  </div>
</template>

<script>
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import Header from './components/Header.vue'



export default {
  name: 'App',
  components: {
    Main,
    Footer,
    Header,
  },
  data(){
    return{
      // common header-footer
      linkNav:["Home", "Pages", "Courses", "Features", "Blog", "Shop"],
      media:["fa-twitter", "fa-facebook-f", "fa-instagram", "fa-linkedin"],
      shop:["far fa-caret-square-right", " far fa-life-ring"," fas fa-book","fas fa-shopping-cart"],
      footerLink:[
        {
          title:"Titolo-1",
          link:["link1", "link2", "link3", ]
        },
          {
          title:"Titolo-2",
          link:["link1", "link2", "link3","link5"]
        }

      ],
      // common header-footer

        //Carosel
        carosel:[
          {
            title:"REAL STORIES",
            text: "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me",
            img: require('./assets/images/testimonial-avata-01.jpg'),
            pg:"Florence Themes",
            job:"/Multimedia Admin"
          },
          {
            title:"REAL STORIES",
            text: "I'm a very strict person so I require everything to be organized and neat. Then, I'll be able to make things right and shine. MaxCoach guys just got me",
            img: require('./assets/images/testimonial-avata-02.jpg'),
            pg:"Mina Hollace",
            job:"/Freelancer"
          },
          {
            title:"REAL STORIES",
            text: "I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students",
            img: require('./assets/images/testimonial-avata-03.jpg'),
            pg:"Tony Stark",
            job:"/Private Tutor"
          },
          {
            title:"REAL STORIES",
            text: "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me",
            img: require('./assets/images/testimonial-avata-03.jpg'),
            pg:"Madley Pondor",
            job:"/IT Specialist",
          }
          ,
        ],

      // sezione COURSES 
      courses:[
        {
          imge:require('./assets/images/motivation-course-06-480x298.jpg'),
          price:'$30.00',
          text:'How to be Successful: create a Growt Mindset For Success',
          icons:[
            {
              img :"fas fa-book  my-5",
              text: "3 Lessons"

            },
            {

              img: "far fa-user ms-5",
              text: "50 Students"
            },
          ]

        },
        {
          imge:require('./assets/images/motivation-course-05-480x298.jpg'),
          price:'$30.00',
          text:'How to be Successful: create a Growt Mindset For Success',
          icons:[
            {
              img :"fas fa-book  my-5",
              text: "3 Lessons"

            },
            {

              img: "far fa-user ms-5",
              text: "50 Students"
            },
          ]
        },
        {
          imge:require('./assets/images/motivation-course-04-480x298.jpg'),
          price:'$30.00',
          text:'How to be Successful: create a Growt Mindset For Success',
          icons:[
            {
              img :"fas fa-book  my-5",
              text: "3 Lessons"

            },
            {

              img: "far fa-user ms-5",
              text: "50 Students"
            },
          ]
        },
        {
          imge:require('./assets/images/motivation-course-03-480x298.jpg'),
          price:'$30.00',
          text:'How to be Successful: create a Growt Mindset For Success',
          icons:[
            {
              img :"fas fa-book  my-5",
              text: "3 Lessons"

            },
            {

              img: "far fa-user ms-5",
              text: "50 Students"
            },
          ]
        },
        {
          imge:require('./assets/images/motivation-course-02-480x298.jpg'),
          price:'$30.00',
          text:'How to be Successful: create a Growt Mindset For Success',
          icons:[
            {
              img :"fas fa-book  my-5",
              text: "3 Lessons"

            },
            {

              img: "far fa-user ms-5",
              text: "50 Students"
            },
          ]
        },
        {
          imge:require('./assets/images/motivation-course-01-480x298.jpg'),
          price:'$30.00',
          text:'How to be Successful: create a Growt Mindset For Success',
          icons:[
            {
              img :"fas fa-book  my-5",
              text: "3 Lessons"

            },
            {

              img: "far fa-user ms-5",
              text: "50 Students"
            },
          ]
        }
      ]
      
    }
  }
}
</script>

<style lang="scss">
@import './assets/style/common.scss';

</style>
