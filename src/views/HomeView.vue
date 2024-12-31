<template>
  <v-app id="home">
    <NavBar />
    <v-container fluid>
      <div class="head">
        <!-- 流星背景 -->
        <div
          class="shooting-star"
          style="top: 10%; left: 80%; animation-delay: 0s"
        ></div>
        <div
          class="shooting-star"
          style="top: 20%; left: 60%; animation-delay: 1s"
        ></div>
        <div
          class="shooting-star"
          style="top: 30%; left: 40%; animation-delay: 2s"
        ></div>
        <v-row>
          <!-- 左側不規則漸層圖形 -->
           <div class="hide-on-mobile">  <div class="gradient-shape gradient-shape-left"></div>

<!-- 右側不規則漸層圖形 -->
<div class="gradient-shape gradient-shape-right"></div></div>
 
          <v-row cols="5" class="center-content" align="center" justify="space-between"> 
            <div style="position: relative" class="mainc">
              <h1 class="text-white-a">Hello, 我是</h1>
              <!-- 打字特效 -->
              <div class="typing-container">
                <span class="typing" id="typing-text"></span>
              </div>

              <a href="mailto:asd46639@gmail.com" class="mainbtn">聯絡我</a>
            </div>
          </v-row>
          <v-col cols="2">
            <div
              style="
                position: absolute;
                z-index: 9999;
                bottom: 0;
                margin-left: auto;
                margin-right: auto;
                left: 0;
                right: 0;
                text-align: center;
              "
              class="mt-16"
            >
              <v-icon>fas fa-angle-double-down</v-icon>
            </div>
          </v-col>
          <v-col cols="5">
            <div style="position: relative; z-index: 9999" class="mt-16 hide-on-mobile">
              <v-img src="i1.png" contain max-height="2000"></v-img>
            </div>
          </v-col>
        </v-row>
      </div>

      <v-col cols="12" class="mt-16" id="about">
        <div>
          <v-row>
            <v-col cols="12" sm="6">
              <div class="egg">
                <v-img src="name.JPG" max-height="300" class="photo"></v-img>
              </div>
            </v-col>
            <v-col cols="12" sm="6">
              <h5 class="mt-16">About Me</h5>
              <div style="width: 120px">
                <v-slider
                  v-model="slider2"
                  color="green"
                  label="track-color"
                ></v-slider>
              </div>
              <h4 class="mt-n4">I Am a Creative Product Designer</h4>

              <p class="text-grey">
                With extensive UI/UX design experience, I have contributed to
                impactful projects in multinational corporations and startups. I
                specialize in user-centric solutions, leveraging data analysis
                to address pain points and deliver results. Proficient in
                JavaScript and Vue, I excel in project management and
                cross-functional collaboration.
              </p>
              <br />
              <p class="text-grey">
                Additionally, I successfully managed a personal e-commerce
                brand, showcasing expertise in business operations and
                marketing. By blending innovative design with practical
                experience, I drive competitive advantages and sustainable
                growth for businesses.
              </p>
              <v-btn
                tile
                black
                color="#6D5ACF"
                class="mt-4 custom-btn"
                @click="downloadResume"
              >
                Download Resume
              </v-btn>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <div class="text-center mt-4">
        <h2>What I Do</h2>
        <div style="width: 120px; margin: 0 auto">
          <v-slider
            v-model="slider2"
            color="green"
            label="track-color"
          ></v-slider>
        </div>
      </div>
      <v-col cols="12" class="padd" id="portfolio">
        <div class="first" id="project">
          <v-row align="center" justify="space-evenly">
            <!-- Product Design Block -->
            <v-col cols="12" md="4" sm="6" class="portfolio-item">
              <div class="child">
                <v-btn
                  icon="fas fa-laptop"
                  color="#FBDF7E"
                  class="text-white"
                ></v-btn>
                <h3 class="ml-3 mt-4">Product Design (APP/WEB)</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  1. UI/UX Interface Design: Over 2 years of experience.<br />
                  2. Figma: Skilled in using Figma for efficient interface
                  design.<br />
                  3. Prototype and Flowchart: Quickly create interactive
                  prototypes and flowcharts to streamline project validation.<br />
                  4. Wireframe: Design wireframes to ensure consistency and
                  usability.<br />
                  5. Innovation: Demonstrate innovative thinking, user-centered
                  design, and effective team collaboration.
                </p>
              </div>
            </v-col>

            <!-- Illustration & Marketing Block -->
            <v-col cols="12" md="4" sm="6" class="portfolio-item">
              <div class="child">
                <v-btn
                  icon="fas fa-mobile-alt"
                  color="#88BCCB"
                  class="text-white"
                ></v-btn>
                <h3 class="ml-3 mt-4">Illustration ＆ Marketing</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  1. Created frame-by-frame animations using AE and
                  Procreate.<br />
                  2. Over 100,000 illustrations designed with hands-on
                  experience.<br />
                  3. Shopee E-Commerce: Increased product exposure and page
                  views by 2% and boosted purchase rates by 50%.<br />
                  4. Consumer Needs: Communicated extensively with customers to
                  understand their needs and resolve issues effectively.
                </p>
              </div>
            </v-col>

            <!-- Front-End Skills Block -->
            <v-col cols="12" md="4" sm="6" class="portfolio-item">
              <div class="child">
                <v-btn
                  icon="fas fa-camera"
                  color="#84B584"
                  class="text-white"
                ></v-btn>
                <h3 class="ml-3 mt-4">Front-End Skills</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  1. Front-End Development: Basic knowledge of CSS3, HTML5, and
                  JavaScript.<br />
                  2. Responsive Web Design: Focused on RWD to ensure optimal
                  user experience across devices.<br />
                  3. Vue Framework: Self-learning Vue.js framework to enhance
                  design and development integration.<br />
                  4. API Integration: Exploring API applications to expand
                  expertise.<br />
                  5. Quick Learning: Rapidly adapting to new tools and
                  technologies.
                </p>
              </div>
            </v-col>
          </v-row>
        </div>
      </v-col>

      <v-col cols="12" sm="12" id="services">
        <!-- <div class="d-flex justify-center mb-6">
          <v-btn
            color="#88bccb"
            class="mr-2"
            :class="{ active: activeTab === 'all' }"
            @click="changeTab('all')"
          >
            All
          </v-btn>
          <v-btn
            class="mr-2"
            variant="tonal"
            :class="{ active: activeTab === 'all' }"
            @click="changeTab('all')"
          >
            Figma Link
          </v-btn>
          <v-btn
            class="mr-2"
            variant="tonal"
            :class="{ active: activeTab === 'all' }"
            @click="changeTab('all')"
          >
            Illustration
          </v-btn>
        </div> -->
      </v-col>

      <!-- 根據標籤顯示內容 -->
      <div>
        <div v-if="filteredItems && filteredItems.length > 0">
          <v-row class="fill-height" align="center" justify="center">
            <template v-for="(item, i) in filteredItems" :key="i">
              <v-col cols="12" md="3">
                <v-card @click="navigateTo(item.url)" style="cursor: pointer">
                  <v-img :src="item.img" height="300px" cover></v-img>
                </v-card>
              </v-col>
            </template>
          </v-row>
        </div>
        <!-- 無內容時顯示 -->
        <div v-else class="text-center text-grey mt-6">
          <p>No items found for this category.</p>
        </div>
      </div>

      <!-- 作品集 -->

      <v-col cols="12" id="page">
        <div class="pre">
          <v-row>
            <v-col cols="12" sm="4">
              <v-card class="mx-auto" max-width="344" height="">
                <v-img src="i11.png" height="200px" cover></v-img>

                <v-card-title> Lolly E-commerce </v-card-title>

                <v-card-subtitle> ocean | 14 Dec 2024 </v-card-subtitle>
                <v-card-text>
                  設計發想：簡單操作，買賣雙方公平平台，不暴利！
                </v-card-text>
                <div class="pagecontent">
                  <button
                    class="more"
                    @click="
                      navigateTo(
                        'https://www.figma.com/proto/DVGkjHZNkSWcuqmB3fMzXQ/%E4%BD%9C%E5%93%81%E9%9B%86?page-id=331%3A25608&node-id=413-32724&p=f&viewport=442%2C167%2C0.11&t=Y693G2vGgfp5B75z-1&scaling=min-zoom&content-scaling=fixed&starting-point-node-id=331%3A31254'
                      )
                    "
                  >
                    詳細內容
                  </button>
                  <button
                    class="more"
                    @click="
                      navigateTo(
                        'https://www.figma.com/proto/1A7uLk91q1y2Sd7xxMK9iF/lolly-online-shop?page-id=1%3A51&node-id=54-32728&p=f&viewport=950%2C1376%2C0.06&t=CHYO9OiZjMRcEDPe-1&scaling=min-zoom&content-scaling=fixed&starting-point-node-id=9%3A51'
                      )
                    "
                  >
                    Prototype
                  </button>
                </div>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card class="mx-auto" max-width="344" height="">
                <v-img src="i12.png" height="200px" cover></v-img>

                <v-card-title> Tripow！ 旅遊規劃 </v-card-title>

                <v-card-subtitle> ocean | 14 Dec 2024 </v-card-subtitle>
                <v-card-text>
                  疫情後旅遊正夯！旅遊規劃自由行需求激增，一站式服務快狠準！
                </v-card-text>
                <div class="pagecontent">
                  <button
                    class="more"
                    @click="
                      navigateTo(
                        'https://www.figma.com/proto/DVGkjHZNkSWcuqmB3fMzXQ/%E4%BD%9C%E5%93%81%E9%9B%86?page-id=331%3A25608&node-id=413-32724&p=f&viewport=442%2C167%2C0.11&t=Y693G2vGgfp5B75z-1&scaling=min-zoom&content-scaling=fixed&starting-point-node-id=331%3A31254'
                      )
                    "
                  >
                    詳細內容
                  </button>
                  <button
                    class="more"
                    @click="
                      navigateTo(
                        'https://www.figma.com/proto/Rm8C1jdOUo8yEUKe2urcul/Tripow-Mandarin-version?page-id=390%3A15612&node-id=390-16129&p=f&viewport=324%2C44%2C0.04&t=AN4xz1O3seWIBb9O-1&scaling=contain&content-scaling=fixed&starting-point-node-id=390%3A16129&show-proto-sidebar=1'
                      )
                    "
                  >
                    Prototype
                  </button>
                </div>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card class="mx-auto" max-width="344" height="">
                <v-img src="i13.png" height="200px" cover></v-img>

                <v-card-title> 共伴 Together </v-card-title>

                <v-card-subtitle> ocean | 14 Dec 2024 </v-card-subtitle>
                <v-card-text>
                  「共伴 Together」是一款專為單身者與情侶， 打造的生活智能APP。
                </v-card-text>
                <div class="pagecontent">
                  <button
                    class="more"
                    @click="
                      navigateTo(
                        'https://www.figma.com/proto/DVGkjHZNkSWcuqmB3fMzXQ/%E4%BD%9C%E5%93%81%E9%9B%86?page-id=331%3A25608&node-id=413-32724&p=f&viewport=442%2C167%2C0.11&t=Y693G2vGgfp5B75z-1&scaling=min-zoom&content-scaling=fixed&starting-point-node-id=331%3A31254'
                      )
                    "
                  >
                    詳細內容
                  </button>
                  <button
                    class="more"
                    @click="
                      navigateTo(
                        'https://www.figma.com/proto/J86AaalT7zYvGdMB8ggTc2/Togethr-%E5%85%B1%E4%BC%B4?page-id=5%3A38&node-id=313-1914&viewport=7473%2C1682%2C0.41&t=ByKHDCm0uZR8pAql-1&scaling=min-zoom&content-scaling=fixed&starting-point-node-id=313%3A1914'
                      )
                    "
                  >
                    Prototype
                  </button>
                </div>
              </v-card>
            </v-col>
          </v-row>
        </div>
      </v-col>

      <!-- 無內容時顯示 -->

      <!-- <v-col cols="12" id="blog">
        <div class="hire">
          <v-row>
            <v-col cols="12" sm="8">
              <h1 class="mt-9">Hire me for your awesome project</h1>
              <p class="text-grey">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod
                itaque, eaque molestiae deleniti, earum voluptate eos id dicta
                at, blanditiis
              </p>
            </v-col>
            <v-col cols="12" sm="4">
              <v-btn color="#88bccb" class="mt-15">Hire Me</v-btn>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <v-col cols="12" sm="12" class="px-16" id="contact">
        <v-row>
          <v-col cols="12" sm="4">
            <div class="child">
              <h1>Contact info.</h1>
              <v-btn
                icon="fas fa-map-marker-alt"
                color=""
                class="mt-10"
                variant="outlined"
              ></v-btn
              ><br />
              <span class="text-caption">Taipei, Taiwan </span><br />
              <v-btn
                icon="fas fa-phone-alt"
                color=""
                class="mt-10"
                variant="outlined"
              ></v-btn
              ><br />
              <span class="text-caption">- </span> <br />

              <v-btn
                icon="fas fa-envelope"
                color=""
                class="mt-10"
                variant="outlined"
              ></v-btn
              ><br />
              <span class="text-caption">asd46639@gmail.com </span> <br />
            </div>
          </v-col>
          <v-col cols="12" sm="8">
            <h1 class="mt-8">Send your message</h1>
            <v-divider></v-divider>

            <v-row class="mt-10">
              <v-col cols="12" sm="6">
                <v-text-field
                  label="Name"
                  persistent-hint
                  variant="outlined"
                ></v-text-field>
              </v-col>
              <v-col cols="12" sm="6">
                <v-text-field
                  label="Phone No"
                  persistent-hint
                  variant="outlined"
                ></v-text-field>
              </v-col>
            </v-row>
            <v-textarea
              label="Message"
              persistent-hint
              variant="outlined"
            ></v-textarea>
            <v-btn color="#FBDF7E" class="mt-2">Submit Now</v-btn>
          </v-col>
        </v-row>
      </v-col> -->
    </v-container>
    <FooterView />
  </v-app>
