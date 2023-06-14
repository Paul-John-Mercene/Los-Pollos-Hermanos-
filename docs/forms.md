# Forms

<box header>
    A forms component in Vue is a collection of reusable user interface elements and functionalities that facilitate the creation and management of interactive forms within an application. Forms are essential for capturing user input, collecting data, and enabling user interactions.

## Default

We have the `v-form` component. Whenever the value of an input is changed, each rule receives a new value and is re-evaluated. If a rule returns false or a string, validation has failed and the string value is presented as an error message.

<vuecode md>
<div slot="demo">
<template>
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

              return 'Name is requred.'
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
    </script>

    </div>
    </vuecode>
    </box>
