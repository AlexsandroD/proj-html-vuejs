<template>
         <form>
                    <div class="input-container">
                        <input type="text" placeholder="Name">
                        <input type="email"  placeholder="Email">
                        <input type="number"  placeholder="Phone">
                        <select>
                            <option value="More Info">More Info</option>
                            <option value="Pices"><a href="#">Prices</a></option>
                            <option value="Deals"><a href="#">Deals</a></option>
                        </select>
                    </div>
                    <textarea placeholder="Message"></textarea>
                    <ButtonForm/>
                </form>
</template>

<script>
import ButtonForm from "../micro/ButtonForm.vue";
export default {
    name:"Form",
    components:{
        ButtonForm,
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
  form{
            .input-container{
                display: grid;
                grid-template-columns:repeat(auto-fill, calc(50% - 5px));
                column-gap:10px;
                row-gap: 10px;
                margin: 5px 0;
                input[type=text], select,input[type=email],input[type=number] {
                width: 100%;
                padding: 8px 20px;
                display: inline-block;
                border:none;
                border-radius: 2px;
                box-sizing: border-box;
                background-color: #ECECEC;
                }
                select{
                    color: gray;
                }
            }
        textarea {
            margin: 10px 0;
            width: 100%;
            padding: 10px;
            aspect-ratio: 4;
            background-color: #ECECEC;
            border: none;
            border: none;
            overflow: auto;
            outline: none;

            -webkit-box-shadow: none;
            -moz-box-shadow: none;
            box-shadow: none;

            resize: none; /*remove the resize handle on the bottom right*/
        }

        }
</style>