<template>
    <div>
        <b-container fluid class="p-4">
            <b-row>
                <b-col>  
	         <b-img thumbnail fluid :src="require('../static/d1.jpg')" alt="Image 1"></b-img> 
                </b-col>
                <b-col>
		 <b-img thumbnail fluid :src="require('../static/d2.jpg')" alt="Image 2"></b-img> 
                </b-col>
                <b-col>
                 <b-img thumbnail fluid :src="require('../static/d3.jpg')" alt="Image 3"></b-img>
                </b-col>
            </b-row>
        </b-container>
        <b-container fluid class="p-4">
            <b-row>
                <b-col>  
	         <b-img thumbnail fluid :src="require('../static/d4.jpg')" alt="Image 1"></b-img> 
                </b-col>
                <b-col>
		 <b-img thumbnail fluid :src="require('../static/d5.jpg')" alt="Image 2"></b-img> 
                </b-col>
                <b-col>
                 <b-img thumbnail fluid :src="require('../static/d6.jpg')" alt="Image 3"></b-img>
                </b-col>
            </b-row>
        </b-container>
    </div>
</template>
<script>
export default {
    
}
</script>