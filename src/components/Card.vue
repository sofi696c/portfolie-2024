<template>
    <div class="card">
      <div class="text-content">
        <h3>{{ title }}</h3>
        <p>{{ description }}</p>
      </div>
      <div class="image-container">
        <img :src="image" alt="project image">
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      title: {
        type: String,
        required: true
      },
      description: {
        type: String,
        required: true
      },
      image: {
        type: String,
        required: true
      }
    }
  }
  </script>
  
  <style scoped>
  .card {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 20px;
    width: 100%;
    max-width: 800px;
    background-color: #d4dad4;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    margin-bottom: 50px;
  }
  
  .text-content {
    flex: 1;
    padding-right: 20px;
  }
  
  .image-container {
    flex: 0 0 40%;
    display: flex;
    justify-content: flex-end;
  }
  
  .image-container img {
    width: 100%;
    height: auto;
    max-width: 200px;
  }
  
  h3 {
    font-family: 'Raleway', sans-serif;
    font-size: 24px;
    margin-bottom: 10px;
  }
  
  p {
    font-family: 'Raleway', sans-serif;
    text-align: left;
    line-height: 1.6;
    width: 90%;
  }
  
  /* Responsive Design */
  @media (max-width: 768px) {
    .card {
      flex-direction: column;
      align-items: center;
    }
  
    .text-content, .image-container {
      flex: 1;
      width: 100%;
      text-align: center;
      padding-right: 0;
    }
  
    h3 {
      font-size: 1.2em;
    }
  
    p {
      font-size: 0.9em;
    }
  
    .image-container img {
      max-width: 100%;
    }
  }
  </style>
  