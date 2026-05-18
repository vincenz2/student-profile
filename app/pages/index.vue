<template>
    <v-app>
        <v-main>
            <v-container>
                <v-row>

                    <v-col
                        cols="12">

                        <v-text-field
                            label="Student no"
                            variant="solo-inverted"
                            placeholder="24-00328">
                        </v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="4">

                        <v-text-field
                            label="Last Name"
                            variant="solo-inverted"
                            placeholder="Garcia">
                        </v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="4">

                        <v-text-field
                            label="First Name"
                            variant="solo-inverted"
                            placeholder="Vincent">
                        </v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="4">

                        <v-text-field
                            label="Middle Name"
                            variant="solo-inverted"
                            placeholder="Canlas">
                        </v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="4">

                        <v-combobox
                            label="Course"
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
                            variant="solo-inverted"
                            placeholder="Laput, Mexico, Pampanga">
                        </v-text-field>
                     </v-col>

                      <v-col
                        cols="12"
                        md="4">

                        <v-text-field
                            label="Contact No."
                            variant="solo-inverted"
                            placeholder="09233453123">
                        </v-text-field>
                     </v-col>

                     <v-col
                        cols="12"
                        md="4">

                        <v-combobox
                            label="Gender"
                            variant="solo-inverted"
                            :items="['Male','Female',' lGBTQ']"
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
            </v-container>
        </v-main>
    </v-app>
</template>