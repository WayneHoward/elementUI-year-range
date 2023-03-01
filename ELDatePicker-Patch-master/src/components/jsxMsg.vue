<script>
export default {
  name: 'jsxMsg',
  props: {
    msg: String
  },
  render () {
    const { msg } = this
    return (
      <div>{msg}</div>
    )
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
