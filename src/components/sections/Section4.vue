<template>
  <section class="section4">
      <div class="container">
        <div class="filter"></div>
        <div class="text-container">
                <h5>what are we doing</h5>
                <h2><span>Results</span> in Numbers</h2>
        </div>
        <div class="results-container">
            <div class="results" v-for="(result,index) in results" :key="index">
                <div class="number">{{result.number}}</div>
                <div class="area">{{result.area}}</div>
            </div>
        </div>
      </div>
  </section>
</template>

<script>
export default {
    name:"Section4",
    data(){
        return{
            results:[
                {
                    number:"128",
                    area:"Certifications",
                },
                {
                    number:"230",
                    area:"Employees",
                },
                {
                    number:"517",
                    area:"Customers",
                },
                {
                    number:"94",
                    area:"Countries Served",
                },
                
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
    .section4{
        overflow: hidden;
        position: relative;
        height: 450px;
        background-image:url("../../assets/img/bg-10.jpg");
        background-size: cover;
        background-position-y: -200px;
        .container{
            width: 65%;
            margin: auto;
            padding:100px 0;
        }
        .filter{
            position: absolute;
            top: 0;
            right: 0;
            left: 0;
            bottom: 0;
            z-index: -1;
        }
        .text-container{
            display: flex;
            flex-direction: column;
            width: 50%;
            margin: auto;
            text-align: center;
            color: #fff;
            h5{
                text-transform: uppercase;
                color: $blue-text;
                font-size: 1rem;
            }
            h2{
                font-size: 2rem;
                margin: 15px 0;
                font-weight: 900;
                span{
                    padding: 1px 10px;
                    background-color: #0384844a;
                }
            }
        }
        .results-container{
            margin: 70px 0px;
            display: grid;
            grid-template-columns:repeat(auto-fill, 25%);
            justify-content: center;
            .results{
                column-gap:15px;
                text-align: center;
                .number{
                    color: $blue-text;
                    margin: 10px 0;
                    font-size: 1.4rem;
                    font-weight: 700;
                }
                .area{
                    color: white;
                }
            }
        }
    }

</style>