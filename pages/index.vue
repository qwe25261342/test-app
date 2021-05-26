<template>
  <div>
    <div class="cont">
      <div class="buttonbox">
        <Secondary v-for="(v,k) in secondary" :key="k" :title="v"> 
        </Secondary>
      </div>

      <div class="cardbox">
        <Video v-for="(item,index) in videos" :key="index" :video="item">
        </Video>
     </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      "secondary": [
          "All",
          "Music", 
          "One Piece", 
          "Animine", 
          "Love songs"
      ],
      "index": 0,
      "videos":[
        {
          title:
            "Drake - Started From The Bottom (Explicit)",
          img:"https://i.ytimg.com/vi/RubBzkZzpUA/hqdefault.jpg?sqp=-oaymwEcCOADEI4CSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLAp-UMFhwG680rBQHjSqtw2bpCBaA",
          time:"10:50",
          user:"面白大丈夫 ● 觀看次數：4.5萬次 ● 2天前"
        },
        {
          title:
            "Imagine Dragons - Demons (Official Video)",
          img:"https://i.ytimg.com/vi/mWRsgZuwf_8/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLAgqR0KvbRVV5cfupuEVRUu0VmpwA",
          time:"10:00",
          user:"Allengoaround ● 觀看次數：3.5萬次 ● 1天前"
        },
        {
          title:
            "大蛇丸】數十萬珍藏大公開家人到底會有什麼反應!",
          img:"https://i.ytimg.com/vi/xC_dGXoBFDk/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLCz4Z8bCSSycK9GF3tmXbrV_pUBmQ",
          time:"14:12",
          user:"大蛇丸 ● 觀看次數：14.4萬次 ● 2天前"
        },
        {
          title:
            "TAI TAI STORY邰哥甲史之歷史懸案 秦始皇到底是誰生的？",
          img:"https://i.ytimg.com/vi/MFhEND7Y3G4/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLADj4CNVW4NYgpznbU4rueqbgjbXQ",
          time:"25:40",
          user:"木曜4超玩● 觀看次數：108萬次 ● 2天前"
        },
        {
          title:
            "Drake - Started From The Bottom (Explicit)",
          img:"https://i.ytimg.com/vi/RubBzkZzpUA/hqdefault.jpg?sqp=-oaymwEcCOADEI4CSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLAp-UMFhwG680rBQHjSqtw2bpCBaA",
          time:"10:50",
          user:"面白大丈夫 ● 觀看次數：4.5萬次 ● 2天前"
        },
        {
          title:
            "Imagine Dragons - Demons (Official Video)",
          img:"https://i.ytimg.com/vi/mWRsgZuwf_8/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLAgqR0KvbRVV5cfupuEVRUu0VmpwA",
          time:"10:00",
          user:"Allengoaround ● 觀看次數：3.5萬次 ● 1天前"
        },
        {
          title:
            "大蛇丸】數十萬珍藏大公開家人到底會有什麼反應!",
          img:"https://i.ytimg.com/vi/xC_dGXoBFDk/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLCz4Z8bCSSycK9GF3tmXbrV_pUBmQ",
          time:"14:12",
          user:"大蛇丸 ● 觀看次數：14.4萬次 ● 2天前"
        },
        {
          title:
            "TAI TAI STORY邰哥甲史之歷史懸案 秦始皇到底是誰生的？",
          img:"https://i.ytimg.com/vi/MFhEND7Y3G4/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLADj4CNVW4NYgpznbU4rueqbgjbXQ",
          time:"25:40",
          user:"木曜4超玩● 觀看次數：108萬次 ● 2天前"
        },
        {
          title:
            "Drake - Started From The Bottom (Explicit)",
          img:"https://i.ytimg.com/vi/RubBzkZzpUA/hqdefault.jpg?sqp=-oaymwEcCOADEI4CSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLAp-UMFhwG680rBQHjSqtw2bpCBaA",
          time:"10:50",
          user:"面白大丈夫 ● 觀看次數：4.5萬次 ● 2天前"
        },
        {
          title:
            "Imagine Dragons - Demons (Official Video)",
          img:"https://i.ytimg.com/vi/mWRsgZuwf_8/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLAgqR0KvbRVV5cfupuEVRUu0VmpwA",
          time:"10:00",
          user:"Allengoaround ● 觀看次數：3.5萬次 ● 1天前"
        },
        {
          title:
            "大蛇丸】數十萬珍藏大公開家人到底會有什麼反應!",
          img:"https://i.ytimg.com/vi/xC_dGXoBFDk/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLCz4Z8bCSSycK9GF3tmXbrV_pUBmQ",
          time:"14:12",
          user:"大蛇丸 ● 觀看次數：14.4萬次 ● 2天前"
        },
        {
          title:
            "TAI TAI STORY邰哥甲史之歷史懸案 秦始皇到底是誰生的？",
          img:"https://i.ytimg.com/vi/MFhEND7Y3G4/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLADj4CNVW4NYgpznbU4rueqbgjbXQ",
          time:"25:40",
          user:"木曜4超玩● 觀看次數：108萬次 ● 2天前"
        },
      ]
    };
  },
};
</script>

