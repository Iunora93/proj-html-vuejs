<script>
export default {
  name: "AppCard",
  props: {
    img: String,
    title: String,
    info: String,
  },
};
</script>

<template>
    
            <main>
                <div class="card">
                    <img :src="img" :alt="title" />
                    <div class="info-card">
                        <h3>{{ title }}</h3>
                        <hr>
                        <span>{{info}}</span>
                    </div>
                </div>
            
            </main>
</template>

<style lang="scss" scoped>
    main{
        display: flex;
        .card{       
            
            width: calc(100% / 4);
            
            
            img{
                width: 100%;
                height: auto;
                border: 1px solid white;
            }
            h3{
                
                color: #b9afa1;
            }
            hr{
                border-color: #b9afa1;  
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

    }
</style>