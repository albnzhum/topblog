<template>
    <table>
        <thead>
            <tr>
                <th>Имя файла</th>
                <th>Количество подписчиков</th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="file in files" :key="file.name">
                <td class="file-name">{{ file.name }}</td>
                <td class="file-subscribes">{{ file.subscribes }}</td>
            </tr>
        </tbody>
    </table>
</template>
  
<script>
export default {
    data() {
        return {
            files: [
                { name: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod", subscribes: "159,99" },
                { name: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod", subscribes: "159,99" },
                { name: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod", subscribes: "159,99" }
            ]
        };
    }
};
</script>

<style> 

table {
     border-collapse: collapse;
     width: 680px;
     height: auto;
     flex-shrink: 0;
 }

 .file-name {
     display: inline-block;
     width: 281px;
     -webkit-box-orient: vertical;
     -webkit-line-clamp: 1;

     /*----FONT------ */
     overflow: hidden;
     color: #2A2626;
     text-overflow: ellipsis;
     white-space: nowrap;
     font-size: 18px;
     font-style: normal;
     font-weight: 400;
     line-height: 140%;

 }

 .file-subscribes {
     color: #2A2626;
     font-size: 18px;
     font-style: normal;
     font-weight: 400;
     line-height: 140%;
     text-align: center;
     /* 25.2px */
 }


 th,
 td {
     border: none;
     padding: 10px;
 }

 td {
     align-items: flex-start;
 }

 tr:nth-child(even) {
     background-color: white;
 }

 th {
     border-bottom: 1px solid #D6E0EA;
     background-color: white;
     color: #4663AB;
     font-size: 20px;
     font-style: normal;
     font-weight: 700;
     line-height: 140%;
     text-align: left;
     /* 28px */
 }
</style>