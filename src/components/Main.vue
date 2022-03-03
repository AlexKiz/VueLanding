<template>
<div>
<Header @open='isModalOpen = true'/>
<LogisticsSection @open='isModalOpen = true'/>
<IssueSection/>
<BenefitSection @open='isModalOpen = true' id='benefit'/>
<AdvantagesSection id='advantages'/>
<TransportManagementSection @open='isModalOpen = true'/>
<Footer/>
<Modal v-if="isModalOpen" @close="isModalOpen = false" />
</div>
</template>

<script>
import Header from './Header.vue'
import LogisticsSection from './LogisticsSection.vue'
import IssueSection from './IssuesSection.vue'
import BenefitSection from './BenefitSection.vue'
import AdvantagesSection from './AdvantagesSection.vue'
import TransportManagementSection from './TransportManagementSection.vue'
import Footer from './Footer.vue'
import Modal from './Modal.vue'

export default {
  name: 'Main',
  components: {
    Header,
    LogisticsSection,
    IssueSection,
    BenefitSection,
    AdvantagesSection,
    TransportManagementSection,
    Footer,
    Modal
  },
  data () {
    return {
      isModalOpen: false
    }
  },
  methods: {
    handleModalOpen () {
      if (this.isModalOpen) {
        this.isModalOpen = false
        document.body.classList.remove('modal-open')
      } else {
        this.isModalOpen = true
        document.body.classList.add('modal-open')
      }
    }
  }
}
</script>

<style lang='scss' scoped>

</style>
