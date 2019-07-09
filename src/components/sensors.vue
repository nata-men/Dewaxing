<template>
    <div id="app">
    <v-container grid-list-md text-xs-center  style="padding-top: 80px">
      <v-layout row wrap>
         <v-flex xs12>
          <v-card elevation=20>
            <v-card-title primary-title style="padding-bottom: 0;padding-left: 24px">
              <div class="headline">Показатели датчиков</div>
           </v-card-title>
            <v-card-text class="px-0" style="padding: 0">
                <v-container fluid grid-list-lg style="padding-top: 14px;">
                    <v-layout row wrap>
                        <v-flex xs12>
                            <hr color=#4CAF50 size="7" style="border-radius: 200px;">
                            <p class="text-sm-left" style="margin-top: 25px;font-size: 18px">Напряжение сети АВ, В</p>
                            <v-slider
                            color=#4CAF50
                            v-model="slider"
                            thumb-label
                            max="255"
                            ></v-slider>
                            
                            <p class="text-sm-left" style="font-size: 18px">Напряжение сети BC, В</p>
                            <v-slider
                            color=#4CAF50
                            v-model="slider"
                            thumb-label
                            ></v-slider>
                            
                            <p class="text-sm-left" style="font-size: 18px">Напряжение сети CA, В</p>
                            <v-slider
                            color=#4CAF50
                            v-model="slider"
                            thumb-label
                            ></v-slider>
                            
                            <p class="text-sm-left" style="font-size: 18px">Значение тензодатчика, В</p>
                            <v-slider
                            color=#4CAF50
                            v-model="slider"
                            thumb-label
                            ></v-slider>
                            
                            <p class="text-sm-left" style="font-size: 18px">Счетчик с датчика оборотов</p>
                            <v-text-field 
                                color=#4CAF50
                                v-if="type === 'number'" 
                                v-model="number" 
                                type="number" 
                                label="Количество оборотов">
                            </v-text-field>
                            
                            <div class="text-xs-right">
                            <v-btn round color=#4CAF50 dark widht="140px">Запуск</v-btn>
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
            slider: 45,
            type: 'number',
            number: 0
        }
      }
}
</script>