</template>

<script>
import { defineComponent, ref, computed, onMounted } from "vue";
import NavBar from "../components/NavBar.vue";
import FooterView from "../components/FooterView.vue";

export default defineComponent({
  name: "HomeView",
  components: {
    NavBar,
    FooterView,
  },
  setup() {
    // 定義當前活躍標籤
    const activeTab = ref("all");

    // 定義項目資料
    const items = ref([
      {
        img: "/a1.png",
        tab: "all",
        url: "https://www.figma.com/proto/DVGkjHZNkSWcuqmB3fMzXQ/%E4%BD%9C%E5%93%81%E9%9B%86?page-id=331%3A25608&node-id=413-32724&p=f&viewport=430%2C69%2C0.23&t=9bWkqw2aabQmcoD7-1&scaling=contain&content-scaling=fixed&starting-point-node-id=331%3A31254",
      },
      {
        img: "/a2.png",
        tab: "all",
        url: "https://www.figma.com/design/DVGkjHZNkSWcuqmB3fMzXQ/%E4%BD%9C%E5%93%81%E9%9B%86?node-id=0-1&t=1Appu2lLSexDfZUw-1",
      },
      {
        img: "/a3.png",
        tab: "all",
        url: "https://github.com/tigers56797",
      },
      {
        img: "/i10.png",
        tab: "all",
        url: "",
      },
    ]);

    // 計算篩選後的項目
    const filteredItems = computed(() => {
      if (activeTab.value === "all") {
        return items.value;
      }
      return items.value.filter((item) => item.tab === activeTab.value);
    });

    const downloadResume = () => {
      const link = document.createElement("a");
      link.href = "/resume.pdf"; // 指向 public 資料夾中的檔案
      link.download = "Resume.pdf"; // 設定下載的檔案名稱
      link.click(); // 模擬點擊事件觸發下載
    };

    const navigateTo = (url) => {
      if (url) {
        window.open(url, "_blank");
      } else {
        console.error("No URL found for this item.");
      }
    };

    const changeTab = (tab) => {
      activeTab.value = tab;
    };

    // 打字效果輪播文字
    const texts = ["Ocean !", "產品設計師", "UI/UX設計師"];
    let textIndex = 0;
    let charIndex = 0; // 每個字的索引
    let isDeleting = false; // 是否正在刪除文字

    const typeText = () => {
      const typingElement = document.getElementById("typing-text");
      if (typingElement) {
        const currentText = texts[textIndex];
        // 判斷是否是刪除文字模式
        if (isDeleting) {
          charIndex--; // 每次減少一個字
        } else {
          charIndex++; // 每次增加一個字
        }

        // 更新文字顯示
        typingElement.textContent = currentText.substring(0, charIndex);

        // 判斷是否完成一個完整的文字顯示或刪除
        if (!isDeleting && charIndex === currentText.length) {
          isDeleting = true; // 開始刪除文字
          setTimeout(typeText, 1700); // 停留 1.7 秒後開始刪除
        } else if (isDeleting && charIndex === 0) {
          isDeleting = false; // 重新開始打下一句文字
          textIndex = (textIndex + 1) % texts.length; // 循環切換文字
          setTimeout(typeText, 700); // 停留 0.7 秒後開始新句
        } else {
          // 控制打字速度
          setTimeout(typeText, isDeleting ? 50 : 100); // 刪除時速度較快
        }
      }
    };

    // 流星生成函數
    const generateShootingStars = () => {
      const container = document.querySelector(".head"); // 獲取背景容器

      const createStar = () => {
        for (let i = 0; i < 10; i++) {
          // 每次生成 10 顆流星
          const star = document.createElement("div"); // 創建流星元素
          star.classList.add("shooting-star");

          // 随机位置和参数
    const randomTop = 10 + Math.random() * 80; // 保证在 10% - 90% 范围内
    const randomLeft = 10 + Math.random() * 80;
    const randomDelay = Math.random() * 5; // 随机延迟 0-5 秒
    const randomDuration = 2 + Math.random() * 4; // 持续时间 2-6 秒
    const randomAngle = Math.random() * 45 - 22.5; // 随机方向 -22.5° 到 +22.5°

          // 設置樣式
star.style.top = `${randomTop}%`;
star.style.left = `${randomLeft}%`;
star.style.animationDelay = `${randomDelay}s`;
star.style.animationDuration = `${randomDuration}s`;
star.style.transform = `rotate(${randomAngle}deg)`; // 添加隨機旋轉方向

          // 將流星加入背景容器
          container.appendChild(star);

          // 移除動畫結束的流星，防止 DOM 混亂
          star.addEventListener("animationend", () => {
            star.remove();
          });
        }
      };

      // 每隔一段時間動態生成流星
      setInterval(() => {
        createStar();
      }, 500); // 每隔 秒創建流星組
    };

    // 在組件掛載時執行
    onMounted(() => {
      typeText(); // 初始化打字效果
      generateShootingStars(); // 初始化流星效果
    });

    return {
      activeTab,
      items,
      filteredItems,
      downloadResume,
      changeTab,
      navigateTo,
    };
  },
});
</script>

