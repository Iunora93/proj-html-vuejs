<script>
export default {
  name: "AppCard",
  props: {
    img: String,
    title: String,
    info: String,
    hover: String,
  },
};
</script>

<template>          
    <div class="card">
        <div class="card-img">
            <img :src="img" :alt="title" />
            <div class="on-hover">
                <h5>{{hover}}</h5>
            </div>
        </div>
        <div class="info-card">
            <h3>{{ title }}</h3>
            <hr>
            <span>{{info}}</span>
            
        </div>
    </div>            
</template>

<style lang="scss" scoped>
    
        .card{       
            border: 1px solid #e1deda;
            width: calc(100% / 4);
            
            .card-img{
                position: relative;
                .on-hover{
                    color: white;
                    text-align: center;
                    position: absolute;                   
                    top: 0;
                    left: 0;
                    right: 0; 
                    display: none; 

                }
            }
            
            img{
                width: 100%;
                height: auto;
                border: 1px solid white;
            }
            h3{
                
                color: #b9afa1;
            }
            hr{
                border-color: #e1deda;  
                margin: 10px 0 10px 0;         
            }
            span{
                font-size: 12px;
                color: #747474;
                
                
            }
            .info-card{
                padding: 20px;
                
            }
        }
        .card:hover .on-hover {
                background-color: #b9afa1;
                width: 100%;
                height: 100%;
                display: flex;
                justify-content: center;
                align-items: center;
            }

    
</style>