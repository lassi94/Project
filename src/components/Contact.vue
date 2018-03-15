<template>
  <div class="Contact">
    <div class="container">
        <h1 class="title">
          {{ title }}
        </h1>
        <h2 class="subtitle">
            {{ subtitle }}
        </h2>
        <div class="field">
            <div class="columns">
                <div class="column is-5">
                    <label class="label">Email</label>
                    <div class="control has-icons-left has-icons-right">
                        <input type="text" class="input" placeholder="Email">
                        <span class="icon is-small is-left">
                            <i class="fas fa-envelope"></i>
                        </span>
                    </div>
                    <label class="label" id="subject-class">Subject</label>
                    <div class="control has-icons-left has-icons-right">
                        <input type="text" class="input" placeholder="Subject">
                        <span class="icon is-small is-left">
                            <i class="fas fa-bookmark"></i>
                        </span>
                    </div>
                    <a class="button">
                        <span>Send</span>
                    </a>
                </div>
                <div class="column is-7">
                    <label class="label">Message</label>
                    <div class="control">
                        <textarea class="textarea" id="text-area" cols="30" rows="6" placeholder="Please insert your message.."></textarea>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Contact',
    data(){
        return{
            title: 'Contact me with the form below ',
            subtitle: 'Do not hesitate to contact me for further information about me'
        }
    }
  
}
</script>

<style lang="sass" scoped>

@import '../mq.sass'

h1.title
    margin: 50px 0 50px 0

h2.subtitle
    margin: 0 0 50px 0
    
.field
    #subject-class
        margin: 20px 0 10px 0
    .button
        margin: 20px 0 0 0
        color: $pri-color
        border: 1px solid $pri-color
        &:hover
            background-color: $pri-color
            color: #fff

.Contact
    margin: 0 0 50px 0

</style>