<style scoped>
/* 全局排版 */
body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  color: #333;
  margin: 0;
  padding: 0;
}



.v-container {
  padding: 16px;
  overflow: hidden; /* 確保圖片放大後不超出範圍 */
}



.mainc {
  padding-left: 200px;
}

.v-card:hover .v-img {
  filter: brightness(50%); /* 減少亮度，呈現反黑效果 */
  transition: all 0.3s ease-in-out; /* 添加過渡效果 */
  transform: scale(1.1); /* 放大 10% */
}

.v-card .v-img {
  transition: all 0.3s ease-in-out; /* 添加過渡效果 */
  transform: scale(1); /* 預設大小 */
  overflow: hidden; /* 避免內容溢出 */
  height: 300px;
}
.text-white-a {
  font-size: 30px;
  color: #000000;
}

/* 深夜黑色漸變背景 */
.head {
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  display: flex;
  height: 100vh; /* 父容器高度設置為視窗高度 */
  align-items: center;
  justify-content: center;
  width: 100%;
  color: white;
  background: linear-gradient(120deg, #f9f9f9, #ffffff, #e3f2fd);
  background-size: 400% 400%; /* 确保动画有足够的移动空间 */
  animation: gradientAnimation 8s ease infinite; /* 确保动画正确应用 */
  overflow: visible; /* 确保流星不超出邊界 */
}


/* 左側圖形樣式 */
#home .gradient-shape-left {
  position: absolute;
  width: 150px !important; ; /* 圖形寬度 */
  height: 150px  !important; ; /* 圖形高度 */
  border-radius: 50%; /* 圓形基礎 */
  opacity: 0.4; /* 調整透明度，數值越小越透明 */
  top: 70%; /* 可適當調整位置 */
  left: 30px; /* 保持偏移 */
  /* filter: blur(2px); 添加模糊效果，數值越大模糊越強 */
  background: linear-gradient(175deg, rgba(255, 229, 126, 0.4), rgba(226, 175, 143, 0.4)); /* 漸層帶透明通道 */
  animation: float-left 12s infinite ease-in-out, gradient-change 20s infinite ease-in-out; /* 飄移+漸變動畫 */
}

