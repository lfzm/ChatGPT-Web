<script lang="ts" setup>
import { NAvatar } from 'naive-ui'
import defaultAvatar from '@/assets/avatar.jpg'
import UserAvatar from '@/assets/img_head.png'

interface Props {
  image?: boolean
}
defineProps<Props>()


</script>

<template>
  <template v-if="image">
    <NAvatar round :src="UserAvatar" />  
  </template>
  <template v-else>
    <NAvatar round :src="defaultAvatar" />
  </template>
</template>
