<template>
  <div id="app">
    <RadarChart></RadarChart>
  </div>
</template>

<script>
import Anchor from '@/new_comp/Anchor'
import BackTop from '@/new_comp/BackTop'
import ColumnOne from '@/new_comp/ColumnOne'
import ColumnTwo from '@/new_comp/ColumnTwo'
import ColumnThree from '@/new_comp/ColumnThree'
import Content from '@/new_comp/Content'
import Cover from '@/new_comp/Cover'
import HeadBar from '@/new_comp/HeadBar'
import Indicator from '@/new_comp/Indicator'
import Share from '@/new_comp/Share'
import FbComment from '@/new_comp/FBComment'
import ParallaxBg from '@/new_comp/ParallaxBg'
import Youtube from '@/new_comp/Youtube'
import Quote from '@/new_comp/Quote'
import Question from '@/new_comp/Question'
import Relate from '@/new_comp/Relate'
import Logo from '@/new_comp/Logo'
import Foot from '@/new_comp/Foot'
import RadarChart from '@/components/RadarChart'
export default {
  name: 'App',
  components: {
    Anchor,
    BackTop,
    ColumnOne,
    ColumnTwo,
    ColumnThree,
    Content,
    Cover,
    HeadBar,
    Indicator,
    Share,
    Relate,
    RadarChart,
    FbComment,
    ParallaxBg,
    Youtube,
    Quote,
    Question,
    Logo,
    Foot
  },
  data () {
    return {
      testCom: {
        name: ColumnOne,
        props: null
      },
      headJSON: {
        headColor: "#fff",
        iconColor: "#000"
      },
      coverJSON: {
        position: "centerCenter",
        src: '../static/CoverBg/cover_mob.jpg',
        srcWeb: '../static/CoverBg/cover_pc.jpg',
        useArrow: 'yes'
      },
      coverJSON_2: {
        position: "leftCenter",
        src: '../static/CoverBg/cover_mob.jpg',
        srcWeb: '../static/CoverBg/cover_pc.jpg',
        useArrow: 'yes',
        useAnimate: true
      },
      Anchor_1: {
        title: '我是安可落一號'
      },
      Anchor_2: {
        title: '我是毛點將'
      },
      ColumnOneJSON: {
        src: '../static/SectionBg/SectionBg_mob.jpg',
        srcWeb: '../static/SectionBg/SectionBg_pc.jpg',
        description: '有段時間阿邦很怕人家問他「家在哪？」「爸爸媽媽呢？」只能笑而帶過'
      },
      ColumnTwoJSON: {
        src_1: '../static/SectionBg/SectionBg_mob.jpg',
        srcWeb_1: '../static/SectionBg/SectionBg_pc.jpg',
        src_2: '../static/SectionBg/SectionBg_mob.jpg',
        srcWeb_2: '../static/SectionBg/SectionBg_pc.jpg',
        description: '有段時間阿邦很怕人家問他「家在哪？」「爸爸媽媽呢？」只能笑而帶過'
      },
      ColumnThreeJSON: {
        src_1: '../static/SectionBg/SectionBg_mob.jpg',
        srcWeb_1: '../static/SectionBg/SectionBg_pc.jpg',
        src_2: '../static/SectionBg/SectionBg_mob.jpg',
        srcWeb_2: '../static/SectionBg/SectionBg_pc.jpg',
        src_3: '../static/SectionBg/SectionBg_mob.jpg',
        srcWeb_3: '../static/SectionBg/SectionBg_pc.jpg',
        description: '有段時間阿邦很怕人家問他「家在哪？」「爸爸媽媽呢？」只能笑而帶過'
      },
      relateData: {
        title: '延伸閱讀',
        href1: 'https://udn.com/news/story/7315/3275143',
        text1: '手球國手被公車撞死 母親淚訴「不能讓女兒白白犧牲」',
        img1: 'https://udn.com/upf/udn/busjustice_201807/static/web/008.jpg',
        href2: 'https://udn.com/news/story/7315/3275143',
        text2: '手球國手被公車撞死 母親淚訴「不能讓女兒白白犧牲」',
        img2: 'https://udn.com/upf/udn/busjustice_201807/static/web/008.jpg',
        href3: 'https://udn.com/news/story/7315/3275143',
        text3: '手球國手被公車撞死 母親淚訴「不能讓女兒白白犧牲」',
        img3: 'https://udn.com/upf/udn/busjustice_201807/static/web/008.jpg',
        href4: 'https://udn.com/news/story/7315/3275143',
        text4: '手球國手被公車撞死 母親淚訴「不能讓女兒白白犧牲」',
        img4: 'https://udn.com/upf/udn/busjustice_201807/static/web/008.jpg'
      },
      Share: {
        href: 'https://udn.com/news/story/7315/3275143'
      },
      Quote: {
        text: '用JSON來寫引言',
        img: '../static/quoteImg.png',
        refer: '李先生'
      },
      Question: {
        href: "https://www.youtube.com/embed/UBEEKPBU_68",
        text: "jsonProps test"
      }
    }
  },
  created () {
    this.testCom.props = this.ColumnOneJSON
  },
  mounted () {
    
  }
}
</script>

<style module>
.give6vh{
  width: 100%;
  height: 200vh;
}
</style>