/* 右側圖形樣式 */
#home .gradient-shape-right {
  position: absolute;
  width: 250px; /* 圖形寬度 */
  height: 250px; /* 圖形高度 */
  border-radius: 50%; /* 圓形基礎 */
  opacity: 0.4; /* 調整透明度 */
  top: 10%;
  right: 20px; /* 保持偏移 */
  /* filter: blur(2px); 添加模糊效果，數值越大模糊越強 */
  background: linear-gradient(135deg, rgba(132, 250, 176, 0.4), rgba(143, 211, 244, 0.4)); /* 漸層帶透明通道 */
  animation: float-right 11s infinite ease-in-out, gradient-change 20s infinite ease-in-out; /* 飄移+漸變動畫 */
  animation-delay: 1s; /* 添加延遲 */
  z-index: 1; /* 確保不被其他元素遮擋 */
}

/* 背景漸變動畫 */
@keyframes gradient-change {
  0% {
    background: linear-gradient(135deg, #ffe57e, #e2af8f);
  }
  10% {
    background: linear-gradient(135deg, #e2af8f, #f9f9a9);
  }
  25% {
    background: linear-gradient(135deg, #f9f9a9, #84fab0);
  }
  50% {
    background: linear-gradient(135deg, #84fab0, #8fd3f4);
  }
  75% {
    background: linear-gradient(135deg, #8fd3f4, #ffe57e);
  }
  90% {
    background: linear-gradient(135deg, #ffe57e, #e2af8f);
  }
  100% {
    background: linear-gradient(135deg, #ffe57e, #e2af8f); /* 循環回到起始 */
  }
}

/* 飄移動畫 */
@keyframes float-left {
  0% {
    transform: translateY(0px) translateX(0px);
  }
  50% {
    transform: translateY(-15px) translateX(15px); /* 稍微飄移 */
  }
  100% {
    transform: translateY(0px) translateX(0px);
  }
}

@keyframes float-right {
  0% {
    transform: translateY(0px) translateX(0px);
  }
  50% {
    transform: translateY(20px) translateX(-20px); /* 稍微飄移 */
  }
  100% {
    transform: translateY(0px) translateX(0px);
  }
}


.shooting-star {
  position: absolute;
  width: 10px;
  height: 10px;
  background: linear-gradient(
    90deg,
    rgba(255, 255, 255, 1), /* 明亮的白色起始 */
    rgba(255, 231, 153, 0.912), /* 黄色稍暗的尾部 */
    rgba(255, 242, 61, 0) /* 尾部完全透明 */
  );
  border-radius: 50%;
  animation: shooting-star 6s linear infinite, flicker 1.5s infinite; /* 增加闪烁效果 */
  transform-origin: left top;
  z-index: 1000;
}

@keyframes flicker {
  0%, 100% {
    filter: brightness(1); /* 正常亮度 */
  }
  50% {
    filter: brightness(1.5); /* 更明亮 */
  }
}
@keyframes shooting-star {
  0% {
    transform: translate(0, 0);
    opacity: 0; /* 起始完全可见 */
  }
  25% {
    opacity: 0.8; /* 稍微变暗 */
  }
  50% {
    opacity: 1; /* 恢复明亮 */
  }
  75% {
    opacity: 0.5; /* 更暗 */
  }
  100% {
    transform: translate(-500px, 500px); /* 终点位置 */
    opacity: 0; /* 消失 */
  }
}

/* 打字機效果 */
.typing {
  font-size: 4rem; /* 放大三倍 (3 x 原來的 3rem) */
  font-weight: bold; /* 加粗文字 */
  white-space: nowrap;
  overflow: hidden;
  border-right: 5px solid black; /* 打字效果游標 */
  animation: blink 0.6s step-end infinite alternate; /* 游標閃爍 */
  color: #3114c3; /* 黑色文字，可以按需更改 */
}

.mainbtn {
  display: flex;
  align-items: center; /* 垂直居中 */
  justify-content: center; /* 水平居中 */
  background-color: #000000;
  color: #ffffff;
  border-radius: 30px; /* 圓角按鈕 */
  width: 120px; /* 按鈕寬度 */
  height: 40px; /* 按鈕高度 */
  margin: 0 auto; /* 水平置中 */
  margin-top: 80px;
  font-size: 16px;
  text-decoration: none; /* 去掉連結的下劃線 */
  cursor: pointer; /* 鼠標樣式 */
}

.mainbtn:hover {
  background-color: #FFC300; /* 懸停效果：更深的黃色 */
}

@keyframes blink {
  from {
    border-color: transparent;
  }
  to {
    border-color: white;
  }
}

/* 避免文字因輪播產生抖動 */
.typing-container {
  position: relative;
  height: 3rem; /* 固定文字高度，避免輪播時跳動 */
}

.head:before,
.head:after {
  content: "";
  position: absolute;
  top: 0;
  height: 100%;
  width: 100%;
  background: inherit; /* 使用父背景，保持連續性 */
  background-size: inherit; /* 确保背景动画继承自父级 */
  animation: inherit; /* 确保动画继承自父级 */
}

.head:before {
  left: 0;
  clip-path: polygon(0 0, 50% 0, 60% 100%, 0 100%); /* 左邊斜切效果 */
}

.mt-16-a {
  display: flex;
  justify-content: center;
  align-items: center;
}

.mainc {
  display: block;
  justify-content: center;
  align-items: center;
  margin: 0,
}

.head:after {
  right: 0;
  clip-path: polygon(50% 0, 100% 0, 100% 100%, 40% 100%); /* 右邊斜切效果 */
}

/* 背景漸變動畫 */
@keyframes gradientAnimation {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}

.mx-auto {
  border-radius: 20px;
}

.egg {
  display: block;
  justify-content: center;
  margin: 50px auto;
  align-items: center;
  width: 300px;
  height: 300px;
  border-radius: 50%; /* 保持容器的圓形效果 */
  overflow: hidden; /* 確保內容不超出圓形範圍 */
  background: #f5f5f5; /* 可選：設置背景色 */
  position: relative; /* 用於內部圖片的定位 */
}

.photo {
  position: absolute; /* 確保圖片可以完全覆蓋容器 */
  top: 50%;
  left: 50%;
  width: 100%; /* 圖片寬度設置為容器的 100% */
  height: 100%; /* 圖片高度設置為容器的 100% */
  transform: translate(-50%, -50%) scale(1.4); /* 居中並填滿容器 */
  object-fit: cover; /* 確保圖片適應容器並裁剪 */
  transition: transform 0.3s ease-in-out; /* 添加平滑過渡效果 */
}

.photo:hover {
  transform: translate(-50%, -50%) scale(1.3); /* 懸停時放大 */
}

/* First Section (Portfolio) */
.first {
  width: 100%;
  text-align: center;
  padding: 20px;
}

.custom-btn {
  color: white !important; /* 确保覆盖默认文字颜色 */
  font-weight: bold; /* 可选：使文字更突出 */
}

/* Portfolio Items */
.child {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
  margin: 10px auto;
  max-width: 360px; /* 限制寬度 */
  text-align: center;
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* 添加陰影 */
}

.more {
  background: #88bccb;
  height: 40px;
  width: 90px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: white;
  border-radius: 100px;
  cursor: pointer; /* 鼠標移到按鈕上時的手勢 */
  transition: all 0.3s ease; /* 添加過渡效果 */
  margin: 0 5px; /* 確保按鈕在卡片內居中 */
  margin-bottom: 15px;
}

.more:hover {
  background: #5f9fa0; /* 添加 hover 效果 */
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.2); /* 提升效果 */
}


.pagecontent {
  display: flex;
  gap: 2px;
  margin: 0;
  padding: 0;
  justify-content: center;
  align-items: center;
  flex-direction: row;
}

/* Image Hover Section */
.imgHover {
  padding: 16px;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); /* 響應式 Grid */
  gap: 20px;
}

/* Pre Section */
.pre {
  width: 100%;
  text-align: center;
  padding: 20px;
  background-color: #ffffff;
  /* box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.1); */
}

/* Hire Section */
.hire {
  width: 100%;
  padding: 20px;
  text-align: center;
  background-color: #e9e9e9;
  margin-top: -24px;
}

/* 響應式設計 */
@media (max-width: 768px) {
  .v-container {
    padding: 8px;
  }
  .head {
    height: 300px; /* 減小高度 */
  }
  .egg {
    width: 200px;
    height: 200px;
  }



.photo {
  position: absolute; /* 確保圖片可以完全覆蓋容器 */
  top: 50%;
  left: 50%;
  width: 100%; /* 圖片寬度設置為容器的 100% */
  height: 100%; /* 圖片高度設置為容器的 100% */
  transform: translate(-50%, -50%) scale(1.4); /* 居中並填滿容器 */
  object-fit: cover; /* 確保圖片適應容器並裁剪 */
  transition: transform 0.3s ease-in-out; /* 添加平滑過渡效果 */
}

  .child {
    max-width: 100%;
    padding: 16px;
  }

  .imgHover {
    grid-template-columns: 1fr; /* 小螢幕一列展示 */
  }

  .center-content {
  padding-left: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left: 30px;
}

.mainc {
  padding-left: 0px;
}

.typing {
  font-size: 1.5rem;
  white-space: nowrap;
  overflow: hidden;
  border-right: 3px solid white;
  animation: blink 0.6s step-end infinite alternate; /* 光標閃爍效果 */
}


.mainbtn {
  display: flex;
  align-items: center; /* 垂直居中 */
  justify-content: center; /* 水平居中 */
  background-color: #000000;
  color: #ffffff;
  border-radius: 30px; /* 圓角按鈕 */
  width: 120px; /* 按鈕寬度 */
  height: 38px; /* 按鈕高度 */
  margin: 0 auto; /* 水平置中 */
  margin-top: 10px;
  font-size: 16px;
  cursor: pointer; /* 鼠標樣式 */
}

.mainbtn:hover {
  background-color: #FFC300; /* 懸停效果：更深的黃色 */
}

.text-white-a {
  font-size: 16px;
}


  /* 在 scoped 中使用深度選擇器 */
  ::v-deep(.active) {
    background-color: #88bccb !important;
    color: white !important;
  }

  .v-btn {
    background-color: #f5f5f5;
    color: black;
  }
}

@media (max-width: 768px) {
  .gradient-shape-left,
  .gradient-shape-right {
    width: 100px;
    height: 100px;
  }

  .gradient-shape-left {
    left: -20px; /* 确保图案不超出屏幕 */
  }

  .gradient-shape-right {
    right: -20px; /* 确保图案不超出屏幕 */
  }
  /* 隐藏 i1.png 的容器 */
.hide-on-mobile {
    display: none !important;
}
}



@media (max-width: 375px){
  .center-content {
  padding-left: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left: 20px;
  margin-top: 50px;
}
/* 隐藏 i1.png 的容器 */
.hide-on-mobile {
    display: none !important;
}

.mainc {
  display: block;
  justify-content: center;
  align-items: center;
  padding: 0px;
  width: 140px;
}

.mainbtn {
  display: flex;
  align-items: center; /* 垂直居中 */
  justify-content: center; /* 水平居中 */
  background-color: #000000;
  color: #ffffff;
  border-radius: 30px; /* 圓角按鈕 */
  width: 80px; /* 按鈕寬度 */
  height: 38px; /* 按鈕高度 */
  margin: 0 auto; /* 水平置中 */
  margin-top: 10px;
  font-size: 16px;
  cursor: pointer; /* 鼠標樣式 */
}
}




</style>