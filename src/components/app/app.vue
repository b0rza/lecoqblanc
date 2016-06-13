<script>
import template from './template.html';
import Diner from 'components/diner/diner';

export default {
  template,

  // Hooks
  // ---------------------------------------
  created() {
    this.diners = this.getDiners();
  },

  // Components
  // ---------------------------------------
  components: {
    Diner,
  },

  // Models
  // ---------------------------------------
  data() {
    return {
      diners: [],
    };
  },

  // Methods
  // ---------------------------------------
  methods: {
    getDiners() {
      return [{
        name: 'Le Coq Blanc',
        address: 'Jurasova 970',
        contacts: ['099-201-3333'],
        hours: ['09-23', '10-22'],
      }];
    },
  },
};
</script>

<style scoped lang="scss" src="./style.scss"></style>
