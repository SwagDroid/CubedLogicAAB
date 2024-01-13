<template>
  <v-form>
    <v-container>
      <v-row>
<v-col cols="12" sm="6" > <v-text-field label="Your product or service" model-value="Grocery delivery" hint="For example, flowers or used cars" ></v-text-field> </v-col>
<v-col cols="12" sm="6" ><v-text-field label="Your landing page" hint="www.example.com/page" persistent-hint></v-text-field></v-col>

<v-col
cols="12"
sm="6"
>
          <v-text-field
            label="Your product or service"
            model-value="Grocery delivery"
            hint="For example, flowers or used cars"
            variant="solo"
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          sm="6"
        >
          <v-text-field
            label="Your landing page"
            hint="www.example.com/page"
            persistent-hint
            variant="solo"
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          sm="6"
        >
          <v-text-field
            label="Your product or service"
            model-value="Grocery delivery"
            hint="For example, flowers or used cars"
            variant="outlined"
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          sm="6"
        >
          <v-text-field
            label="Your landing page"
            hint="www.example.com/page"
            persistent-hint
            variant="outlined"
          ></v-text-field>
        </v-col>
      </v-row>
    </v-container>
  </v-form>
  <v-row>
      <v-col cols="4">
        <v-list-subheader>Prefix for dollar currency</v-list-subheader>
      </v-col>

      <v-col cols="8">
        <v-text-field
          label="Amount"
          model-value="10.00"
          prefix="$"
        ></v-text-field>
      </v-col>
    </v-row>
</template>

<!-- <template>
  <v-form v-model="valid">
    <v-container>
      <v-row>
        <v-col
          cols="12"
          md="4"
        >
          <v-text-field
            v-model="firstname"
            :rules="nameRules"
            :counter="10"
            label="First name"
            required
            hide-details
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          md="4"
        >
          <v-text-field
            v-model="lastname"
            :rules="nameRules"
            :counter="10"
            label="Last name"
            hide-details
            required
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          md="4"
        >
          <v-text-field
            v-model="email"
            :rules="emailRules"
            label="E-mail"
            hide-details
            required
          ></v-text-field>
        </v-col>
      </v-row>
    </v-container>
  </v-form>
</template>
<script>
  export default {
    data: () => ({
      valid: false,
      firstname: '',
      lastname: '',
      nameRules: [
        value => {
          if (value) return true
          return 'Name is required.'
        },
        value => {
          if (value?.length <= 10) return true

          return 'Name must be less than 10 characters.'
        },
      ],
      email: '',
      emailRules: [
        value => {
          if (value) return true

          return 'E-mail is requred.'
        },
        value => {
          if (/.+@.+\..+/.test(value)) return true

          return 'E-mail must be valid.'
        },
      ],
    }),
  }
</script> -->

 