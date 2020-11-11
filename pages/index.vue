<template>
  <div>
    <hero />
    <capability />
    <project />
    <contact />
  </div>
</template>

<script>
import Hero from '@/components/Hero'
import Capability from '@/components/Capability'
import Project from '@/components/Project'
import Contact from '@/components/Contact'
export default {
  name: 'LandingPage',
  components: {
    Hero,
    Capability,
    Project,
    Contact
  }
}
</script>
