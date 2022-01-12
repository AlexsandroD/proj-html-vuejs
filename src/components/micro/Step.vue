<template>
     

<div class="step">
    <div class="steps">
        <span class="number">01</span>
        <div class="text">
        <h3>collection of information</h3>
        <p>Lorem ipsum dolor, sit amet consectetur.</p>
        </div>
    </div>
</div>
            
        
</template>

<script>
export default {
    name:"Step",
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss"; 

            .steps{
                width: 20%;
                text-align: center;
                margin: 0 20px;
                .step{
                    display: inline;
                }
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
        
</style>