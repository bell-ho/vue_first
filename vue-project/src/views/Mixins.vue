<script>
import ApiMixin from '../api.js';
export default {
    mixins: [ApiMixin],
    data() {
        return {
            productList: []
        };
    },
    async mounted() {
        this.productList = await this.$callAPI("https://8daa045a-f995-4be6-9aa3-f5c2ecb1bf5b.mock.pstmn.io/list", "get");
        console.log(this.productList);
    }
}
</script>