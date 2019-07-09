<template>
    <div id="app">
    <v-container grid-list-md text-xs-center>
      <v-layout row wrap>
         <v-flex xs12>
          <v-card elevation=20>
            <v-card-title primary-title style="padding-bottom: 0;padding-left: 24px">
              <div class="headline">Работа установки</div>
           </v-card-title>
            <v-card-text class="px-0" style="padding: 0">
                <v-container fluid grid-list-lg style="padding-top: 14px;">
                    <v-layout row wrap>
                        <v-flex xs12>
                            <hr color=#4CAF50 size="7" style="border-radius: 200px;">   
                            <p></p>
                            <v-card style="border: 3px solid #4CAF50;border-radius: 20px;">
                                <v-list class=#E8F5E9>
                                <v-list-tile 
                                      v-for="item in items"
                                      :key="item.title"
                                      @click="">
                                <v-list-tile-title v-text="item.title" ></v-list-tile-title>
                                </v-list-tile-content>
                                </v-list-tile>
                                </v-list>
                            </v-card>
                            
                            <v-text-field
                              color=#4CAF50
                              value=""
                              label="Причина остоновки процесса"
                              readonly
                            ></v-text-field>
          
                              
                        
                            <div class="text-xs-right">
                            <v-btn round color=#4CAF50 dark widht="140px">Остановить процесс</v-btn>
                            </div>
                        </v-flex>
                    </v-layout>
                </v-container>                    
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
    </div>
</template>

<script>
export default{
    data (){
        return {
            items: [
        { title: 'Процесс 1'},
        { title: 'Процесс 2'},
        { title: 'Процесс 3' },
        { title: 'Процесс 4' }
      ]
        }
      }
}
</script>