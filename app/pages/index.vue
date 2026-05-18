<template>
    <v-app>
        <v-main>
            <v-container>
                <v-row>

                    <v-col
                        cols="12">

                        <v-text-field
                            label="Student no"
                            variant="outlined"
                            placeholder="24-00328">
                        </v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="4">

                        <v-text-field
                            label="Last Name"
                            variant="outlined"
                            placeholder="Garcia">
                        </v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="4">

                        <v-text-field
                            label="First Name"
                            variant="outlined"
                            placeholder="Vincent">
                        </v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="4">

                        <v-text-field
                            label="Middle Name"
                            variant="outlined"
                            placeholder="Canlas">
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
                    
                    <v-col
                        cols="12"
                        md="4">

                        <v-text-field
                            label="Age"
                            variant="outlined"
                            placeholder="18 Years Old">
                        </v-text-field>
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