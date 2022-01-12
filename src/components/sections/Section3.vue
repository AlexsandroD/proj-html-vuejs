<template>
  <div class="section3">
      <div class="container">
          <div class="text-container">
              <h5>how it works in practice</h5>
              <h2><span>Logistical</span> Procedures</h2>
              <p>We work with innovative methodologies to ensure that the entire delivery process is done from start to finish</p>
          </div>
          <div class="container-line-steps">
            <div class="line"></div>
            <div class="container-steps">
                <div class="steps" v-for="(step,index) in steps" :key="index">
                    <span class="number">{{step.number}}</span>
                    <div class="text">
                        <h3>{{step.title}}</h3>
                        <p>{{step.info}}</p>
                    </div>
                </div>
            </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name:"Section3",
    data(){
        return{
            steps:[
                {
                    number:"01",
                    title:"Collection of information",
                    info:" Lorem ipsum dolor sit amet consectetur."
                },
                {
                    number:"02",
                    title:"Service invoice sending",
                    info:" Lorem ipsum dolor sit amet consectetur."
                },
                {
                    number:"03",
                    title:"Withdrawal of Cargo",
                    info:" Lorem ipsum dolor sit amet consectetur."
                },
                {
                    number:"04",
                    title:"Transport Customer Order",
                    info:" Lorem ipsum dolor sit amet consectetur."
                },
                {
                    number:"05",
                    title:"Successful delivery",
                    info:" Lorem ipsum dolor sit amet consectetur."
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
 .section3{
     padding: 100px 0;
     background-color: #EEF4ED;

        .text-container{
            display: flex;
            flex-direction: column;
            width: 50%;
            margin: auto;
            text-align: center;
            h5{
                color: $bermuda;
                text-transform: uppercase;
            }
            h2{
                font-size: 2rem;
                margin: 15px 0;
                font-weight: 900;
                span{
                    padding: 1px 10px;
                    color: $dark-lagoon;
                    background-color: $light-coral;
                }
            }
            p{
                color: $silver-sand;
            }
        }
        .container-line-steps{
            position:relative;
            margin-top: 40px;
        }

       .line{
           position: absolute;
           top: -32px;
           width: 100%;
           height: 3px;
           background-color:$light-coral;
           margin: 50px 0;
           z-index: 1;
       }

        .container-steps{
            display: flex;
            width: 80%;
            margin: auto;
            .steps{
                width: 20%;
                text-align: center;
                margin: 0 20px;
                .number{
                    position: relative;
                    display: inline-block;
                    color: $blue-lagoon;
                    font-weight: 700;
                    padding: 10px;
                    border-radius: 50%;
                    background-color: $light-coral;
                    margin-bottom: 30px;
                    z-index: 2;
                }
                .text{
                    h3{
                        font-size: 1.3rem;
                    }
                    p{
                        color: $silver-sand;
                        margin: 10px 0;
                    }
                }
            }
        }
                    
}

</style>