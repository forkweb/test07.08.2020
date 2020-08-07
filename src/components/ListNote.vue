<template>
  <div class="notes">



    <div class="list-notes">

      <div class="notes-item">
        <div class="notes-item__title">
          <h3>Заголовок</h3>
        </div>
        <div class="notes-item__block">

          <input type="checkbox" id="jack" value="1" v-model="checkedNoteItem">
          <label for="jack">Выполнить первое задание</label>
          <input type="checkbox" id="john" value="2" v-model="checkedNoteItem">
          <label for="john">Выполнить второе задание</label>
          <input type="checkbox" id="mike" value="5" v-model="checkedNoteItem">
          <label for="mike">Выполнить пятое задание</label>
          <br>
          <span>Отмеченные заметки: {{ checkedNoteItem }}</span>
          
        </div>
      </div>

    </div>

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: function() {
    return {
      checkedNoteItem: []
    };
  },
  props: {
    msg: String
  }
}
</script>

<style lang="scss" type="text/scss">
  @import "~@/style/list_note.scss";
</style>