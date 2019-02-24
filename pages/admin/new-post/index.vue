<template>
  <div class="admin-new-post-page">
    <section class="new-post-form">
      <form @submit.prevent="onSave"> 
        <AppControlInput v-model="editedPost.author">Author Name</AppControlInput>
        <AppControlInput v-model="editedPost.title">Title</AppControlInput>
        <AppControlInput v-model="editedPost.thumbnailLink">ThumbnailLink</AppControlInput>
        <AppControlInput control-type="textarea" v-model="editedPost.content">Content</AppControlInput>
        <AppButton type="submit">Save</AppButton>
        <AppButton
          @click="onCancel"
          btn-style="cancel"
          style="margin-left: 10px;"
          type="button"
        >Cancel</AppButton>
      </form>
    </section>
  </div>
</template>

<script>
import AppControlInput from '@/components/UI/AppControlInput'
import AppButton from '@/components/UI/AppButton'
export default {
    components:{
        AppControlInput,
        AppButton
    },
    data(){
        return{
            editedPost:{
                author:'',
                title: '',
                thumbnailLink:'',
                content:''
            }
        }
    },
    methods:{
        onSave(){
            console.log(this.editedPost)
        },
        onCancel(){
            this.$router.push('/admin')
        }
    }
}
</script>