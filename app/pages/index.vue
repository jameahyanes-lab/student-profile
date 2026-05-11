<template>
   <v-app>
         <v-main>
               <v-container>

                  <v-row>
                     <v-col   
                        cols="12"
                        >
                           <v-text-field
                           label="Student No."
                           variant="outlined"
                           placeholder="24-00892">
                           </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-text-field
                           label="Last Name"
                           variant="outlined"
                           placeholder="Dela Cruz">
                           </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-text-field
                           label="First Name"
                           variant="outlined"
                           placeholder="Juan">
                           </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-text-field
                           label="Middle Name"
                           variant="outlined"
                           placeholder="Santos">
                           </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="6">
                           <v-combobox
                           label="Gender"
                           variant="outlined"
                           :items="['Male','Female','LGBTQ']"
                           clearable>
                           </v-combobox>
                     </v-col>

                     <v-col
                        cols="12"
                        md="6">
                           <v-text-field
                           label="Age"
                           variant="outlined"
                           placeholder="18">
                           </v-text-field>
                     </v-col>                    
                  </v-row>
   
                     <v-btn
                        prepend-icon="mdi mdi-file-edit"
                        variant="outlined"
                        color="green"
                        >EDIT
                     </v-btn>

                     <v-btn
                        prepend-icon="mdi mdi-update"
                        variant="outlined"
                        color="blue"
                        >UPDATE
                     </v-btn>

                     <v-btn
                        prepend-icon="mdi mdi-content-save-check-outline"
                        variant="outlined"
                        color="orange"
                        >SAVE
                     </v-btn>

                     <v-btn
                        prepend-icon="mdi mdi-trash-can"
                        variant="outlined"
                        color="red"
                        >DELETE
                     </v-btn>

               </v-container>
         </v-main>
   </v-app>
</template>                