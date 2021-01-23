<template>
  <div>
    <Comment
      v-for="(comment, index) in comments"
      :key="index"
      :comment="comment"
    />
  </div>
</template>

<script>
import Comment from '~/components/Comment.vue'
export default {
  components: { Comment },
  data() {
    return {
      comments: [
        {
          message:
            'Hi guys i am really proud to join this group and be able to meet new bengladeshis friends !',
          author: 'Shahid',
          likes: 23,
          date: '12-11-2020',
        },
        {
          message:
            'Hae duae provinciae bello quondam piratico catervis mixtae praedonum a Servilio pro consule missae sub iugum factae sunt vectigales.',
          author: 'Nadim',
          likes: 11,
          date: '12-11-2020',
        },
        {
          message:
            'Et hae quidem regiones velut in prominenti terrarum lingua positae ob orbe eoo monte Amano disparantur.',
          author: 'Dini',
          likes: 7,
          date: '12-11-2020',
        },
      ],
    }
  },
}
</script>

<style></style>
