<template>
<div>
<Header/>
<LogisticsSection/>
<IssueSection/>
<BenefitSection/>
<AdvantagesSection/>
<TransportManagementSection/>
<Footer/>
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

export default {
  name: 'Main',
  components: {
    Header,
    LogisticsSection,
    IssueSection,
    BenefitSection,
    AdvantagesSection,
    TransportManagementSection,
    Footer
  }
}
</script>

<style lang='scss' scoped>

</style>
