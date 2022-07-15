<template>
  <div id="body1">
    <div id="box">
        <div id="logo">
          <img src="@/assets/vuerity_logo.png" width="200" height="40" alt=""/>
        </div>
        
        <div id="user">
          <v-card
            border
            class="mb-2"
            density="compact"
            prepend-avatar="https://randomuser.me/api/portraits/men/32.jpg"
            subtitle="爵士鼓 读书 运动 电影 Popping"
            title="宋刚"
            variant="text">

            <v-img src="https://picsum.photos/512/128?image=660" height="128" cover></v-img>

            <v-card-text>
              最近恶补前端技术，持续冲电中。
            </v-card-text>

            <template v-slot:actions>
              <v-btn color="primary" variant="text">查看更多</v-btn>
            </template>
          </v-card>
        </div>

        <div id="message">
          <v-row justify="space-around">
            <v-card>
              <v-card-text>
                <div class="font-weight-bold ml-1 mb-2">
                  今日消息
                </div>

                <v-timeline
                  density="compact"
                  truncate-line="none"
                >
                  <v-timeline-item
                    v-for="message in messages"
                    :key="message.time"
                    :dot-color="message.color"
                    size="x-small"
                  >
                    <div class="mb-4">
                      <div class="font-weight-normal">
                        <strong>{{ message.from }}</strong> @{{ message.time }}
                      </div>
                      <div>{{ message.message }}</div>
                    </div>
                  </v-timeline-item>
                </v-timeline>
              </v-card-text>
            </v-card>
          </v-row>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TopComp',
  data(){
    return {
        username: 'Mark',
        messages: [
          {
            from: 'You',
            message: `Sure, I'll see you later.`,
            time: '10:42am',
            color: 'deep-purple lighten-1',
          },
          {
            from: 'John Doe',
            message: 'Yeah, sure. Does 1:00pm work?',
            time: '10:37am',
            color: 'green',
          },
          // {
          //   from: 'You',
          //   message: 'Did you still want to grab lunch today?',
          //   time: '9:47am',
          //   color: 'deep-purple lighten-1',
          // },
        ],
    }
  }
}
</script>

<style scoped>
  * {
    margin: 0px;
    padding: 0px;
  }

  #body1 {
    background-color: #030303;
    width: 100%;
    margin: 0px auto;
    font-family: 微软雅黑;
    font-size: 48px;
    height: 100px;
  }

  #logo {
    border: solid 2px #FFF;
    float: left;
    margin-top: 10px;
    margin-left: 20px;
  }

  #user {
    float: left;
    margin-top: 20px;
  }

  #message {
    float: left;
  }

</style>