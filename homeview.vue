<template>
    <div class="tour-details">
      <h2>The Weeknd World Tour</h2>
      <p>Join us on The Weeknd's world tour for an unforgettable musical journey.</p>
      
      <h2>Tour Dates</h2>
      <ul>
        <li v-for="date in tourDates" :key="date.id">{{ date.location }} - {{ date.date }}</li>
      </ul>
    </div>
  </template>
  
  <script setup>
  const tourDates = ref([
    { id: 1, location: 'New York', date: 'July 15, 2023' },
    { id: 2, location: 'Los Angeles', date: 'August 5, 2023' },
    { id: 3, location: 'London', date: 'September 10, 2023' },
  ]);
  
  </script>
  
  <style>
  /* Keep the existing styles and add new styles as needed for the website's look and feel */
  .tour-details {
    padding: 20px;
    font-family: Arial, sans-serif;
    max-width: 600px;
    margin: 0 auto;
    background-color: #fff;
    border: 1px solid #ddd;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  
  h2 {
    color: #333;
    margin-top: 0;
  }
  
  ul {
    list-style: none;
    padding: 0;
  }
  
  li {
    margin: 5px 0;
  }
  </style>
  