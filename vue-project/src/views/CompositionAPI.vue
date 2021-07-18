<template>
    <div>
        <div>계산기</div>
        <div>
            <input type="text" v-model="num1" @keyup="plusNumbers"/>
            <span> + </span>
            <input type="text" v-model="num2" @keyup="plusNumbers"/>
            <span> = </span>
            <span>{{ result }}</span>
        </div>
    </div>
</template>
<script>
import {reactive} from 'vue';

export default {
    name: '계산기',
    setup() {
        let state = reactive({ //reactive를 이용하여 실시간 변경에 따른 반응형 적용
            num1: 0,
            num2: 0,
            result: 0
        });

        function plusNumbers() {
            state.result = parseInt(this.num1) + parseInt(this.num2);
        }

        return { //reactive로 선언된 state와 plusNumbers 함수를 반환함으로써 기존 data , methods 옵션처럼 사용가능
            state,
            plusNumbers
        }
    }
}
</script>