<template>
  <div class="numberLike">
    <p>{{likeValue}}</p><button @click="addLike" class="buttonjaimepost"><i class="fa-solid fa-heart"></i>
    </button>
  </div>
</template>


<script>
export default {
  data() {
    return {
      likeValue: "",
        
      counternumber:[]
      
    };
  },
  methods: {
    addLike() {
      
      
      
      


      // const token = localStorage.getItem("token");
      // if (token) {
      //   const options = {
      //     method: "POST",
      //     headers: {
      //       "Content-Type": "application/json",
      //       "Authorization": "bearer " + token,
      //     },
    
      //     body: JSON.stringify({
      //       postId: this.likeValue,
      //     }),
      //   };

      //   console.log("like:",this.likeValue)
      // }
      //   const response = await fetch(
      //     "https://social-network-api.osc-fr1.scalingo.io/ntmsmile/post",
      //     options
      //   );

      //   const data = await response.json();
      // }
    }
  },
}

</script>

<style scoped lang="scss">
.numberLike {
  display: flex;
}

.buttonjaimepost {
  border: none;
  margin-top: 5px;
  padding: 6px;
  border-radius: 25px;
  background-color: white;
  cursor: pointer;

  i {
    border-radius: 30px;
    background-color: #1DA1F2;
    padding: 10px;
    color: white;

    &:hover {

      background-color: white;
      color: #1DA1F2;
      transition: 0.3s;
    }
  }
}
</style>