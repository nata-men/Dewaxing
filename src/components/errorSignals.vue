<template>
    <div id="app">
    <v-container grid-list-md text-xs-center>
      <v-layout row wrap>
         <v-flex xs12>
          <v-card elevation=20>
            <v-card-title primary-title style="padding-bottom: 0;padding-left: 24px">
              <div class="headline">Сигналы об ошибках</div>
           </v-card-title>
            <v-card-text class="px-0" style="padding: 0">
                <v-container fluid grid-list-lg style="padding-top: 14px;">
                    <v-layout row wrap>
                        <v-flex xs12>
                            <hr color=#4CAF50 size="7" style="border-radius: 200px;">   
                            
                            <v-switch v-model="people" color=#4CAF50>
                                <template v-slot:label>
                                    <div class="black--text"><big>Ошибка контроля питающей сети</big></div>
                                </template>
                            </v-switch>
                            
                            <v-switch v-model="people" color=#4CAF50>
                                <template v-slot:label>
                                    <div class="black--text"><big>Ошибка модуля МС</big></div>
                                </template>
                            </v-switch>
                            
                            <v-switch v-model="people" color=#4CAF50>
                                <template v-slot:label>
                                    <div class="black--text"><big>Ошибка модуля МR1</big></div>
                                </template>
                            </v-switch>
                            
                            <v-switch v-model="people" color=#4CAF50>
                                <template v-slot:label>
                                    <div class="black--text"><big>Ошибка ЧРП</big></div>
                                </template>
                            </v-switch>
                            
                            <v-switch v-model="people" color=#4CAF50>
                                <template v-slot:label>
                                    <div class="black--text"><big>Ошибка тензодатчик</big></div>
                                </template>
                            </v-switch>
                           
                            <v-switch v-model="people" color=#4CAF50>
                                <template v-slot:label>
                                    <div class="black--text"><big>Неклассифицированая ошибка</big></div>
                                </template>
                            </v-switch>
                            
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
        data () {
            return {
               
    }
  }
}</script>