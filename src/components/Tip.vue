<script>
  export default {
    name: 'vue-treeselect--tip',
    functional: true,

    props: {
      type: {
        type: String,
        required: true,
      },
      icon: {
        type: String,
        required: true,
      },
    },

    render() {
      return (
        <div class={`vue-treeselect__tip vue-treeselect__${this.type}-tip`}>
          <div class="vue-treeselect__icon-container">
            <span class={`vue-treeselect__icon-${this.icon}`} />
          </div>
          <span class={`vue-treeselect__tip-text vue-treeselect__${this.type}-tip-text`}>
            {this.$slots.default()}
          </span>
        </div>
      )
    },
  }
</script>
