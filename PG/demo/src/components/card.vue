
<template>

  <img class="card-img-top img-fluid" :src="'/img2/' + setImg" alt="Card image" >
  <div class="card-body">
      <h5 class="card-title">{{ setName }}</h5>
      <p class="card-text">Some example text some example text.
          John Doe is an architect and engineer
      </p>
      <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#myModal1">
      See Profile
      </button>
      <!-- The Modal -->
      <div class="modal fade" id="myModal1">
          <div class="modal-dialog">
              <div class="modal-content">

              <!-- Modal Header -->
                  <div class="modal-header">
                      <h4 class="modal-title">Information</h4>
                      <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
                  </div>

                  <!-- Modal body -->
                  <div class="modal-body">
                  Lorem ipsum dolor sit, amet consectetur adipisicing elit. Pariatur alias adipisci aspernatur, odit error, consectetur aperiam sed consequatur voluptatum cumque temporibus eius quis molestias autem dolorem tempore? Ipsa, id pariatur.
                  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Fugit molestiae ex eligendi dolor ab obcaecati esse quae possimus iure sunt voluptatum minima, velit dolore error amet placeat repellendus ut. Laboriosam?
                  </div>

                  <!-- Modal footer -->
                  <div class="modal-footer">
                  <button type="button" class="btn btn-primary" data-bs-dismiss="modal">Enter</button>
                  </div>   
              </div>
          </div>
      </div>
  </div>
<!-- </div> -->

</template>

<script>
export default {
props: ['setName', 'setImg'],
} 

</script>


<style> 
.country-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  border: 3px solid #ddd;
  border-radius: 8px;
  height: 350px;
  width: 30%;
  margin: 10px;
  padding: 10px;
}

.card-img-top {
  width: 200px;
  height: auto;
  margin-bottom: 10px;
}

.card-body {
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
}

</style>    