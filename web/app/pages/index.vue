<template>
    <v-app>
        <v-main>
            <v-container>
                <v-row>

                    <v-col
                        cols="12">

                        <v-text-field
                            label="Student No."
                            prepend-inner-icon="mdi mdi-numeric"
                            variant="solo-inverted"
                            placeholder="24-00328">
                        </v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="4">

                        <v-text-field
                            label="Last Name"
                            prepend-inner-icon="mdi-account-box-outline"
                            variant="solo-inverted"
                            placeholder="Garcia">
                        </v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="4">

                        <v-text-field
                            label="First Name"
                            prepend-inner-icon="mdi-account-box-outline" 
                            variant="solo-inverted"
                            placeholder="Vincent">
                        </v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="4">

                        <v-text-field
                            label="Middle Name"
                            prepend-inner-icon="mdi-account-box-outline" 
                            variant="solo-inverted"
                            placeholder="Canlas">
                        </v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="4">

                        <v-combobox
                            label="Course"
                            prepend-inner-icon="mdi-account-details-outline" 
                            variant="solo-inverted"
                            :items="['BSCS','DCT',]"
                            clearable>
                        </v-combobox>
                    </v-col>

                    
                    <v-col
                        cols="12"
                        md="4">

                        <v-combobox
                            label="Year"
                            prepend-inner-icon="mdi-account-details-outline" 
                            variant="solo-inverted"
                            :items="['1st year','2nd year','3rd year','4th year']"
                            clearable>
                        </v-combobox>
                    </v-col>

                    <v-col
                        cols="12"
                        md="4">

                        <v-combobox
                            label="Section"
                            prepend-inner-icon="mdi-account-details-outline" 
                            variant="solo-inverted"
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
                            variant="solo-inverted"
                            placeholder="Laput, Mexico, Pampanga">
                        </v-text-field>
                     </v-col>

                      <v-col
                        cols="12"
                        md="4">

                        <v-text-field
                            label="Contact No."
                            prepend-inner-icon="mdi-card-account-phone-outline"
                            variant="solo-inverted"
                            placeholder="09233453123">
                        </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">

                        <v-combobox
                            label="Gender"
                            prepend-inner-icon="mdi mdi-gender-transgender"
                            :items="['Male','Female',' lGBTQ']"
                            variant="solo-inverted"
                            clearable>
                        </v-combobox>
                    </v-col>

                </v-row>
                    <v-btn 
                        prepend-icon="mdi mdi-tag-edit-outline"
                        variant="outlined"
                        color="green">
                        Edit
                    </v-btn>

                    <v-btn 
                        prepend-icon="mdi mdi-update"
                        variant="outlined"
                        color="blue">
                        Update
                    </v-btn>

                    <v-btn 
                        prepend-icon="mdi mdi-content-save-all-outline"
                        variant="outlined"
                        color="orange">
                        Save
                    </v-btn>

                    <v-btn 
                        prepend-icon="mdi mdi-delete-alert-outline"
                        variant="outlined"
                        color="red">
                        Delete
                    </v-btn>


                    <v-card
                        title="Student Profile"
                        flat>

                         <v-text-field
                            v-model="search"
                            label="Search"
                            prepend-inner-icon="mdi-magnify"
                            variant="outlined"
                            hide-details
                            single-line
                        ></v-text-field>

                        <v-data-table
                            :headers="titlecolum"
                            :items="nilalamanngcolum"
                            :search="search"
                        ></v-data-table>
                    </v-card>
            </v-container>
        </v-main>
    </v-app>
</template>

<script setup>
 const search = ref('')

const titlecolum = [
    {
        key: 'stuno', 
        title: 'Student Name'
    
    },

    {
        key: 'lname', 
        title: 'Last Name'
    
    },

    {
        key: 'fname', 
        title: 'First Name'
    
    },

    {
        key: 'mname', 
        title: 'Middle Name'
    
    },

    {
        key: 'ylevel', 
        title: 'Year Level'
    
    },

     {
        key: 'csection', 
        title: 'Section'
    
    },
]

const  nilalamanngcolum = [
    {
        stuno: '2400328', 
        lname: 'Garcia',
        fname: 'Vincent'
    },

    {
        stuno: '2400328', 
        lname: 'Garcia',
        fname: 'Vincent'
    },
    {
        stuno: '2400328', 
        lname: 'Garcia',
        fname: 'Vincent'
        mname: 'Canlas'
    },
 
    {
        stuno: '2400328', 
        lname: 'Garcia',
        fname: 'Vincent'
        mname: 'Canlas'
        ylevel: '2025-2026'
    },
 

    {
        stuno: '2400328', 
        lname: 'Garcia',
        fname: 'Vincent'
        mname: 'Canlas'
        ylevel: '2025-2026'
        csection: 'A'
    },
    
]
</script>
