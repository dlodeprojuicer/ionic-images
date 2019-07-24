<template>
   <ion-content>
    <table>
      <tr>
        <th>id</th>
        <th>tag</th>
        <th>source</th>
        <th>type</th>
        <th>render</th>
      </tr>
      <tr v-for="item in ionArray" :key="item.id">
        <td>{{ item.id }}</td>
        <td>{{ item.tag }}</td>
        <td>{{ item.source }}</td>
        <td>{{ item.type }}</td>
        <td><ion-img :src="item.source" width="10" /></td>
      </tr>
      <tr v-for="item in imgArray" :key="item.id">
        <td>{{ item.id }}</td>
        <td>{{ item.tag }}</td>
        <td>{{ item.source }}</td>
        <td>{{ item.type }}</td>
        <td><ion-img :src="item.source" width="140"></ion-img></td>
      </tr>
    </table>
  </ion-content>
</template>

<script>
export default {
  name: "header",
  data() {
    return {
      ionArray: [
        {
          id: 0,
          tag: "<ion-img>",
          source: "http://www.own-appeal.com/images/common/logo.png",
          type: "png"
        },
        {
          id: 1,
          tag: "<ion-img>",
          source: "https://ionicframework.com/docs/demos/api/card/madison.jpg",
          type: "jpg"
        },
        {
          id: 2,
          tag: "<ion-img>",
          source: "../img/logo.png",
          type: "png"
        },
        {
          id: 3,
          tag: "<ion-img>",
          source: "../img/madison.jpg",
          type: "jpg"
        },
        {
          id: 4,
          tag: "<ion-img>",
          source: "../assets/logo.png",
          type: "png"
        },
        {
          id: 5,
          tag: "<ion-img>",
          source: "../assets/madison.jpg",
          type: "jpg"
        }
      ],
      imgArray: [
        {
          id: 6,
          tag: "<img>",
          source: "http://www.own-appeal.com/images/common/logo.png",
          type: "png"
        },
        {
          id: 7,
          tag: "<img>",
          source: "https://ionicframework.com/docs/demos/api/card/madison.jpg",
          type: "jpg"
        },
        {
          id: 8,
          tag: "<img>",
          source: "../img/logo.png",
          type: "png"
        },
        {
          id: 9,
          tag: "<img>",
          source: "../img/madison.jpg",
          type: "jpg"
        },
        {
          id: 10,
          tag: "<img>",
          source: "../assets/logo.png",
          type: "png"
        },
        {
          id: 11,
          tag: "<img>",
          source: "../assets/madison.jpg",
          type: "jpg"
        }
      ]
    };
  }
};
</script>

<style>
table {
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width: 50%;
  margin: 0 auto;
}

td, th {
  border: 1px solid #dddddd;
  text-align: left;
  padding: 20px;
}

tr:nth-child(even) {
  background-color: #dddddd;
}

ion-img {
  height: 90px;
  width: 100px;
}
</style>
