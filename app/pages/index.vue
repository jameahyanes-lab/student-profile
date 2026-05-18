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
                           placeholder="Yanes">
                           </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-text-field
                           label="First Name"
                           variant="outlined"
                           placeholder="Jameah Faith">
                           </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-text-field
                           label="Middle Name"
                           variant="outlined"
                           placeholder="Valencia">
                           </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-combobox
                           label="Course"
                           variant="outlined"
                           :items="['BSCS','DCT']"
                           clearable>
                           </v-combobox>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-combobox
                           label="Year"
                           variant="outlined"
                           :items="['1st Year','2nd Year','3rd Year','4th Year']"
                           clearable>
                           </v-combobox>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-combobox
                           label="Section"
                           variant="outlined"
                           :items="['A','B','C']"
                           clearable>
                           </v-combobox>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-text-field
                           label="Address"
                           variant="outlined"
                           placeholder="SAN SIMON, PAMPANGA">
                           </v-text-field>
                     </v-col>       

                     <v-col
                        cols="12"
                        md="4">
                           <v-text-field
                           label="Contact Number"
                           variant="outlined"
                           placeholder="09554818095">
                           </v-text-field>
                     </v-col>        
                     
                     <v-col
                        cols="12"
                        md="4">
                           <v-combobox
                           label="Gender"
                           variant="outlined"
                           :items="['Male','Female','LGBTQ']"
                           clearable>
                           </v-combobox>
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