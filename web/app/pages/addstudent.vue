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
                           prepend-inner-icon="mdi-numeric"
                           variant="outlined"
                           placeholder="24-00892">
                           </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-text-field
                           label="Last Name"
                           prepend-inner-icon="mdi-account"
                           variant="outlined"
                           placeholder="Yanes">
                           </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-text-field
                           label="First Name"
                            prepend-inner-icon="mdi-account"
                           variant="outlined"
                           placeholder="Jameah Faith">
                           </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-text-field
                           label="Middle Name"
                           prepend-inner-icon="mdi-account"
                           variant="outlined"
                           placeholder="Valencia">
                           </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">
                           <v-combobox
                           label="Course"
                           prepend-inner-icon="mdi-account-details-outline"
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
                           prepend-inner-icon="mdi-account-details-outline"
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
                           prepend-inner-icon="mdi-account-details-outline"
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
                           prepend-inner-icon="mdi-map-marker-outline"
                           variant="outlined"
                           placeholder="SAN SIMON, PAMPANGA">
                           </v-text-field>
                     </v-col>       

                     <v-col
                        cols="12"
                        md="4">
                           <v-text-field
                           label="Contact Number"
                           prepend-inner-icon="mdi-card-account-phone-outline"
                           variant="outlined"
                           placeholder="09554818095">
                           </v-text-field>
                     </v-col>        
                     
                     <v-col
                        cols="12"
                        md="4">
                           <v-combobox
                           label="Gender"
                           prepend-inner-icon="mdi-gender-transgender"
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
                        >SAVE
                     </v-btn>

                     <v-btn
                        prepend-icon="mdi mdi-update"
                        variant="outlined"
                        color="blue"
                        >EDIT
                     </v-btn>

                     <v-btn
                        prepend-icon="mdi mdi-content-save-check-outline"
                        variant="outlined"
                        color="orange"
                        >UPDATE
                     </v-btn>

                     <v-btn
                        prepend-icon="mdi mdi-trash-can"
                        variant="outlined"
                        color="red"
                        >DELETE
                     </v-btn>

                      <v-card
                        title="Student Profile"
                        flat
                     >
                        <template v-slot:text>
                           <v-text-field
                           v-model="hanapstudent"
                           label="Search"
                           prepend-inner-icon="mdi-magnify"
                           variant="outlined"
                           hide-details
                           single-line
                           ></v-text-field>
                        </template>

                        <v-data-table
                           :headers="titlecolumn"
                           :items="nilalamanngcolumn"
                           :search="hanapstudent"
                        ></v-data-table>
                     </v-card>

               </v-container>
         </v-main>
   </v-app>
</template>                

  <script setup>
      const hanapstudent = ref('')
                     
      const titlecolumn = [
         {
            key: 'studno', title: 'Student Number'           
         },
         {
            key: 'lname', title: 'Last Name'           
         },
         {
            key: 'fname', title: 'First Name'           
         },
         {
            key: 'mname', title: 'Middle Name'           
         },
         {
            key: 'course', title: 'Course'           
         },
          {
            key: 'year', title: 'Year'           
         },
         {
            key: 'section', title: 'Section'           
         },
         {
            key: 'address', title: 'Address'           
         },
         {
            key: 'contact', title: 'Contact Number'           
         },
         {
            key: 'gender', title: 'Gender'           
         },
      ]

      const nilalamanngcolumn = [
         {
            studno:'24-00892',
            lname: 'Yanes',
            fname: 'Jameah Faith',
            mname: 'Valencia',
            course: 'DCT',
            year: '2nd Year',
            section: 'B',
            address: 'San Simon',
            contact: '09454077324',
            gender: 'Female',
         }
      ]

 </script>