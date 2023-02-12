<template>
  <div>
    <section-index-hero
      user-name="I Am Khan Igor"
      :job="['Developer', 'Frontend', 'Fullstack', 'Freelancer']"
      :locations="locations"
    />
    <section-about
      title="About Me"
      text="I am a website designer from Lousiana, with a strong focus in UI/UX design. I love to get new experiences and always learn from my surroundings. I've done more than 285 projects. You can check it through portfolio section on
            this website. I looking forward to any opportunities and challenges."
      :skills="skills"
    />
    <section-quote
      text="Do more than is required. What is the distance between someone who achieves their goals consistently and those who spend their lives and careers merely following? The extra mile."
      author="Khan Igor"
    />
    <section-services
      title="What I Do"
      :services="services"
    />
    <section-portfolio
      title="Portfolio"
      :cases="cases"
    />
    <section-resume
      title="My Resume"
      title-col1="Experiences"
      title-col2="Education"
      :items-col1="resumeItems1"
      :items-col2="resumeItems2"
    />
    <section-facts
      :items="facts"
    />
    <section-blog
      title="Recent Blog"
      :posts="posts"
    />
    <section-contact
      title="Contact Me"
      bg-image="/images/background/5.jpg"
      :items="contacts"
    />
  </div>
</template>

<script>
import SectionIndexHero from "~/components/sections/SectionIndexHero";
import SectionAbout from "~/components/sections/SectionAbout";
import SectionQuote from "~/components/sections/SectionQuote";
import SectionServices from "~/components/sections/SectionServices";
import sectionPortfolio from "~/components/sections/SectionPortfolio";
import SectionResume from "~/components/sections/SectionResume";
import SectionFacts from "~/components/sections/SectionFacts";
import SectionBlog from "~/components/sections/SectionBlog";
import SectionContact from "~/components/sections/SectionContact";
export default {
  name: 'IndexPage',
  components: {
    SectionIndexHero, SectionAbout, SectionQuote,
    SectionServices, sectionPortfolio, SectionResume,
    SectionFacts, SectionBlog, SectionContact
  },
  layout: 'main',
  data() {
    const locations = [{
      loc1: 'Russia',
      loc2: 'Khabarovsk',
    }];
    const skills = [
      { name: 'HTML', percent: 90 },
      { name: 'CSS', percent: 85 },
      { name: 'PHP', percent: 80 },
      { name: 'jQuery', percent: 75 }
    ];
    const services = [
      {
        icon: 'icon_genius',
        name: 'Branding',
        text: 'Ex velit cupidatat magna voluptate deserunt quis et dolor adipisicing elit culpa ad exercitation proident irure deserunt irure.'
      },
      {
        icon: 'icon_tools',
        name: 'Development',
        text: 'Ex velit cupidatat magna voluptate deserunt quis et dolor adipisicing elit culpa ad exercitation proident irure deserunt irure.'
      },
      {
        icon: 'icon_camera_alt',
        name: 'Photography',
        text: 'Ex velit cupidatat magna voluptate deserunt quis et dolor adipisicing elit culpa ad exercitation proident irure deserunt irure.'
      },
    ];
    const cases = [
      {
        url: 'single-project.html',
        name: 'Single Image',
        tag: 'website',
        img: '/images/gallery/1.jpg'
      },
      {
        url: 'single-project-2.html',
        name: 'Multiple Images',
        tag: 'website',
        img: '/images/gallery/2.jpg'
      },
      {
        url: 'single-project-3.html',
        name: 'Self Hosted Video',
        tag: 'website',
        img: '/images/gallery/3.jpg'
      },
      {
        url: 'single-project.html',
        name: 'Bluetec App',
        tag: 'website',
        img: '/images/gallery/4.jpg'
      },
      {
        url: 'single-project.html',
        name: 'Uhost Hosting',
        tag: 'website',
        img: '/images/gallery/5.jpg'
      },{
        url: 'single-project.html',
        name: 'Bolo Creative',
        tag: 'website',
        img: '/images/gallery/6.jpg'
      },
    ];
    const resumeItems1 = [
      {
        date: '2014 - now',
        text: '<span class="d_title">Founder &amp; Creative Director</span><span class="d_company">Kyros Studio</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi tempora perferendis vero officia enim impedit voluptatem dignissimos, veniam ratione est alias rerum aperiam, nam aliquam reprehenderit iste dolor.'
      },
      {
        date: '2010 - 2014',
        text: '<span class="d_title">Senior UI / UX Designer</span><span class="d_company">Google Inc</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi tempora perferendis vero officia enim impedit voluptatem dignissimos, veniam ratione est alias rerum aperiam, nam aliquam reprehenderit iste dolor.'
      },
      {
        date: '2008 - 2010',
        text: '<span class="d_title">Graphic Designer</span><span class="d_company">Kyros Studio</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi tempora perferendis vero officia enim impedit voluptatem dignissimos, veniam ratione est alias rerum aperiam, nam aliquam reprehenderit iste dolor.'
      },
    ];
    const resumeItems2 = [
      {
        date: '2004 - 2008',
        text: '<span class="d_title">Master in Design</span><span class="d_company">New York University</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi tempora perferendis vero officia enim impedit voluptatem dignissimos, veniam ratione est alias rerum aperiam, nam aliquam reprehenderit iste dolor.'
      },
      {
        date: '2004 - 2008',
        text: '<span class="d_title">Bachelor of Arts</span><span class="d_company">University of London</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi tempora perferendis vero officia enim impedit voluptatem dignissimos, veniam ratione est alias rerum aperiam, nam aliquam reprehenderit iste dolor.'
      },
      {
        date: '2006 - 2004',
        text: '<span class="d_title">Artist of College</span><span class="d_company">University of Sydney</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi tempora perferendis vero officia enim impedit voluptatem dignissimos, veniam ratione est alias rerum aperiam, nam aliquam reprehenderit iste dolor.'
      },
    ];
    const facts = [
      { name: 'Hours of Works', value: '8240' },
      { name: 'Projects Done', value: '315' },
      { name: 'Satisfied Customers', value: '250' },
      { name: 'Awards Winning', value: '32' },
    ];
    const posts = [
      {
        url: 'single-blog.html',
        image: '/images/blog/1.jpg',
        title: 'How to Make Better User Interface',
        text: `Dolore officia sint incididunt non excepteur ea mollit commodo ut enim reprehenderit cupidatat labore ad
              laborum consectetur consequat...`,
      },
      {
        url: 'single-blog.html',
        image: '/images/blog/2.jpg',
        title: '10 Web Design Tips From Experts',
        text: `Dolore officia sint incididunt non excepteur ea mollit commodo ut enim reprehenderit cupidatat labore ad
              laborum consectetur consequat...`,
      },
      {
        url: 'single-blog.html',
        image: '/images/blog/3.jpg',
        title: 'The Importance of Web Design',
        text: `Dolore officia sint incididunt non excepteur ea mollit commodo ut enim reprehenderit cupidatat labore ad
              laborum consectetur consequat...`,
      },
      {
        url: 'single-blog.html',
        image: '/images/blog/4.jpg',
        title: '10 Web Design Tips From Experts',
        text: `Dolore officia sint incididunt non excepteur ea mollit commodo ut enim reprehenderit cupidatat labore ad
              laborum consectetur consequat...`,
      },
      {
        url: 'single-blog.html',
        image: '/images/blog/5.jpg',
        title: 'The Importance of Web Design',
        text: `Dolore officia sint incididunt non excepteur ea mollit commodo ut enim reprehenderit cupidatat labore ad
              laborum consectetur consequat...`,
      },
      {
        url: 'single-blog.html',
        image: '/images/blog/6.jpg',
        title: 'Tips for Healthy Teeth',
        text: `Dolore officia sint incididunt non excepteur ea mollit commodo ut enim reprehenderit cupidatat labore ad
              laborum consectetur consequat...`,
      }
    ];
    const contacts = [
      { title: 'Email Me', text: 'contact@kyrosnoriaki.com' },
      { title: 'Call Me', text: '+1 700 333 92 96' },
      { title: 'Address', text: 'Collins Street West, Louisiana, Bayerfurt, USA' }
    ];
    return {
      locations, skills,
      services, cases,
      resumeItems1, resumeItems2,
      facts, posts, contacts
    };
  },

  head() {
    return {
      script: [
        { src: "/js/recaptcha.js" },
        { src: "/js/typed.js" }
      ]
    };
  }
}
</script>

<style lang="scss">
:root {
  --primary-color: #CF1F1F;
  --primary-color-rgb: 207, 31, 31;
}
</style>
