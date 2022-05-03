<template>
    <header> 
         <SiteLogo />
        <div class="header-container">
            <div class="logo">
                <img src="@/assets/img/dc-logo.png" alt="logo">
            </div>
            <nav class="header-navbar">
                <ul>
                    <li>
                        <h3>ciao</h3>
                        <h3>ciao</h3>
                        <h3>ciao</h3>
                        <h3>ciao</h3>
                        <h3>ciao</h3>
                        <h3>ciao</h3>
                        <h3>ciao</h3>
                        <h3>ciao</h3>
                        <h3>ciao</h3>
                        <h3>ciao</h3>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
import SiteLogo from '@/components/HeaderComponents';
export default {
    name: 'HeaderComponents',
    components: {
        SiteLogo
    }
}
</script>

<style lang="scss" scoped>  
header{
    
    .header-container{
        margin: 0 auto;
        display: flex;
        justify-content: space-around;
        align-items: center;
        .logo{
            margin: 15px 10px;
        }
        .header-navbar{
            ul{
                display: flex;
                li {
                    padding: 15px;
                    list-style: none;
                    text-transform: uppercase;
                    font-weight: bold;
                    cursor: pointer;
                    
                    &:hover{
                        color: black;
                        border-bottom: 5px solid blue;
                    }
                    a{
                        text-decoration: none;
                        color: grey;
                    }
                }
            }
        }
    }
};
</style>



